---
title: Live coding challenge tips
description:
date: "2022-08-27"
tags: [tech, challenge, job]
image: "/images/live-coding-challenge/computer-girl.jpg"
translationKey: "post_live_coding_challenge_tips"
---

On continue la série avec les tant redoutés **live coding challenges** ! Personnellement, j'ai la boule au ventre rien que de lire l'email qui me dit que je devrais en passer un pendant un processus de recrutement (et ça fait 10 ans que je dev).

Postuler à un job dans la tech vient, le plus souvent, avec son lot de tests techniques. Live coding, deep dive, QCM... chaque type d'entretien comporte son lot d'avantages et inconvénients.

Ayant porté les deux casquettes, maintenant je suis plutôt celle qui fait passer les entretiens. Je partage donc ici les conseils qui pourront vous aider si jamais vous en passez ou allez en passer.

> Ça ne veut pas dire qu'en suivant ces conseils, vous réussirez forcément votre entretien !

Je vous donne ici des clés pour avoir une approche plus claire, propre et organisée, ce qui sont des qualités généralement recherchées par les personnes qui vont vous recevoir. Évidemment, le niveau technique et les autres qualités attendues dépendent de l'entreprise et du poste auquel vous postulez; mais ces conseils sont des éléments essentiels qui ne peuvent que jouer en votre faveur. Voire potentiellement jouer en votre défaveur s'ils n'y sont pas ou pas bien présentés.

# Tips pour un live coding challenge

## Le live coding challenge

Le but c'est de résoudre un ou plusieurs exercices tech **en live** devant une ou plusieurs personnes. Ce genre de test est difficile et particulièrement redouté car **on se retrouve comme mis à nu devant un ou plusieurs inconnus** qui nous jugent en temps réel, ce qui laisse peu de place à l'erreur. En tout cas, c'est ce qu'on se dit.

## Un test à double sens

Comme pour n'importe quel entretien, le but doit toujours rester le même: **donner envie à la personne en face de travailler avec vous.**. Mais cette fois c'est valable dans les deux sens; il faut aussi que les personnes en face vous donnent envie de travailler avec elles - se retrouver en face d'un \*\*\* prétentieux donne très peu envie de rejoindre l'entreprise !

Mon tip est alors d'aborder cet entretien comme un échange, une discussion voir même comme une session de mob-programming. Ça peut-être vos futurs collègues que vous rencontrez pour la première fois. Ces personnes en face ne sont pas de simples spectateurs, ils doivent pouvoir vous accompagner, répondre à vos questions, vous débloquer au besoin.

### Avant l'entretien, la préparation

Comme pour tout entretien, l'idéal c'est déjà de faire ses recherches avant et de préparer des questions. En plus de donner du contexte, cela permet d'avoir des questions à poser en fin d'entretien. On peut alors fouiller des conférences, blogs techniques, publications... C'est non seulement important pour montrer son intérêt dans l'entreprise, mais aussi et surtout pour montrer qu'on se projette.

Concernant la partie technique, le processus est parfois communiqué à l'avance, ce qui rend alors relativement simple de savoir sur quoi plancher. Si non, plusieurs possibilités et ressources:

