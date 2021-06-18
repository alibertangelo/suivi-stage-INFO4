# Suivi de stage INFO4 - Angelo ALIBERT

## Semaine 5 - 14 Juin 2021

La version 3 du logiciel Kallisté a été codée en rapartant "de zéro". Tous les objets/widgets à disposition de l'utilisateur (led, cadrans, afficheurs, boutons, graphes...) doivent donc être réimplémentés, avec un achitecture et organisation différente du code et des fichiers, tout en gardant les mêmes propriétés. Voici un aperçu de la structure nécessaire pour définir un objet : 

![capture_led_cpp](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Led_cpp.png)

Dans cette nouvelle version, les propriétés de chaque objet sont décrites dans un fichier Json à l'aide de UUID, reliés par la suite aux setters/getters dans le code c++.

![capture json led](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Led_sdsod_json.png)

Voici un aperçu du rendu final dans le logiciel Kallisté (ici sur la version 2) où l'on peut voir une led avec ses propriétés sur la droite :

![capture_kalliste_v2_led](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/KallisteV2_led.png)  

Pour réaliser le portage des objets, mon travail consiste donc à :  
- Générer le fichier JSON pour chaque objet décrivant toutes ses propriétés  
- Ecrire les fichiers headers décrivant les méthodes et attributs de chaque objet/widget/sous-widgets
- Implémenter les méthodes c++ (setters/getters/méthodes internes...) en me basant sur le code de la v2.  

## Semaine 4 - 7 Juin 2021

- Réalisation de tests unitaires sur les fonctions de manipulation de vecteurs, matrices et listes de vecteurs (SetColumun, SetRow, Remove).  
- Ajout des conversions entre les types QSize, QPoint, CSDSSample et CSDSComplex.  

## Semaine 3 - 31 Mai 2021

- Réalisation de tests unitaires sur les fonctions de manipulation de vecteurs, matrices et listes de vecteurs (Append, AppendRow, AppendColumn, InsertRow, InsertColumn...).    

## Semaine 2 - 25 Mai 2021

- Réalisation de nouveaux tests unitaires sur les fonctions de conversion entre scalaires, vecteurs, matrices et listes de vecteurs.  


## Semaine 1 - 17 Mai 2021

- Réalisation de nouveaux tests unitaires sur les fonctions de conversion entre scalaires.  
- Suivi du parcours HSE : Présentations des règles pour la sécurité, l'hygiène et l'environnement qui s'appliquent au sein du groupe Nexeya.
- Découverte de l'outil QTest fourni par Qt pour l'édition des tests unitaires.  

## Semaine 0 - 10 Mai 2021

Voici un résumé de cette première semaine qui n'a duré seulement que 3 jours à cause du week-end ferié :  
- J'ai suivi un tutoriel pour découvrir le logiciel Kallisté, produit sur le quel est centré mon stage. Il permet d'éditer des minis programmes pré-compilés et des synoptiques en faisant de simple glissés/déposés avec de nombreux plugings (compteurs, afficheurs, graphes, led, boutons...).
- Mon tuteur a procédé à l'installation des logiciels nécessaires sur windows (Visual studio, Qt, Git..) et cloné le code source c++ de l'application Kallisté.  
- J'ai commencé ensuite à réaliser des tests unitaires sur les fonctions de conversion. Le logiciel permettant à l'utilisateur de ne pas se soucier des conversions de données, chaque conversion doit être vérifiée et certaines doivent être refusées (ex: "abc" -> int). Le logiciel Kallisté utilise de nombreux types dont certains sont personnalisés : int, uint, short, ushort, long, ulong, char, uchar, bool, float, double, QDate, QTime, QDateTime, QColor, QString, SDSComplex, SDSPoint, SDSSize, SDSScalar, SDSVector, SDSMatrix, SDSVectorList. Voici un extrait des tests :

![capture1](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Capture%20d%E2%80%99%C3%A9cran%202021-05-12%20152910.png)
![capture2](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Capture%20d%E2%80%99%C3%A9cran%202021-05-12%20153010.png)
