---
title: Design Patterns en Sketchnote
description:
date: "2022-10-11"
tags: [sketchnote, design patterns, softskill]
image: "/images/sketchnote-patterns/title.png"
translationKey: "post_sketchnote_design_patterns"
---

# Initiative

On utilise tellement d'outils, de frameworks, on lit tellement de code au quotidien... Je voulais prendre un moment pour repartir sur les bases de ce que j'avais pu voir à l'école et que je voyais repasser ici et là dans ma vie quotidienne. Afin de mieux comprendre. D'améliorer ma reflexion face à des problèmes.

J'ai été très surprise de voir que les sketchnotes publiés sur Twitter avaient reçu un certain engouement; je les fais avec plaisir sur mon temps libre et chaque like, chaque message est une récompense que je n'attendais pas. Cela est aussi venu avec des débats passionnés et instructifs, notamment sur le Singleton pattern.

Tous les sketchnotes sur les design pattern que je réalise sont et seront ajoutés dans cet article.

La majorité du contenu des sketchnotes sont basés sur le site https://refactoring.guru

# SOLID

5 principes de base OOP #SOLID que l’on retrouve parfois dans certain des patterns cités ensuite !

Il s’avère que ces principes sont plus récents que je ne le pensais initialement 😇

![SOLID](/images/sketchnote-patterns/solid.jpg)

# Singleton

La série des design patterns en sketchnote commence avec le Singleton. Largement utilisé dans les frameworks front-end, mais n'est pas toujours une bonne pratique quand il s'agit de l'implémenter dans notre code.

Des débats enflammés sur Twitter à propos de bonne pratique quant à l'utilisation de ce pattern: https://twitter.com/AmelieBenoit33/status/1570313646605234177 - j'en ferai un résumé bientôt !

![Singleton](/images/sketchnote-patterns/singleton.jpg)

# Builder

Ça me fait penser au constructeur de personnage qu’on retrouve dans les Sims ou certains RPGs (des semaines passées sur Baldur's Gate, mon enfance ❤️)

J’utilise souvent ce pattern pour construire des jeux de données dans des tests unitaires - cependant pas toujours avec un Director.

![Builder](/images/sketchnote-patterns/builder.jpg)

# Observer

Il peut s’apparenter à un système d’abonnement (magazine, journal, channel YouTube…) où le publisher appelle une méthode des abonnés lorsqu’un événement survient.

Très utilisé en frontend dans divers contextes !

![Observer](/images/sketchnote-patterns/observer.jpg)

# Adapter

Simple et efficace à mettre en place, il permet aux clients de consommer des api ou des données de façon uniforme.

![Adapter](/images/sketchnote-patterns/adapter.PNG)
