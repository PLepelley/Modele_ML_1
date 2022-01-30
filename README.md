# Modele_ML_1
 Premier modèle de machine learning (régression linéaire)

## Plan
1. Rappel de la régression linéaire, multiple et polynomiale
2. Explication des fonctions
3. Présentation des résultats sous forme de graphiques
4. Evaluation des modèles
5. Présentation des résultats avec Scikit-Learn
6. Comparaison avec la méthode normale
7. Conclusion

---------------

1. Régressions
> Une régression est un modèle qui cherche à établir une relation entre une variable "expliquée" (y) et une ou plusieurs variables "explicatives" (x1, x2...)  

    - Régression linéaire  
Pour une régression linéaire, on chercher à trouver y à partir d'une seule variable x (ou feature), sous forme d'équation :   
`y = ax + b`   
    - Régression multiple
On chercher à expliquer y à partir de plusieurs variables (ou features) :    
`y = ax1 + bx2 + cx3 + d`  
    - Régression polynomiale  
`y = ax^2 + bx + c`   

2. Les fonctions
    - Modèle  
 `F = X . Theta`     
 où X est une matrice de m lignes et n colonne(s) représentant l'ensemble des observations du/des features x et 1 colonne de valeur 1
 et Theta est une matrice à n lignes et 1 colonne correspondant aux paramètres a et b (en prenant l'exemple d'une équation linéaire d'équation y = ax + b)  
La fonction permet de trouver de nouvelles valeurs de y (appelé y prédits) à partir de nouvelles observations (x).

    - Fonction de coût  
`J = 1/2m . sum((X.Theta - Y)^2)`  
La fonction de coût représente la somme des différences entre y prédits (X.Theta) et y observés (Y) mis au carré, divisé par le nombre d'observation. Il s'agit donc d'une moyenne, appelé aussi erreur quadratique moyenne  

    - Gradient  
 `G = 1/m . X(transposé)(X.Theta - Y)`  
 Le gradient correspond à la dérivée de la fonction de coût, aussi appelé la pente.  
 
    - Descente de gradient  
`Theta = Theta - alpha . G`  
La descente de gradient permet de trouver les paramètres a et b (dans le cadre d'une régression linéaire) pour que la fonction de coût soit la plus proche de 0.  

    - Coefficient de détermination  
`r2 = sum(Y - X.Theta)^2 / sum(Y - moyenne(Y))^2`  
Le coefficient de détermination permet d'évaluer un modèle

3. Représentation des résultats
    - Régression linéaire  
[Regression lineaire](reg_lineaire.png)
    - Régression multiple  
[Regression multiple]() 
    - Régression polynomiale  
[Regression polynomiale]()

4. Evaluation des modèles
    - Régression linéaire  
Mean Squared Error = 9.9307  
R2 = 0.9732  
    - Régression multiple  
Mean Squared Error = 26.9088  
R2 = 0.3624  
    - Régression polynomiale  
Mean Squared Error = 7766436069.9260  
R2 = 0.8074  

6. Comparaison des modèles avec Scikit Learn
    - Régression linéaire  
L'erreur quadratique à la moyenne est de 9.888 pour le modèle manuel et de 8.752 pour le modèle de SK-Learn.  
    - Régression multiple  
L'erreur quadratique à la moyenne est de 53.818 pour le modèle manuel et de 48.466 pour le modèle de SK-Learn.    
    - Régression polynomiale  
L'erreur quadratique à la moyenne est de 7766436069.926 pour le modèle manuel et de 4400142334.915 pour le modèle de SK-Learn.  

7. Conclusion
Ce projet m'a permis d'apprendre à créer manuellement un modèle de machine learning et de comprendre le fonctionnement du calcul matriciel. 
