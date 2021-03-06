# Data Formatting and Quality Control, Computing for Ecology  
# Mise en forme et contrôle qualité de données, l’informatique au service de l’écologie
#### Computer program and example relating to the article / Programme informatique et exemple relatifs à l'article 


# Abstract
In many scientific disciplines, experimental studies or field monitoring ensure the data collection. The data is stored on raw files with an intuitive format, easily entered by the experimenter. However, this raw format is rarely directly compatible with the analysis of the collected data and the data may be erroneous; it is then necessary to carry out a formatting and quality control. Faced with the increasing number of ever more massive raw data sets, the discipline of digital for life sciences has developed. Computer programming represents a precious help for modellers since it allows the automation of data formatting and data cleaning. The data formatting makes it possible to obtain a format that will be directly used in the analyses. Automation also enables to avoid errors generated by manual formatting, such as typing errors and omissions. Data cleaning, a term used in computer science, corresponds to the data quality control according to the criteria provided by the modeller. The modeller knows the range of values of the data obtained and the possible errors produced. In this article, we present a collaboration between computer scientist and modeller in the framework of animal abundance monitoring. The data collected on several sheets of a spreadsheet had to be gathered on one sheet and their quality had to be checked. The various functionalities of the program carrying out this verification were implemented using the agile method, a computer development method consisting of sprints. After a version was provided, a new sprint defined the next functionality to be implemented by the computer scientist in a new version of the program. The first version allows the appropriation of the dataset by the computer scientist thanks to the formatting functionality. A more advanced version manages the absence of data, then others check the collected data quality and reports the processing of detected anomalies, data missing or erroneous or outside a specified range, in a text file. This computer program has been explained so that it can be re-appropriated and re-used, the full version is available at https://github.com/FloHugon/DataFormatting.
#### Abundance, Agile software development, Computer Programming, Data cleaning, Data management.


# Résumé
Dans de nombreuses disciplines scientifiques, des études expérimentales ou des suivis sur le terrain assurent la récolte de données. Les données sont stockées sur des fichiers bruts avec un format intuitif, saisies facilement par l’expérimentateur. Cependant, ce format brut est rarement directement compatible avec l’analyse des données récoltées et peut engendrer des analyses erronées ; il est nécessaire d’effectuer une mise en forme et un contrôle qualité des données. Face au nombre de jeux de données bruts croissants et toujours plus massifs, la discipline du numérique pour les sciences du vivant s’est développée. La programmation informatique représente une aide précieuse pour les modélisateurs puisqu’elle permet d’automatiser la mise en forme et le contrôle qualité qui nécessitent souvent un nettoyage des données. Dans cet article, nous présentons une collaboration entre informaticien et modélisateur dans le cadre du suivi de l’abondance d’espèces animales. Les données récoltées sur plusieurs feuilles d’un tableur sont regroupées sur une seule et leur qualité est vérifiée. Les diverses fonctionnalités du programme effectuant cette vérification ont été mises en place à l’aide de la méthode « agile », méthode de développement informatique constituée de sprints. Après la fourniture d’une version du programme, un nouveau sprint définit une nouvelle fonctionnalité à mettre en place par l’informaticien dans une nouvelle version du programme. La première version permet l’appropriation du jeu de données par l’informaticien grâce à la fonctionnalité de mise en forme. Une version plus avancée gère l’absence de données, puis d’autres contrôlent la qualité des données récoltées et rapporte le traitement des anomalies détectées, donnée absente ou erronées ou en dehors d’une plage spécifiée, dans un fichier texte. Ce programme informatique a été explicité afin qu’il puisse être ré-approprié et ré-utilisé, sa version complète est disponible à l’adresse suivante https://github.com/FloHugon/DataFormatting.
#### Abondance, Gestion de données, Méthode « agile », Nettoyage des données,  Programmation Informatique.


# About joined files
Supply of the computer program and the input, output, anomaly, corrected output files for the example of a torrent with 4 sites. 

Input: raw data for the computer program.  
Output: output file obtained after running the computer program.  
Anomaly: text file which reports the anomalies detected.  
OutputCorrected: correction of the anomalies detected, not processed automatically by the program, by the modeller  

In this example, according to the sampling protocol :   
Cloudiness (Cloud variable) at 100% have been corrected by the number 5;  
Variable Flow "lent voire nul" and "Faible à nul" have been corrected by the value 1;  
The diameter of the largest basin (Variable MaxSize) was expressed in centimetres for all site;    
The variables S.trutta and N.maura have been indicated as 0 or 1;  
The values of the variables relative to the vegetative strata (Moss, Herbaceous, Shrubs and Trees) do not allow their correction as they are, it is necessary to observe the files of other years for the same torrent which may give more coherent values. Otherwise, these variables will not be usable for the abundance analysis. 


# A propos des fichiers joints
Fourniture du programme informatique et des fichiers input, output, anomalie, output corrected pour l’exemple d’un torrent découpé en 4 sites. 

Input : données brutes en intrant du programme informatique  
Output : fichier de sortie obtenu après l’exécution du programme informatique  
Anomalie : fichier texte qui reporte les anomalies détectées  
OutputCorrected : correction des anomalies détectées, non traitées automatiquement par le programme, par le modélisateur  

Dans cet exemple, selon le protocole d'échantillonnage :   
Les nébulosités (variable Cloud) à 100% ont été corrigées par le chiffre 5 ;  
Les débits (Variable Flow) "lent voire nul" et "Faible à nul" ont été corrigés par la valeur 1 ;  
Le diamètre de la plus grande vasque (Variable MaxSize) a été exprimé en centimètres pour tous les sites ;  
Les variables S.trutta et N.maura ont été indiquées selon 0 ou 1 ;  
Les valeurs des variables relatives aux strates végétatives (Moss, Herbaceous, Shrubs et Trees) ne permettent pas leur correction telle quelle, il est nécessaire d'observer les fichiers des autres années pour le même torrent qui renseigneront peut être des valeurs plus cohérentes. Dans le cas contraire, ces variables ne seront pas exploitables pour l'analyse d'abondance. 


# To test the program / Pour tester le programme
Download the input file and the PrgmInfo file (.xlsm), record them in a same folder. Open the PrgmInfo file and active macro, go to Display - Macro - Display macros. Select the macro to execute, clic on Execute, enter the input filename (here: "Input"), clic on OK.  
Télécharger le fichier Input et le fichier PrgmInfo (.xlsm), enregistrer les dans le même dossier. Ouvrir le fichier PrgmInfo et activer les macros, aller dans Affichage - Macro - Afficher les macros. Sélectionner la macro à exécuter, cliquer sur Exécuter, entrer le nom du fichier input (ici : "Input"), cliquer sur OK.

