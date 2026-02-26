# Projet-R

# Simulation du Modèle de Bhaduri-Marglin sous R

## Présentation du Projet

Ce projet consiste en une modélisation macroéconomique du modèle de Bhaduri-Marglin.
L'objectif est d'analyser l'équilibre du revenu (Y) en fonction du partage de la valeur ajoutée entre salaires et profits (part salariale w).
Le projet explore deux méthodes de résolution :
**Méthode Analytique** : Résolution directe de l'équation algébrique.
**Méthode Itérative** : Simulation des ajustements successifs des variables endogènes jusqu'à convergence.

# Fonctionnalités de l'OutilCalcul de l'équilibre (Y) :

Utilisation de paramètres exogènes tels que la **consommation autonome (c0)**, l'**investissement autonome (i0)** et les **dépenses publiques (G)**.

**Simulation de scénarios** : Analyse de la sensibilité du revenu à la part salariale w sur une plage de 0.40 à 0.80.

**Identification du régime économique** : Détermination automatique de la nature du régime: 
- Wage-led ==>  L'activité est tirée par les salaires Delta > 0.
- Profit-led ==> L'activité est tirée par les profits (Delta < 0).

**Analyse de stabilité** : Vérification que le dénominateur de la fonction d'équilibre est différent de zéro pour garantir la validité du modèle.

# Stack TechniqueLangage: 

**R Framework**  : Quarto Librairies utilisées :dplyr : Pour la manipulation de données (mutate, case_when)
**tidyr** : Pour la création de grilles de paramètres (crossing).

## Utilisation 
Le script principal permet de générer un tableau de résultats (grid) testant 27 combinaisons de paramètres comportementaux (cw, cp, i_pi)
