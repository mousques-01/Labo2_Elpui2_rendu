# Laboratoire 2 — Redresseur Actif Triphasé (AFE) & Simulation HIL

Ce dépôt contient l'ensemble des fichiers de simulation PLECS, des schémas temps réel (RT-Box / TI ControlCARD) ainsi que l'analyse complète réalisée dans le cadre du **Laboratoire 2 d'Électronique de Puissance II**.

## Où trouver le rapport ?
* **Le rapport principal attendu est le fichier [`PI.ipynb`](./PI.ipynb).**
* Vous pouvez le consulter directement dans votre navigateur en cliquant sur le fichier ci-dessus : l'ensemble des graphiques, tableaux comparatifs, schémas et interprétations y sont déjà intégrés et affichés.

## Objectif et public visé
Ce rapport a été rédigé de manière détaillée et pédagogique afin d'être accessible à **tout lecteur souhaitant comprendre en profondeur le fonctionnement, le dimensionnement et le comportement d'un redresseur actif triphasé (Active Front-End)** — depuis la modélisation et le réglage des boucles de régulation en cascade jusqu'à l'implémentation matérielle *Hardware-in-the-Loop* (HIL).

## Retour d'expérience & état d'avancement
* **Investissement :** La réalisation complète de ce laboratoire (modélisation, débogage des boucles, tests paramétriques, mise en œuvre sur banc temps réel et rédaction) a représenté environ **40 heures de travail**, marquées par de nombreux défis techniques et problèmes de synchronisation/configuration résolus au fil des essais.
* **Note sur la partie 3.2 :** Suite à un incident de manipulation ayant entraîné l'écrasement de plusieurs fichiers de simulation qu'il a fallu reconstruire intégralement, **la sous-partie 3.2 (Court-circuit côté réseau) n'a malheureusement pas pu être finalisée** dans le temps imparti. Toutes les autres sections (simulation *offline*, études paramétriques, implémentation HIL et dissymétrie de tension) sont complètes et documentées.

## Contenu du dépôt
* `PI.ipynb` : **Rapport complet** (analyses théoriques, relevés et graphiques commentés).
* `*.plecs` : Modèles de simulation *offline* et fichiers temps réel *Hardware-in-the-Loop* (RT-Box & TI F2837x).
* `*.png` : Schémas d'architecture, détails des sous-systèmes de commande et spectres FFT.
