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

## Exercice supplémentaire

Maintenant que vous avez corrigé le code, ajoutez ces améliorations :

1. **Validation des notes** : Vérifiez que chaque note est entre 0 et 20
3. **Affichage amélioré** : Arrondissez la moyenne à 2 décimales
