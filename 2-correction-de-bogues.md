# Exercice de correction d'erreurs - Python

## Code avec erreurs à corriger

Voici un programme qui devrait calculer la moyenne de 5 notes et afficher une appréciation, mais il contient **8 erreurs**. Trouvez-les et corrigez-les !

```python
# Programme pour calculer la moyenne de notes
Print("=== Calculateur de moyenne ===")

# Demander le nom de l'étudiant
nom = input("Nom de l'étudiant : ")

# Initialiser les variables
somme = 0
nb_notes == 5

# Saisir les notes
for i in range(1, nb_notes):
    note = input(f"Note {i} sur 20 : ")
    somme = somme + note

# Calculer la moyenne
moyenne = somme / nb_notes
print("Bonjour", nom, "votre moyenne est :", moyenne)

# Afficher l'appréciation
if moyenne >= 16
    print("Excellent !")
elif moyenne >= 14:
    print("Très bien")
elif moyenne >= 12:
    print("Bien")
elseif moyenne >= 10
    print("Passable")
else:
    print("Insuffisant")

# Vérifier si l'étudiant passe
si moyenne >= 10:
    print("Vous validez l'examen !")
sinon:
    print("Vous devez repasser l'examen.")
```

---

## Instructions pour les étudiants

1. **Lisez attentivement** le code ci-dessus
2. **Identifiez les 10 erreurs** (syntaxe, logique, types, etc.)
3. **Corrigez chaque erreur** une par une
4. **Testez votre code** pour vérifier qu'il fonctionne correctement

### Types d'erreurs à chercher :
- Erreurs de syntaxe (majuscules/minuscules, deux-points manquants, etc.)
- Erreurs de logique (boucles, conditions)
- Erreurs de types (conversion de données)
- Erreurs de notation (opérateurs)
- Mélange pseudo-code/Python

---

## Solution corrigée

```python
# Programme pour calculer la moyenne de notes
print("=== Calculateur de moyenne ===")  # Erreur 1: Print -> print

# Demander le nom de l'étudiant
nom = input("Nom de l'étudiant : ")

# Initialiser les variables
somme = 0
nb_notes = 5  # Erreur 2: == -> =

# Saisir les notes
for i in range(1, nb_notes + 1):  # Erreur 3: range(1, nb_notes) -> range(1, nb_notes + 1)
    note = float(input(f"Note {i} sur 20 : "))  # Erreur 4: input() donne une chaîne, il faut convertir
    somme = somme + note

# Calculer la moyenne
moyenne = somme / nb_notes
print("Bonjour", nom, "votre moyenne est :", moyenne)

# Afficher l'appréciation
if moyenne >= 16:  # Erreur 5: deux points ":" manquant
    print("Excellent !")
elif moyenne >= 14:
    print("Très bien")
elif moyenne >= 12:
    print("Bien")
elif moyenne >= 10:  # Erreur 6: elseif -> elif
    print("Passable")
else:
    print("Insuffisant")

# Vérifier si l'étudiant passe
if moyenne >= 10:  # Erreur 7: si -> if
    print("Vous validez l'examen !")
else:  # Erreur 8: sinon -> else
    print("Vous devez repasser l'examen.")
```

---

## Liste des erreurs corrigées

1. **Ligne 2** : `Print` → `print` (Python est sensible à la casse)
2. **Ligne 8** : `nb_notes == 5` → `nb_notes = 5` (affectation vs comparaison)
3. **Ligne 11** : `range(1, nb_notes)` → `range(1, nb_notes + 1)` (pour avoir 5 notes, pas 4)
4. **Ligne 12** : `note = input(...)` → `note = float(input(...))` (conversion en nombre)
5. **Ligne 18** : `if moyenne >= 16` → `if moyenne >= 16:` (deux-points manquant)
6. **Ligne 24** : `elseif moyenne >= 10` → `elif moyenne >= 10:` (elif et non elseif)
7. **Ligne 29** : `si moyenne >= 10:` → `if moyenne >= 10:` (mélange pseudo-code/Python)
8. **Ligne 31** : `sinon:` → `else:` (mélange pseudo-code/Python)

**Erreurs bonus** (si on compte plus finement) :
- Le programme ne gère pas les notes invalides (< 0 ou > 20)
- Pas de vérification si l'utilisateur entre du texte au lieu d'un nombre (c'est correct de ne pas gérer ceci à ce stade de notre apprentissage. Cela n'est pas également demandé dans le TP1)

Dans l'énoncé du TP1, c'est indiqué :

>{note} **Important :** À chacune des entrées utilisateur, vous pouvez supposer que l'utilisateur
entrera une chaîne valide. En d'autres termes, si on demande par exemple la taille du losange
et qu'on entre la chaîne "salut", il est tout à fait normal que votre programme plante ou
agisse de manière imprévisible

---

## Exercice supplémentaire

Maintenant que vous avez corrigé le code, ajoutez ces améliorations :

1. **Validation des notes** : Vérifiez que chaque note est entre 0 et 20
3. **Affichage amélioré** : Arrondissez la moyenne à 2 décimales

### Code amélioré (optionnel)

```python
# Programme pour calculer la moyenne de notes (version améliorée)
print("=== Calculateur de moyenne ===")

# Demander le nom de l'étudiant
nom = input("Nom de l'étudiant : ")

# Initialiser les variables
somme = 0
nb_notes = 5

# Saisir les notes avec validation
for i in range(1, nb_notes + 1):
    note_valide = False
    while not note_valide:
        note = float(input(f"Note {i} sur 20 : "))
        if 0 <= note <= 20:
            note_valide = True
        else:
            print("La note doit être entre 0 et 20 !")
    
    somme = somme + note

# Calculer la moyenne
moyenne = somme / nb_notes
print(f"Bonjour {nom}, votre moyenne est : {moyenne:.2f}")

# Afficher l'appréciation
if moyenne >= 16:
    print("Excellent !")
elif moyenne >= 14:
    print("Très bien")
elif moyenne >= 12:
    print("Bien")
elif moyenne >= 10:
    print("Passable")
else:
    print("Insuffisant")

# Vérifier si l'étudiant passe
if moyenne >= 10:
    print("Vous validez l'examen !")
else:
    print("Vous devez repasser l'examen.")
```
