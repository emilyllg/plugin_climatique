# plugin_climatique

Existant : 
- Icetool plugin pour calculer les températures de surface : https://github.com/Art-Ev/ICEtool/tree/main
avantage : interface accessible, calculs précis
inconvénients : beaucoup de données à fournir en entrée, besoin de se connecter a leur base de données sql pour les requêtes.
- services web de localisation de risques ( inondations, vagues de chaleur)

sources de données : 

ILOTS DE CHALEUR
- Geojson à télécharger en local ilôts de chaleurs : https://data.iledefrance.fr/explore/dataset/ilots-de-chaleur-urbains-icu-classification-des-imu-en-zone-climatique-locale-lc/export/?dataChart=eyJxdWVyaWVzIjpbeyJjb25maWciOnsiZGF0YXNldCI6Imlsb3RzLWRlLWNoYWxldXItdXJiYWlucy1pY3UtY2xhc3NpZmljYXRpb24tZGVzLWltdS1lbi16b25lLWNsaW1hdGlxdWUtbG9jYWxlLWxjIiwib3B0aW9ucyI6e319LCJjaGFydHMiOlt7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQVZHIiwieUF4aXMiOiJvYmplY3RpZCIsInNjaWVudGlmaWNEaXNwbGF5Ijp0cnVlLCJjb2xvciI6IiNlNzRjM2MifV0sInhBeGlzIjoib2JqZWN0aWQiLCJtYXhwb2ludHMiOjUwLCJzb3J0IjoiIn1dLCJ0aW1lc2NhbGUiOiIiLCJkaXNwbGF5TGVnZW5kIjp0cnVlLCJhbGlnbk1vbnRoIjp0cnVlfQ%3D%3D&location=9,48.68404,2.50266&basemap=jawg.sunny
- arcgis open data : https://data-iau-idf.opendata.arcgis.com/datasets/2846134ea6b94177af1366d11e517187_96/explore?location=48.827829%2C2.615816%2C12.66&showTable=true
- liste indicateurs : https://www.institutparisregion.fr/fileadmin/DataStorage/IauEtVous/CartesEtDonnees/cartesetdonnees/opendata/MetaPDF/ICU_LCZ_Alea_Vuln_Champs_2022.pdf

- attributs couche ilot :https://www.institutparisregion.fr/fileadmin/DataStorage/IauEtVous/CartesEtDonnees/cartesetdonnees/opendata/MetaPDF/LCZ_ICU2022.pdf
- avec note vulj/vuln finale de vulnerabilité à une vague de chaleur basée sur ICU potentiel la nuit.

VEGETATION 

INONDATION
