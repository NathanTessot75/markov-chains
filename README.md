# Markov Explorer

**Visualisez et manipulez des chaînes de Markov en temps réel.**

Markov Explorer est un outil interactif pour explorer les chaînes de Markov à travers deux modes : un **bac à sable** libre pour construire et simuler n'importe quel graphe de transitions, et un **mode niveaux** avec des puzzles progressifs à résoudre.

---

## Modes

### Sandbox
Construisez librement votre chaîne de Markov :
- Ajoutez et déplacez des états sur un canvas SVG
- Définissez les probabilités de transition entre chaque paire d'états
- Lancez une simulation pas-à-pas ou en continu
- Visualisez la distribution stationnaire calculée en temps réel

### Mode Niveaux
Résolvez des puzzles basés sur la théorie des chaînes de Markov :

| # | Titre | Concept | Difficulté |
|---|-------|---------|------------|
| 1 | Tour du Monde | Cycle déterministe | Facile |
| 2 | Le Puits | État absorbant | Moyen |
| 3 | La Hiérarchie | Distribution stationnaire contrôlée | Difficile |
| 4 | Le Touriste | Temps de passage | Moyen |

Chaque niveau a un objectif précis (ex : "faites en sorte que l'état C soit absorbant") et vérifie automatiquement si la solution est valide.

---

## Fonctionnalités techniques

- **Canvas SVG interactif** — nœuds déplaçables, zoom, pan
- **Calcul de la distribution stationnaire** — résolution numérique de πP = π
- **Simulation animée** — visualisation du chemin parcouru état par état
- **Validation automatique** des objectifs de chaque niveau
- **Zéro dépendance externe** — tout en un seul fichier HTML (React via CDN, Tailwind via CDN)

---

## Utilisation

Aucune installation requise. Ouvrez simplement `index.html` dans un navigateur.

```bash
git clone https://github.com/NathanTessot75/markov-chains.git
cd markov-chains
open index.html
```

---

## Concepts couverts

- Chaînes de Markov à temps discret
- Matrices de transition stochastiques (lignes normalisées à 1)
- Distribution stationnaire (vecteur propre gauche pour λ=1)
- États absorbants, cycles, ergodicité

---

## Licence

© 2026 Nathan Tessot — Tous droits réservés.
