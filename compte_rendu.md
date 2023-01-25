# Mise en place 

## Récupération des données (24/01 et 25/01)

Nous avons récupéré les données d'un jeu avec le fichiers localDataManager.py 
Nous l'appelons dans le main pour traité les données dans la classe Mem. 
Cette classe est un singleton avec la variable instance qui permet d'instancier la classe si c'est le premier appel de la classe sinon on garde le même objet Mem(). 

création de fillMemory, rempli la mémoire avec le contenu du jeu en bit. 

---

## Récupération des instructions et mise en fonction (25/01)

Nous avons créer une boucle (loop) afin de récupérer dans la mémoire les bits(par paquet de 8) afin de convertir chaque octet en
en hexadécimal. Puisque 1 octet correspond à un hexadécimal à 2 "membres", il nous faut donc coller 2 à 2 les octets pour récuprer le code Hexadécimal (4 membres).
Implémentation du CPu en classe CPU (singleton comme la Mem), fonction de classe (decode) récupère l'instruction en Hexa et identifie chaque terme des 4 membres de l'instruction (en hexa) pour affecter l'instruction à la bonne instruction(qui renverra à une fonction python).

---

## A faire
régler decode()
mapping des instruction hexa
def des fonctions pour chaque 'fonction' hexa
