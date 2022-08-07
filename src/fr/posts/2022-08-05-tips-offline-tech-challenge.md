---
title: Conseils pour son challenge technique offline
description:
date: "2022-08-05"
tags: [tech, challenge, job]
image: ""
translationKey: "post_offline_challenge_tips"
---

Postuler à un job dans la tech vient, le plus souvent, avec son lot de tests techniques. Live coding, deep dive, QCM,... chaque type d'entretien vient avec son lot d'avantages et inconvénients - pour le recruteur et pour le candidat !

J'ai déjà porté les deux casquettes, et maintenant que je suis plutôt celle qui fait passer les entretiens, j'aimerai partager les conseils que je pense être valuables pour toute personne passant un entretien.

> Ça ne veut pas dire qu'en suivant ces conseils, vous réussirez forcément votre entretien !

Je vous donne ici des clés pour avoir une approche plus claire, propre et organisée, ce qui sont des qualités généralement recherchées par les personnes qui vont vous recevoir en entretien. Évidemment, le niveau et les qualités attendues dépendent de l'entreprise à laquelle vous postulez; mais les conseils donnés ci-après sont - selon moi - des éléments essentiels qui ne peuvent que jouer en votre faveur. Voire potientiellement jouer en votre défaveur s'ils n'y sont pas ou pas bien présentés (encore une fois, dépendemment des attentes de l'entreprise).

On commence cette série avec des conseils pour **le coding challenge offline** ! J'ai nommé cet exercice avec des instructions plus ou moins précises que l'on vous donne à travailler chez vous dans un temps donné.

⚠️ Je suis développeuse front-end et donne des conseils plutôt porté sur un test JS / TS, mais la plupart sont appliquables quelque soit le langage et le type de challenge.

# 10 tips for rocking your front-end coding challenge

## The instructions you will read very carefully

Ça paraît extrêmement basique comme conseil, mais c'est pourtant le plus important. Lire les consignes, s'assurer de les comprendre. S'il y a le moindre doute, ne pas hésiter à demander des clarifications aux contacts qui vous ont envoyé le coding challenge. Si les instructions sont longues ou complexes, on peut aussi les reformuler de son côté, sous forme de TODO liste par exemple. Il est aussi important à ce stade de définir les élements primaires et secondaires.

Exemple: Créer une application web qui affiche un formulaire avec un champ texte et un bouton "rechercher". Quand on clique sur "rechercher", afficher une liste d'items parmi la liste [qu'on vous donne via API ou fichier JSON].
La demande est super floue, et c'est parfois fait exprès. Mais les élements absolument essentiels dans cette demande sont :

- Une app web (une page, Vanilla, React, ce que vous voulez)
- Un text field et un submit button
- sur le click du submit button, afficher la liste des items en fonction de la recherche.
  - ça sous-entend généralement aussi un état de chargement, où un loading spinner ou un texte apparaitra le temps du chargement

Et THAT'S IT
Évidemment, c'est ensuite à votre appréciation d'ajouter des bonus - qui par définition viennent après que les éléments principaux soient réalisés

- Une validation du formulaire
- Un message spécifique quand la liste retournée est vide
- Attention particulière donnée à l'UI / UX
- Accessibilité
- Internationalisation
- Déployer l'application sur Github pages / Heroku / Netlify...
- [une liste qui s'étend à l'infini]

Une fois seulement que les instructions sont claires et comprises, et que vous avez déterminé les éléments principaux et essentiels, vous pouvez commencer à voir comment coder. Les avantages de faire l'exercice dans ce sens est que:

- on s'assure de comprendre et de ne rien oublier par rapport aux instructions données, le travail qui en découle est plus organisé
- la solution choisie peut dépendre des instructions: l'exercice demande du Vanilla / VueJS / React ? Est-ce que j'ai besoin d'une SPA / routing ? Est-ce que j'ai un state complexe à gérer (spoiler: non la plupart du temps)? etc...

Vous voilà lancés, et par définition, vous prendrez vos premiers choix techniques et architecturaux, ce qui m'amène au second point: restez aussi simples que possible.

## KISS - Keep It Simple Stupid

Même si le challenge que l'on vous a envoyé vous passionne, vous n'avez probablement pas ni envie ni le temps d'y consacrer un temps fou. Et personne [de censé] ne pourra vous le reprocher. Vous avez le droit de choisir tel librairie ou framework parce que vous êtes à l'aise avec pour aller vite. Ou de choisir une implémentation plus naïve / simple parce qu'elle suffit dans le cadre de ce projet.