- l'entreprise est connue: [Glassdoor](https://www.glassdoor.fr/) recense des témoignages d'entretiens de candidats qui peuvent alors donner une indication du type d'exercice habituellement donné.
- si rien n'apparaît sur GlassDoor, il est toujours possible de s'entraîner gratuitement sur des plateformes comme [CodingGame](https://www.codingame.com/) sur des exercices plus ou moins complexes.

## Pendant l'entretien

### La consigne

Ça paraît extrêmement basique comme conseil, mais c'est pourtant le plus important. **Lire les consignes, s'assurer de les comprendre. et ÉCOUTER.** S'il y a le moindre doute sur une consigne, poser des questions. Il vaut mieux faire répéter que de partir à côté des ronces. Une façon plus habile de s'assurer qu'on a bien compris (ou justement qu'on n'est pas sûr de comprendre) est de reformuler l'exercice avec ses propres mots, et demander si c'est bien ce qui est attendu.

## Donner le meilleur de soi-même

Le syndrôme le plus courant que j'ai pu noter chez les développeurs c'est **l'over-engineering**.

> "Super easy, je sais faire, alors go pour un double reduce imbriqué !"

Expectation VS Reality: On oublie le return, les paramètres sont dans le mauvais sens, on a mal initialisé la fonction et on a fait une typo à chaque mot.

Avec le stress, c'est en fait super difficile de sortir du code sur un éditeur que vous ne maîtrisez probablement pas - probablement sans auto-complétion, et avec des gens qui regardent et dont vous pensez juger chaque typo. Même quand on a l'habitude. Même quand on est Senior !

<mark>Globalement, et surtout quand on est stressé, #1 tip: ITÉRER.</mark>

```
Exemple: commencer avec une première boucle `for`, des variables mutées par-ci par-là. Puis extraire dans une fonction. Puis utiliser plutot un `.map` (ou pourquoi pas un `reduce` si vraiment vous le sentez). etc
```

<mark>Et le secret qui n'en est pas un - conseil #2 PARLER.</mark>

Super important pour éviter de s'isoler dans son exercice et faire comprendre son intention aux personnes en face. Elles pourront ainsi comprendre, vous aider ou vous challenger. **Vous vous donnez une chance d'argumenter sur vos choix tout en montrant que vous êtes objectif sur votre code.**

```
Exemple : "Là je pars sur une approche naïve pour commencer, ça n'est pas idéal parce que ça n'est pas une solution très performante mais je vais revenir dessus par la suite."
```

<mark>Et si le résultat n'est pas à la hauteur escomptée **dédramatisez**.</mark>

Les personnes en face savent que c'est un exercice stressant et que personne n'est en possession de tous ses moyens.

## Gérer son stress

Le jour J, qu'on se soit préparé pendant des semaines ou pas du tout, on est généralement **hyper stressé** (sauf des personnes surhumaines dont je ne ferai jamais partie).

Le stress est en fait plutôt bon **à petite dose**. Il permet d'être concentré, de chercher à se dépasser pendant l'exercice. Mais il est primordial de ne pas se laisser déborder. Plusieurs techniques existent:

- Se connaître
- Préparer l'entretien
- Poser des questions

### Se connaître

C'est difficile de savoir connaître nos réactions avant d'être confronté à la situation. Est-ce qu'en situation de stress devant des gens, j'ai tendance à bloquer / faire des blagues / parler trop ... ?

C'est souvent après plusieurs entretiens qu'on apprend à mieux se connaître, au travers de ce qu'on ressent mais aussi des feedback que l'on peut recevoir (ou demander à recevoir) après l'entretien.

## Poser des questions

Posez des questions en rebondissant sur le test ou remarques des intervenants; "est-ce que vous utilisez une convention / lib / archi / process ? etc". Cela montre que vous vous intéressez et peut vous donner des indications sur la façon dont les équipes travaillent.

Entraînez-vous si possible **à parler en codant**. On a rarement ce besoin au quotidien, c'est donc assez peu naturel et probablement déstabilisant au début. Au moins de lever la tête entre quelques lignes de code pour expliquer ce qu'on cherche à faire. **Demander de l'aide si on est bloqué.**

Garder le contact avec les personnes en face est primordial. Oui c'est un test technique mais il n'en reste pas moins qu'une part importante de la réussite de ce challenge est attribuée à la communication, au feeling car c'est une composante primordiale dans notre vie quotidienne (même les devs oui oui).

## À la fin de l'entretien

C'est le moment idéal de dire ce que vous avez pensé du test et de votre performance. L'idéal c'est de donner des pistes d'améliorations sur le code rendu, que ce soit technique, fonctionnel, d'un point de vue QA, performance, etc.

<mark>Aucun code n'est parfait (et certainement pas du code issu d'un live coding challenge). Tip #3: rester objectif et humble !</mark>

# Conclusion

Les live coding challenges sont difficiles et stressants, c'est normal de les ressentir comme tels. Les personnes en face - nos futurs collègues ? - sont là pour nous aider et nous mettre à l'aise. Comptez-sur eux, mais aidez-les en gardant la communication ouverte continuellement.
