# Environment setup

- pip install qsharp (éventuellement dans un environnement virtuel)
- dotnet tool install -g Microsoft.Quantum.IQSharp
- dotnet iqsharp install

# Estimation de phase quantique

## Introduction

L'algorithme d'estimation de phase quantique est un outil essentiel dans le domaine de l'informatique quantique. Il permet de déterminer avec une grande précision la phase associée à un opérateur unitaire, ce qui est crucial pour de nombreuses applications, notamment en calcul quantique et en simulation quantique.

## Importance de l'algorithme

L'estimation de phase quantique est fondamentale pour plusieurs raisons :

1. **Algorithmes Quantiques Avancés** : De nombreux algorithmes quantiques avancés, tels que l'algorithme de Shor pour la factorisation d'entiers et l'algorithme de Grover pour la recherche quantique, dépendent de l'estimation précise de phase.

2. **Optimisation Quantique** : L'estimation de phase est utilisée dans des problèmes d'optimisation quantique où la précision de la phase est critique pour trouver des solutions efficaces.

3. **Simulation Quantique** : Dans le domaine de la simulation quantique, l'estimation de phase permet d'obtenir des résultats précis pour simuler le comportement de systèmes quantiques complexes.

## Contenu du Projet

Le projet se compose de deux fichiers principaux :

1. **BasicPhaseEstimation.qs** : Ce fichier contient l'implémentation de l'algorithme d'estimation de phase quantique. Il définit les opérations nécessaires à l'estimation de phase.

2. **rendu.ipynb** : Ce fichier est un notebook Jupyter contenant un script Python qui importe l'algorithme de BasicPhaseEstimation.qs. Il effectue des simulations pour étudier la précision de l'estimation de phase et analyse les résultats.

## Utilisation

### Fichier Q# - BasicPhaseEstimation.qs

- `U(phi, psi)`: Une opération unitaire qui applique une rotation contrôlée sur les qubits de l'état donné.
- `basicPhaseEstimation(n, theta, oracle, psi)`: L'opération principale qui effectue l'estimation de phase en utilisant un oracle spécifié.
- `run(nShots, phi, oraclePower)`: L'opération d'entrée qui exécute l'algorithme pour un nombre spécifié de tirs, une phase donnée et une puissance d'oracle.

### Notebook Jupyter - rendu.ipynb

Le notebook **rendu.ipynb** utilise l'algorithme implémenté dans **BasicPhaseEstimation.qs** pour effectuer des simulations et analyser la précision de l'estimation de phase. Il offre un environnement interactif pour explorer les résultats et comprendre les performances de l'algorithme dans divers scénarios.