Le test technique ne doit pas être une application boostée aux stéroïdes parce que vous vouliez montrer l'intégralité de vos connaissances. Appliquez-les plutôt intelligemment et simplement, selon le besoin de l'application (ce conseil est aussi valable pour n'importe quel projet). Quelque soient vos choix, pensez simplement à le mentionner dans la section documentation - voir plus bas.

Exemple: Je connais Redux sur le bout des doigts. L'application me demande d'afficher une liste d'items; ai-je vraiment besoin d'une telle implémenatation dans ce cadre ?

### Run the app

Pensez à expliquer comment lancer votre application ! Aidez les personnes qui vous relisent et faites-leur gagner du temps. Il s'agit également d'une bonne pratique sur tout projet d'indiquer comment lancer l'application ainsi que les tests s'il y en a

```bash
# Install dependencies
npm install

# Start application: this will run the app in the development mode.
# Open http://localhost:3000 to view it in the browser.
npm start

# Run unit tests
npm run test
```

## Documentation you will write

Quand on passe un entretien en direct on peut facilement décrire le fond de sa pensée. Mais quand on est seuls face à son exercice, c'est souvent quelque chose que l'on oublie de faire (même professionnellement, même les plus aguéris): expliquer, documenter. Lorsque vous rendrez votre test technique, une documentation pourra guider la personne qui relit votre challenge au travers de votre démarche.

### Technial choices

De mon point de vue, les choix techniques pris par un candidat lors de son challenge importent peu, tant qu'il est capable d'expliquer pourquoi il les a fait. Sans explication, difficile de dire si le candidat est parti dessus parce que c'était ce qu'il connaissait ou si c'était par conviction que c'était le meilleur choix pour ce cas d'usage. Et quand bien même les explications peuvent amener à poser des questions, les choix techniques et les explications qui y sont associées pourront ensuite être challengés dans la suite du process.

À la base de votre projet, vous pouvez créer un README.md s'il n'existe pas déjà et y écrire une section sur ces choix techniques - ou non choix techniques.

Exemple 1: L'application comportait un formulaire et un bouton, ce qui m'a amené à créer une validation du formulaire simple, directement dans le code. Cependant, sur une application de production qui aurait besoin de scaler, on pourra penser à intégrer une librairie comme par exemple [lib de validation de formulaire de votre choix].

Exemple 2: Afin de délivrer une expérience utilisateur agréable et de gagner du temps, j'ai utilisé [nom de la librairie UI de votre choix]. Cette librarie est légère et propose les composants dont j'avais besoin pour composer facilement l'interface de l'application.

Les explications peuvent porter sur le language (pourquoi Typescript?), les libraries / frameworks utilisées, la façon dont vous avez architecturé le code, le state management que vous avez (ou pas) utilisé...

Tous vos choix découlent de décisions et de votre expérience, et cette démarche de tout expliquer ne pourra qu'éclairer la personne qui relira votre challenge.

## Consistency you will keep

Le but est de créer un code qui induit le moins de charge cognitive possible pour le reviewer. Une façon d'aider est d'avoir un code consistant: toujours les mêmes spacings, organisation d'imports, convention de nommage des variables...

Il existe une multitude d'outils qui nous permettent d'avoir un code consistent et facile a lire. Je nomme simplement [ESLint](https://eslint.org/) et [Prettier](https://prettier.io/), qui prennent respectivement seulement quelques minutes à installer.

Dans la même idée, mettez-vous d'accord avec vous mêmes (ou avec les instructions) sur la façon dont vous allez nommer vos fonctions, composants et variables: camel case / snake case ? Noms de fichiers commençant par une majuscule ? Hierarchie de fichiers ? ...

## Be clear!

Pas tant une question de consistence, mais veillez le plus possible à garder un code simple à lire. Une personne tierce va passer derrière vous et va checher à comprendre ce que vous avez codé. Il existe des moyens simples d'avoir un code simple à lire:

- nommer ses variables, composnats et fonctions de façon significative
- limiter l'identitation: une fonction ou un composant qui contient trop de niveaux d'indentation peut probablement être redécoupé dans une fonction / composant / variable avec un nom représentatif
- éviter les ternaires imbriquées
- éviter les fichiers / fonctions trop longs. Cela peut passer par des partterns comme 1 composant / fonction = 1 responsabilité.

Si vous sentez le besoin de rajouter un commentaire dans votre code pour aider à comprendre un élément en particulier, n'hésitez pas à le faire. Cela peut cependant parfois être un code smell indiquant que votre code devrait être écrit différemment ou refactorisé - mais d'autres fois il peut apporter de la valeur dans la clarification.

### Possible improvements

Vous avez passé un certain temps sur ce test technique. Vous avez implémenté les éléments essentiels, mais vous avez dépensé tout votre quota de temps pour ce challenge. Tout va bien ! Il suffit alors d'écrire les choses que vous n'avez pas eu le temps d'implémenter. Si jamais vous avez eu l'impression de tout implémenter - restez humbles, aucun code ni aucune app ne sont jamais parfaits. Cherchez les améliorations, les choses qui manqueraient, techniques ou en terme de feature. Il est extrêmement important d'être objectif sur son code. Et si vous ne trouvez toujours pas quoi dire, vous pouvez toujours ajouter des notes sur comment l'application pourrait évoluer dans le cas où on demanderait de la scaler (rajouter des features, des personnes pour travailler dessus, des masses d'utilisateurs, rendre l'app accessibile, optimisations...)

Exemple 1 - l'amélioration tech: Je n'ai pas eu le temps d'implémenter les tests unitaires pour tous les composants. À l'image de [ce composant que vous avez pu tester], il s'agirait de continuer ce process pour tous les autres composants de l'application.

Exemple 2 - l'amélioration produit: l'API me retournait d'autres éléments qui auraient été intéressants de montrer aux utilisateurs comme [telle propriété]. De plus, il est possible d'ajouter une fonction de filtre / tri / pagination qui améliorerait l'expérience utilisateur la liste retournée est parfois très grande.

Cette section peut paraître annodine, mais elle peut vous sauver si vous n'avez simplement pas eu le temps de tout faire. Pas la peine de cacher la poussière sous le tapis, les personnes qui vont vous relire ne sont pas dupes; prennez les devant, expliquez tout, et cela vous permettra de vous défendre lors d'un potentiel entretien de debriefing.

## API tokens you won't commit

Les tokens ou clés d'API ou tout autre secret dont vous pourriez avoir besoin ne doivent **jamais** être commités ni présents en clair dans votre code. Utilisez des variables d'environnement, et potentiellement une librairie pour accéder à celles-ci (je pense à la célèbre [nconf](https://github.com/indexzero/nconf#readme) mais il y en a probablement plein d'autres).

Il s'agit là encore d'une bonne pratique non seulement pour les tests techniques mais aussi pour toute application que vous pourriez être amené à écrire.

## Tests you will write (if you have time)

Dans un monde idéal, on a le temps d'écrire des tests: unitaires d'abord, intégration si possible et idéalement un petit end-to-end test. Mais - comme dans la vraie vie - cela prend généralement du temps. Si vous arrivez à la fin du temps qui vous est imparti et que vous n'avez pas écrit votre application en TDD (rarement le cas pour du front-end), essayez si possible de rajouter au moins des tests unitaires / intégration sur le composant principal de votre application. Cela permettra d'appuyer le fait que vous savez quand même faire et d'avoir un cas d'exemple concret à montrer.

Et si vous ne savez pas faire ou n'avez pas le temps, alors écrivez-le dans la section "Améliorations possibles" dans votre compte rendu. N'hésitez alors pas à y indiquer les scénarios que vous auriez testé et quelle librairie vous auriez pu utiliser - et pourquoi.

## Commit messages

Idéalement, et comme dans tout projet, il est conseillé de ne pas pousser tout son code d'un seul coup. Vous allez construire votre application de façon itérative, et cela devrait pouvoir se retrouver dans les commit history de votre branche.

Cela n'a pas besoin d'être parfait, mais au moins de refléter votre processus d'implémentation de l'app

Exemple:

- init app
- create search form
- API call to search for the items
- list all the items
- loading state
- ...

Si vous voulez aller plus loin dans les types de commits que vous pourriez écrire, il existe aujourd'hui beaucoup de conventions de commit sur lesquels vous pouvez vous baser. Je pense notament à [Conventional commits](https://www.conventionalcommits.org/en/v1.0.0/), il en existe d'autres.

## Read youself!

Enfin, quand vous aurez terminé, je ne peux que vous encourager de sortir votre corps, de vous mettre à la place de la personne qui va découvrir votre projet. Relisez tout, le README, le code sur Github (ou peu importe la plateforme). Cela vous permettra d'identifier des potentiels points à améliorer - que vous aurez soit le temps de corriger, soit de rajouter comme piste d'amélioration dans le README !

Vérifiez également que

- il ne reste aucun élément du boilerplate que vous n'utilisez pas (assets, tests unitaires qui ne correspondent plus à rien...)
- l'intention derrière votre code est claire, que celui-ci est lisible

# Conclusion

Je me rends compte en écrivant cet article que tous ces conseils peuvent paraître comme beaucoup de charge mentale. Gardez simplement en tête que votre test n'a pas à être parfait. Aussi que:

- la personne qui va vous lire est un humain - et potentiellement votre futur collègue ! Aidez le à se projeter. Le plus simple vous rendez son travail, le plus satisfait il pourra être - cela passe par de l'organisation et des explications
- vous avez un temps limité pour ce challenge: si vous n'en avez pas de défini dans le test que l'on vous a envoyé, donnez vous une limite que vous noterez dans le README. Ce n'est pas votre travail principal d'écrire ce challenge et vous ne devriez pas y passer un temps démeusuré
