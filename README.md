# Laboratoire 2 — Redresseur Actif Triphasé (AFE) & Simulation HIL

Ce dépôt contient l'ensemble des fichiers de simulation PLECS, des schémas temps réel (RT-Box / TI ControlCARD) ainsi que l'analyse complète réalisée dans le cadre du **Laboratoire 2 d'Électronique de Puissance II**. (Nous tenons à mentionner que nous nous sommes servis de Google IA afin de comprendre certaines de nos erreurs lors de nos simulations PLECS.)

## Où trouver le rapport ?
* **Le rapport principal attendu est le fichier [`PI.ipynb`](./PI.ipynb).**
* Vous pouvez le consulter directement dans votre navigateur en cliquant sur le fichier ci-dessus : l'ensemble des graphiques, tableaux comparatifs, schémas et interprétations y sont déjà intégrés et affichés.

## Objectif et public visé
Ce rapport a été rédigé de manière détaillée et pédagogique afin d'être accessible à **tout lecteur souhaitant comprendre en profondeur le fonctionnement, le dimensionnement et le comportement d'un redresseur actif triphasé (Active Front-End)** — depuis la modélisation et le réglage des boucles de régulation en cascade jusqu'à l'implémentation matérielle *Hardware-in-the-Loop* (HIL).

## Retour d'expérience & état d'avancement
* **Investissement :** La réalisation complète de ce laboratoire (modélisation, débogage des boucles, tests paramétriques, mise en œuvre sur banc temps réel et rédaction) a représenté environ **40 heures de travail**, marquées par de nombreux défis techniques et problèmes de synchronisation/configuration résolus au fil des essais.
* **Gains :** Ce laboratoire nous a permis de nous familiariser avec les notions vues en cours de manière beaucoup plus concrète que lors de la lecture d'un pdf. Nous avons également pu comprendre comment implémenter des boucles de régulation plus complexe notamment en simulation HIL (et comment changer les gains en fonction des cas). Enfin, même si nous avons fait de nombreuses erreurs souvent pas malignes, elles nous ont permis de bien mieux comprendre le fonctionnement du redresseur et lors d'erreurs ultérieurs (datant du mardi 17.11.26), alors qu'un de nos schémas (celui de la partie B) a été écrasé (nous avons sauvegardé en double le schéma de la partie C pour le HIL et viré celui de la partie B), nous avons pris un temps record de 1h pour refaire tout le schéma HIL (ce qui est un grand progrès par rapport aux 10 heures passés la première fois pour débuguer le HIL).
* **Note sur la partie 3.2 :** Suite à un incident de manipulation ayant entraîné l'écrasement de plusieurs fichiers de simulation qu'il a fallu reconstruire intégralement (aka le problème du 17.11.26 mentionné plus haut), **la sous-partie 3.2 (Court-circuit côté réseau) n'a malheureusement pas pu être finalisée** dans le temps imparti (Nous avons pu le tester sur notre ordinateur mais n'avons pas eu le temps de le mettre dans le rapport). Toutes les autres sections (simulation *offline*, études paramétriques, implémentation HIL et dissymétrie de tension) sont complètes et documentées.

## Contenu du dépôt
* `PI.ipynb` : **Rapport complet** (analyses théoriques, relevés et graphiques commentés).
* `*.plecs` : Modèles de simulation *offline* et fichiers temps réel *Hardware-in-the-Loop* (RT-Box & TI F2837x).
* `*.png` : Schémas d'architecture, détails des sous-systèmes de commande et spectres FFT.
Certaines photos des PLECS dans le rapport n'existent plus dans les PLECS finaux car c'était des modifications brèves. Cependant la démarche pour reproduire ces parties des fichiers a été bien entendu expliqué en détail dans le `Pi.ipynb`.

## Remerciements
Nous tenons à remercier M.Siemaszko et M.Sefaranga pour nous avoir aidé à débuguer et mieux comprendre certains résultats de ce labo.
