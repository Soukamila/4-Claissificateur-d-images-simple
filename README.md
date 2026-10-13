# 4-Claissificateur-d-images-simple


## Objectif

Entraîner un modèle d'intelligence artificielle capable de reconnaître en direct 3 objets 
différents grâce à la webcam : un stylo, un téléphone et une main vide.

## Expliquez en 3-4 phrases ce qui s’est passé pendant l’entraînement (en lien avec le Module 11 du cours). 

Pendant l’entraînement, le modèle a analysé les photos que j’ai prises pour chaque classe (stylo, téléphone, main vide) afin de repérer les caractéristiques visuelles qui les distinguent : formes, couleurs, contours. À chaque passage sur les données (appelé « epoch »), il a ajusté ses paramètres internes, les « poids », pour réduire l’écart entre sa prédiction et la bonne étiquette. C'est de l'apprentissage supervisé : le modèle apprend à partir d'exemples étiquetés, sans règles écrites à la main.


## Composants

- **Ordinateur avec navigateur** : exécute Teachable Machine, sans installation.
- **Webcam** : capture les images d'entraînement et le test en direct.
- **Google Teachable Machine** : outil qui entraîne le modèle directement dans le navigateur.
- **3 classes** (`stylo`, `telephone`, `main vide`) : les catégories que le modèle doit distinguer.
- **Objets réels** (un stylo et un téléphone) : servent à créer les données d'entraînement.

## Fonctionnement

1. **Collecte des données** : création de 3 classes et enregistrement de [30 ou plus] photos par classe avec la webcam, en variant les angles, les distances et la position de l'objet.
2. **Entraînement** : clic sur *Train Model*. Le modèle apprend à associer chaque image à sa classe en ajustant ses paramètres sur plusieurs passages.
3. **Test en direct** : chaque objet est présenté devant la webcam. Le modèle affiche un pourcentage de confiance pour chaque classe, et la plus haute est sa prédiction.

## Résultats obtenus

- Stylo présenté : reconnu comme `stylo` avec [ex. 98 %] de confiance.
- Téléphone présenté : reconnu comme `telephone` avec [ex. 96 %] de confiance.
- Main vide présentée : reconnue comme `main vide` avec [ex. 99 %] de confiance.
- Nombre de photos par classe : [30 ou plus].
- Cas où le modèle s'est trompé : [ex. objet trop loin ou mal éclairé, ou « aucun »].
