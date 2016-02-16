# Vision

  - avoir un langague facile à écrire (de type markdown)
  - possibilité d'incorporer des éléments:
    - de structure (relations)
    - de logique (sémantique)

## Stratégie

  - Obtenir un graphe
    - markdown <-> arbre
    - Quel types de graphes permet-on?

  - ajout de propriété aux noeuds en utilisant un minimum de symboles
  - Utiliser à fond la logique

... on devrait pouvoir décrire pas mal de choses avec ça

# Éléments de logique

## Assertions

Exemple: *Mon programme est un code écrit en fortran*

```
#monProgramme
  .code
    lang: fortran
```

ou pour simplifier au maximum l'indentation

```
#monProgramme.code
  lang: fortran
```

ou

```
#monProgramme
.code
  lang: fortran
```

ou

```
#monProgramme.code.lang: fortran
```

## Assertion implicite

Exemple: Le document décrit un object HTML

```
@html

.head
  lang: fr
  charset: utf-8
.body
  h1: "Mon Titre"
  p: "Ceci est un exemple"
```
