# CLAUDE.md

## Le dépôt

Roadmap produit publique de DigitalCrew. Le dépôt ne contient qu'un `README.md` :
pas de code, pas de `package.json`, pas de dépendances, pas de CI (`.github/` absent).
Les éléments de roadmap sont des issues GitHub ; le tableau de référence est le
projet d'organisation lié en tête du README.

## Commandes

Aucune : pas d'installation, de lint, de typecheck, de tests ni de build.
Avant de pousser, relire le rendu Markdown (tableaux, liens) et vérifier le diff.

## Règles

- Contenu public : n'y mettre ni information interne (le *pourquoi* et le *comment*
  se discutent dans Discussions et les RFC, comme le dit le README), ni secret, ni nom
  d'hôte interne, ni donnée personnelle, ni date ou engagement de livraison ferme.
- Le README commence par `<!-- last-reviewed: AAAA-MM-JJ -->` : mettre à jour cette
  date quand le contenu est resynchronisé.
- Garder les libellés cohérents entre les sections : phases (le README les écrit avec
  emoji : `🔭 exploring`, `🎨 in design`, `🔬 preview`, `✅ ga`, `🚢 shipped`),
  `area: …`, `worker: …`. Ces libellés doivent correspondre aux labels réels des
  issues ; ne pas en inventer.
- Les listes de workers ne sont pas alignées aujourd'hui (introduction, `area: agents`
  et tableau « Digital Workers » citent des ensembles différents) : corriger toutes
  les occurrences ensemble si on touche à cette liste. Même chose pour la colonne
  appelée « Exploring » puis « Exploratory » selon la section.
- Garder la section « Forward-looking statement ».

## Flux Git

- Branche par défaut : `main`. Il existe aussi `develop` (identique à `main` à ce jour).
- Branche de travail : `claude/<clé-de-la-carte>-<mot-clé>`.
- PR vers `main` avec relecture humaine.
- Jamais de push sur `main` ou `develop`, jamais de merge, jamais de force-push.
