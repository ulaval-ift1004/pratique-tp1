# IFT-1004 - Pratique TP1

## Description

Ce dépôt contient des exercices pratiques de programmation destinés aux débutants. Il comprend des exemples de traduction entre pseudo-code et Python, ainsi que des exercices de correction d'erreurs pour apprendre les bases de la programmation.

## Contenu du dépôt

### 1. `1-traduction-pseudo-code-a-python.md`
- **15 exemples complets** de pseudo-code avec leurs équivalents Python
- Progression logique du simple au complexe
- Couverture des concepts fondamentaux :
  - Variables et affectation
  - Structures conditionnelles (si/sinon)
  - Boucles (pour tout, tant que)
  - Entrées/sorties utilisateur
  - Programmes pratiques (calculatrice, jeu de devinette, etc.)

### 2. `2-correction-de-bogues.md`
- **Exercice de correction d'erreurs** avec un programme Python défaillant
- **8 erreurs typiques** que font les débutants
- Solution détaillée avec explications
- Version améliorée du programme avec validation

## Objectifs pédagogiques

- Comprendre la correspondance entre pseudo-code et Python
- Identifier et corriger les erreurs de programmation courantes
- Maîtriser les structures de contrôle de base
- Développer de bonnes pratiques de programmation
- Apprendre à valider les entrées utilisateur

## Convention de pseudo-code utilisée

```
afficher()     →  print()
demander()     →  input()
<-             →  =
pour tout i dans <1,2,...,n> faire:  →  for i in range(1, n+1):
tant que condition faire:             →  while condition:
si condition alors:                   →  if condition:
sinon:                               →  else:
fin si/fin pour tout/fin tant que   →  indentation Python
```

## Comment utiliser ce dépôt

### Pour les étudiants :
1. **Commencez par** `1-traduction-pseudo-code-a-python.md`
2. **Étudiez** les exemples un par un
3. **Testez** les codes Python sur votre machine
4. **Passez à** `2-corriger-des-bogues.md`
5. **Tentez** de corriger les erreurs avant de regarder la solution

### Pour les enseignants :
- Utilisez les exemples comme support de cours
- Adaptez les exercices selon le niveau de vos étudiants
- Créez de nouveaux exercices en vous inspirant de la structure

## Erreurs courantes à éviter
- `print()` pas `Print()` (Python est sensible à la casse)
- `=` pour affecter, `==` pour comparer
- Ne pas oublier les `:` après `if`, `for`, `while`
- Respecter l'indentation (4 espaces recommandés)
- Convertir les entrées : `int(input())` ou `float(input())`
