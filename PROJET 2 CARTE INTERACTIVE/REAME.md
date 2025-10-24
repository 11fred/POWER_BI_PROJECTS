# 🌍 Données démographiques et météo du monde

## 🧭 Introduction

L’objectif de ce projet est de concevoir une carte interactive permettant de visualiser et d’analyser les **données démographiques** et **météorologiques** des pays du monde.  
Ce tableau de bord Power BI offre une vue dynamique et intuitive des informations clés telles que la **population**, la **superficie**, la **température actuelle**, et la **vitesse du vent**, tout en permettant des comparaisons entre pays ou continents.

Le projet repose sur des données collectées à partir d’**API externes**, notamment :
- 🌐 [REST Countries API](https://restcountries.com/v3.1/all) – pour les données démographiques (population, langues, superficie, etc.)
- 🌦️ [Open Meteo API](https://open-meteo.com/) – pour les données météorologiques (température et vitesse du vent actuelles)

---

## ⚙️ Développement 

## PAGE 1 Suivi des ventes

![](/PROJET%202%20CARTE%20INTERACTIVE/Capture%20d’écran%202025-10-24%20174303.png)

### 🔹 Étape 1 : Nettoyage et préparation des données
Les données brutes issues des API ont été importées et **nettoyées dans Power Query**.  
Les principales opérations effectuées sont :
- Normalisation des colonnes (formatage des textes et des nombres)  
- Transformation et fusion de tables pour relier les pays à leurs données météo  
- Suppression des doublons et gestion des valeurs manquantes  

### 🔹 Étape 2 : Modélisation des données
Une **modélisation en étoile (star schema)** a été mise en place pour optimiser la performance du modèle Power BI :
- Une table **Faits** regroupant les mesures quantitatives (population, température, vitesse du vent, superficie)
- Des tables **Dimensions** pour les continents, les langues et les pays

### 🔹 Étape 3 : Création des mesures DAX
Des **mesures DAX** ont été créées pour calculer et agréger les valeurs selon différents filtres, par exemple :
- Moyenne de température par continent    

### 🔹 Étape 4 : Visualisation et interaction
Le tableau de bord intègre une **carte interactive** permettant de :
- Filtrer les données par **continent**, **langue**, **température** ou **mesure choisie**
- Visualiser instantanément les variations à travers les couleurs de la carte  
- Accéder à des **infobulles dynamiques** affichant pour chaque pays :
  - La population  
  - La langue principale  
  - La température actuelle  
  - La vitesse du vent  
  - La superficie  

Cette interactivité permet de comparer les pays entre eux sur plusieurs axes (démographique, géographique et climatique) à travers une expérience fluide et intuitive.

---

## 📊 Analyse du graphique principal

La **carte interactive** présente une vue géographique du monde avec des codes couleurs selon la mesure sélectionnée (ex : population ou température).  
- Les **pays les plus peuplés** ressortent avec une teinte plus intense, facilitant l’identification des zones de forte densité.  
- Lors du filtrage par **continent**, on peut observer les différences de températures moyennes ou de population d’une région à l’autre.  
- Le **curseur de température** permet d’exclure certains pays selon la plage thermique choisie.  

Ainsi, la carte combine à la fois **données démographiques** et **météo en temps réel**, offrant une vision globale et analytique du monde.

---

## 🧠 Compétences acquises

Au cours de ce projet, plusieurs compétences techniques et analytiques ont été mobilisées et renforcées :

- 🔹 **Nettoyage et transformation des données** avec *Power Query*  
- 🔹 **Requête et intégration d’API REST** (REST Countries et Open Meteo)  
- 🔹 **Modélisation des données en étoile**  
- 🔹 **Création de mesures avec DAX**  
- 🔹 **Conception de cartes et de visualisations interactives** dans Power BI  
- 🔹 **Création d’infobulles dynamiques** pour enrichir l’expérience utilisateur  
- 🔹 **Mise en place de filtres dynamiques** (par continent, langue, température, etc.)  

---

## 🧩 Conclusion

Ce projet démontre la puissance de Power BI dans la **fusion de données hétérogènes** issues de différentes sources (API, fichiers CSV,

