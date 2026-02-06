# Exemples de pseudo-codes et codes équivalents en Python pour pratiquer

## 1. Affichage et saisie de base

### Pseudo-code

```
afficher("Bonjour le monde !")
nom <- demander("Quel est votre nom ? ")
afficher("Salut", nom)
```

---

## 2. Variables et calculs simples

### Pseudo-code

```
a <- 5
b <- 10
somme <- a + b
afficher("La somme est :", somme)
```

---

## 3. Calculatrice simple

### Pseudo-code

```
nombre1 <- demander("Premier nombre : ")
nombre2 <- demander("Deuxième nombre : ")

resultat <- nombre1 + nombre2

afficher("Résultat :", resultat)
```

---

## 4. Condition simple

### Pseudo-code

```
age <- demander("Votre âge : ")

si age >= 18 alors:
    afficher("Vous êtes majeur")
sinon:
    afficher("Vous êtes mineur")
fin si
```

---

## 5. Conditions multiples

### Pseudo-code

```
note <- demander("Votre note sur 20 : ")

si note >= 16 alors:
    afficher("Très bien")
sinon:
    si note >= 14 alors:
        afficher("Bien")
    sinon:
        si note >= 12 alors:
            afficher("Assez bien")
        sinon:
            si note >= 10 alors:
                afficher("Passable")
            sinon:
                afficher("Insuffisant")
            fin si
        fin si
    fin si
fin si
```

---

## 6. Boucle pour simple

### Pseudo-code

```
pour tout i dans <1,2,3,4,5> faire:
    afficher("Nombre :", i)
fin pour tout
```

---

## 7. Table de multiplication

### Pseudo-code

```
nombre <- demander("Table de multiplication de : ")

pour tout i dans <1,2,...,10> faire:
    resultat <- nombre * i
    afficher(nombre, "x", i, "=", resultat)
fin pour tout
```

---

## 8. Boucle tant que simple

### Pseudo-code

```
compteur <- 1

tant que compteur <= 5 faire:
    afficher("Compteur :", compteur)
    compteur <- compteur + 1
fin tant que
```

---

## 9. Jeu de devinette

### Pseudo-code

```
nombre_secret <- 7
tentative <- 0

tant que tentative != nombre_secret faire:
    tentative <- demander("Devinez le nombre : ")
    si tentative > nombre_secret alors:
        afficher("Trop grand !")
    sinon:
        si tentative < nombre_secret alors:
            afficher("Trop petit !")
        fin si
    fin si
fin tant que

afficher("Bravo ! Vous avez trouvé !")
```

---

## 10. Calcul de moyenne

### Pseudo-code

```
somme <- 0

pour tout i dans <1,2,3,4,5> faire:
    note <- demander("Note " + i + " : ")
    somme <- somme + note
fin pour tout

moyenne <- somme / 5
afficher("Moyenne :", moyenne)
```

---

## 11. Compter les nombres pairs

### Pseudo-code
```
compteur_pairs <- 0

pour tout i dans <1,2,...,10> faire:
    si i % 2 == 0 alors:
        afficher(i, "est pair")
        compteur_pairs <- compteur_pairs + 1
    fin si
fin pour tout

afficher("Total de nombres pairs :", compteur_pairs)
```

---

## 12. Menu avec choix

### Pseudo-code
```
afficher("=== MENU ===")
afficher("1. Addition")
afficher("2. Soustraction")
afficher("3. Multiplication")
choix <- demander("Votre choix : ")

si choix == 1 alors:
    a <- demander("Premier nombre : ")
    b <- demander("Deuxième nombre : ")
    afficher("Résultat :", a + b)
sinon:
    si choix == 2 alors:
        a <- demander("Premier nombre : ")
        b <- demander("Deuxième nombre : ")
        afficher("Résultat :", a - b)
    sinon:
        si choix == 3 alors:
            a <- demander("Premier nombre : ")
            b <- demander("Deuxième nombre : ")
            afficher("Résultat :", a * b)
        sinon:
            afficher("Choix invalide")
        fin si
    fin si
fin si
```

---

## 13. Trouver le maximum

### Pseudo-code

```
maximum <- 0
pour tout i dans <1,2,3,4,5> faire:
    nombre <- demander("Entrez un nombre : ")
    si nombre > maximum alors:
        maximum <- nombre
    fin si
fin pour tout
afficher("Le maximum est :", maximum)
```

---

## 14. Validation d'entrée

### Pseudo-code
```
age <- 0
tant que age < 1 ou age > 120 faire:
    age <- demander("Votre âge (1-120) : ")
    si age < 1 ou age > 120 alors:
        afficher("Âge invalide, réessayez !")
    fin si
fin tant que
afficher("Votre âge est :", age)
```

---

## 15. Somme des nombres de 1 à N (repratiquer, nous avons déjà vu cela en classe)

### Pseudo-code
```
n <- demander("Calculer la somme de 1 à : ")
somme <- 0
pour tout i dans <1,2,...,n> faire:
    somme <- somme + i
fin pour tout
afficher("La somme de 1 à", n, "est :", somme)
```

---

1. **Indentation** : En Python, l'indentation remplace les mots "fin si", "fin pour tout", etc.
2. **Types de données** : `input()` retourne toujours une chaîne, utiliser `int()` ou `float()` si nécessaire
3. **range()** : Pour les boucles, `range(1, 6)` génère 1,2,3,4,5 (le dernier nombre est exclu)