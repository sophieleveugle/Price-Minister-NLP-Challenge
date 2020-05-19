# Price-Minister-NLP-Challenge
Evaluer si un avis utilisateur sur un produit peut être utile pour d’autres utilisateurs

## Contexte du challenge

PriceMinister permet à ses utilisateurs de partager leur avis sur les produits qu’ils ont achetés. Avec plus d’un million d’avis, ce jeu de données a un énorme potentiel pour améliorer la qualité du site et permettre aux utilisateurs de trouver leur produit qui leur convient le mieux. Chaque utilisateur peut aussi évaluer un avis, en spécifiant si il est utile pour lui ou non. Ce retour est aussi très important pour la qualité des services. Ce jeu de données est original car il contient des avis sur des contenus textuels et non pas sur les produits eux même. Prédire le retour des utilisateurs sur les avis eux même, est particulièrement ambitieux, et peut avoir des implications plus général que le e-commerce.

## Objectifs du challenge

Le but est d’évaluer si un avis utilisateur sur un produit peut être utile pour d’autres utilisateurs. Certains avis sont ainsi particulièrement intéressants.
Chaque avis est labélisé comme useful (class 1) ou not useful (class 0), en se basant sur leur nombre de retours useful si (nombre de retours positifs / total du nombre de retours) > 0.5 not useful si (nombre de retours positifs / total du nombre de retours) < 0.5

Nous avons enlevé les avis pour lesquels le nombre de retour positifs et le nombre de retours négatifs étaient égaux. Nous utiliserons la mesure AUC (Area Under the Curve) pour l’évaluation, et vous devrez fournir la probabilité d’être utile (class 1) pour chaque avis du jeu de données de test. 
