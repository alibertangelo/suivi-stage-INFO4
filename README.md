# Suivi de stage INFO4 - Angelo ALIBERT

## Semaine 2 - 17 Mai 2021

Réalisation de tests unitaires.  
Suivi du parcours HSE : Présentations des règles pour la sécurité, l'hygiène et l'environnement qui s'appliquent au sein du groupe Nexeya.

## Semaine 1 - 10 Mai 2021

Voici un résumé de cette première semaine qui n'a duré seulement que 3 jours à cause du week-end ferié :  
- J'ai suivi un tutoriel pour découvrir le logiciel Kallisté, produit sur le quel est centré mon stage. Il permet d'éditer des minis programmes pré-compilés et des synoptiques en faisant de simple glissés/déposés avec de nombreux plugings (compteurs, afficheurs, graphes, led, boutons...).
- Mon tuteur a procédé à l'installation des logiciels nécessaires sur windows (Visual studio, Qt, Git..) et cloné le code source c++ de l'application Kallisté.  
- J'ai commencé ensuite à réaliser des tests unitaires sur les fonctions de conversion. Le logiciel permettant à l'utilisateur de ne pas se soucier des conversions de données, chaque conversion doit être vérifiée et certaines doivent être refusées (ex: "abc" -> int). Le logiciel Kallisté utilise de nombreux types dont certains sont personnalisés : int, uint, short, ushort, long, ulong, char, uchar, bool, float, double, QDate, QTime, QDateTime, QColor, QString, SDSComplex, SDSPoint, SDSSize, SDSScalar, SDSVector, SDSMatrix, SDSVectorList. Voici un extrait des tests :

![capture1](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Capture%20d%E2%80%99%C3%A9cran%202021-05-12%20152910.png)
![capture2](https://github.com/alibertangelo/suivi-stage-INFO4/blob/main/images/Capture%20d%E2%80%99%C3%A9cran%202021-05-12%20153010.png)
