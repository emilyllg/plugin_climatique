# plugin_climatique

Existant : 
- Icetool plugin pour calculer les températures de surface : https://github.com/Art-Ev/ICEtool/tree/main
avantage : interface accessible, calculs précis
inconvénients : beaucoup de données à fournir en entrée, besoin de se connecter a leur base de données sql pour les requêtes.
- outil collaboratif diaclimap : https://www.cerema.fr/system/files/documents/2017/11/projet_diaclimap_cle1a3fca.pdf
- services web de localisation de risques ( inondations, vagues de chaleur) : https://georisques.gouv.fr/

sources de données : 

ILOTS DE CHALEUR
- Geojson à télécharger en local ilôts de chaleurs : https://data.iledefrance.fr/explore/dataset/ilots-de-chaleur-urbains-icu-classification-des-imu-en-zone-climatique-locale-lc/export/?dataChart=eyJxdWVyaWVzIjpbeyJjb25maWciOnsiZGF0YXNldCI6Imlsb3RzLWRlLWNoYWxldXItdXJiYWlucy1pY3UtY2xhc3NpZmljYXRpb24tZGVzLWltdS1lbi16b25lLWNsaW1hdGlxdWUtbG9jYWxlLWxjIiwib3B0aW9ucyI6e319LCJjaGFydHMiOlt7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQVZHIiwieUF4aXMiOiJvYmplY3RpZCIsInNjaWVudGlmaWNEaXNwbGF5Ijp0cnVlLCJjb2xvciI6IiNlNzRjM2MifV0sInhBeGlzIjoib2JqZWN0aWQiLCJtYXhwb2ludHMiOjUwLCJzb3J0IjoiIn1dLCJ0aW1lc2NhbGUiOiIiLCJkaXNwbGF5TGVnZW5kIjp0cnVlLCJhbGlnbk1vbnRoIjp0cnVlfQ%3D%3D&location=9,48.68404,2.50266&basemap=jawg.sunny
- arcgis open data : https://data-iau-idf.opendata.arcgis.com/datasets/2846134ea6b94177af1366d11e517187_96/explore?location=48.827829%2C2.615816%2C12.66&showTable=true
- liste indicateurs : https://www.institutparisregion.fr/fileadmin/DataStorage/IauEtVous/CartesEtDonnees/cartesetdonnees/opendata/MetaPDF/ICU_LCZ_Alea_Vuln_Champs_2022.pdf

- attributs couche ilot :https://www.institutparisregion.fr/fileadmin/DataStorage/IauEtVous/CartesEtDonnees/cartesetdonnees/opendata/MetaPDF/LCZ_ICU2022.pdf
- avec note de vulnerabilité de jour et nuit aux vagues de chaleurs basée sur somme des autres aléas des IMU : vulj/vuln

- vulnerabilitemax5 : where ( vuln and vulj)>5.



VEGETATION 
- Déjà pris en compte pour ilôt de chaleur mais voir si ajouter une couche de visualisation seule des espaces verts et de leurs apports ( ilôts de fraicheur).
 
INONDATION alearg : 
depuis source data brgm 
- REMNAPPE_FR : carte nationale des remontée de nappes
- MASQ_EAIP : enveloppe approchée des inondations potentielles cours d'eau et surbmersion marine de plus d'un hectare
depuis https://georisques.gouv.fr/services :
- ALEA_synth_01 : Surface inondable - Aléa débordement de cours d'eau fréquent ou décennal - France métropolitaine - Rapportage 2020
- meme chose "avec prise en compte du changement climatique"; "moyen ou decennal"; "rare ou millenal";
- Surface inondable - Aléa ruissellement fréquent ou décennal - France métropolitaine - Rapportage 2020
- Surface inondable - Aléa submersion moyen ou centennal - France métropolitaine - Rapportage 2020
- Hauteurs d'eau - Aléa débordement de cours d'eau rare ou millénial - France métropolitaine - Rapportage 2020
- Zones soustraites à l'aléa inondation - France métropolitaine - Rapportage 2020
- Zones de sur-aléa inondation - France métropolitaine -raportage 2020

  METADATA DES COUCHES

