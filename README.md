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
> Une régression linéaire est un modèle qui cherche à établir une relation entre une variable "expliquée" (y) et une ou plusieurs variables "explicatives" (x1, x2...)  

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
 où X est une matrice à m lignes et n colonne(s) représentant l'ensemble des observations du feature x
 et Theta est une matrice à une ligne et 2 colonnes correspondant aux paramètres a et b (de l'équation y = ax + b)  
 
    - Fonction de coût  
  
    - Gradient
    - Descente de gradient
