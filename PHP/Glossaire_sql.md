Glossaire SQL
=============


----------

| Notions SQL (ou BDD en g�n�ral) | D�finition |
|--------------|--------------------------------|
|**Banque de donn�es** |  Collection de bases de donn�es|
|**Base de donn�es** | Collection de tables de donn�es |
|**Table**| Collection de lignes d'enregistrement|
|**Ligne d'enregistrement**|Collection de donn�es associ�es (exemple dans une table "client", une ligne peut contenir nom, pr�nom et adresse du client, dans des "cases" correspondantes)|
|**SGBD**|Syst�me de Gestion de Base de Donn�es|
|**Moteur SQL**|Programme qui manipule les fichiers de la BDD, et retranscrit les informations stock�es de mani�re "lisible" |
|**Catalogue**|Description de la BDD ++ informations "subsidiaires" (typiquement les droits d'acc�s � la base de donn�es)|
|**Requ�te**|Demande envoy�e � la BDD, qui va renvoyer|
|**Langage de requ�te**|Langage informatique dans lequel sera cod� les requ�tes envoy�s au SGBD|
|**Processeur de requ�te**|Programme d'interpr�tation de la requ�te|
|**Plan d'�x�cution**|Liste des op�rations � r�aliser sur la BDD. pour une requ�te �crite dans le langage de requ�te, le processeur de requ�te d�termine un plan d'�x�cution. Apr�s avoir v�rifier que toutes les op�rations n�cessaires au plan d'�x�cution sont autoris�es � l'utilisateur (v�rification dans le catalogue), le plan est envoy� au moteur SQL, qui renvoie le r�sultat de la requ�te|
|**Primary Key**|Cl� primaire : ensemble de donn�es d'un enregistrement (un ou plusieurs champs) permettant d'identifier de mani�re unique un enregistrement donn�. La cl� primaire est d�finie � la cr�ation de la table|
|**Foreign Key**|Cl� �trang�re : cl� fasat r�f�rence dans une table � la cl� primaire d'une autre table. Ce sont ces r�f�rences entre tables qui permettent de cr�er des relations entre ces tables.|
|**Cardinalit�**|La cardinalit� d�finit, dans une relation entre 2 tables, le nombre d'�l�ment de la table 2 que l'on doit relier � un enregistrement de la table 2. Il y a 4 types de cardinalit� possibles : <ul><li> 0..1 : Il y a 0 ou 1 enregistrement de la table 2 pouvant faire r�f�rence � un enregistrement de la table 1</li><li>  1 : Un seul enregistrement de la table 2 peut et doit faire r�f�rence � un enregistrement de la table 1.</li><li>  0..N : Il peut y avoir 0, 1 ou plusieurs enregistrements dans la table 2 faisant r�f�rence � un seul enregistrement dans la table 1. </li><li>  1..N : Il y a au moins un enregistrement dans la table 2 faisant r�f�rence � un enregistrement dans la table 1, il est possible d'en avoir plusieurs.</ul>|
|--|--|
|**Langage de d�finition de donn�es (LDD/DDL)**|Langage dans lequel s'�crit l'architecture de la BDD|
|**CREATE**|mot-cl� pour cr�er un �l�ment (**DATABASE**,**TABLE**,**VIEW**, **INDEX**)|
|**ALTER**|mot-cl� pour modifier (alt�rer) un �l�ment|
|**DROP**|mot-cl� pour supprimer un �l�ment|
|**Collation**|Table de conversion des caract�res sp�ciaux, par exemple pour les tris|
|**COLLATE**|mot-cl� d�finissant la collation � utiliser pour la table. ex. **COLLATE utf8_general_ci;**|
|--------------------|-------------------|
|**Langage de manipulation de donn�es (LMD/DML)**|Langage dans lequel les requ�tes INSERT SELECT UPDATE et DELETE sont �crites|
|--|--|
|**INSERT**|Insertion (cr�ation) de donn�es dans une table|
|**SELECT**|S�lection (lecture) de donn�es dans une table|
|**UPDATE**|Mise � jour (r��criture) de donn�es dans une table|
|**DELETE**|Suppression de donn�es dans une table

------------------------------------------------------------------------------------------
## PHP fait la jonction entre nous et MySQL

	Il va faire l'interm�diaire entre nous et **MySQL**. 
	On devra demander � **PHP** : 
	� Va dire � MySQL de faire ceci. �

![Sch�ma architecture d'un site](http://www.phpdebutant.org/system/images/intro/schema2.gif)

	le serveur utilise toujours PHP, il lui fait donc passer le message ;

	PHP effectue les actions demand�es et se rend compte qu'il a besoin de MySQL. 
	En effet, le code PHP contient � un endroit � Va demander � MySQL d'enregistrer ce message �. 
	Il fait donc passer le travail � MySQL ;

	MySQL fait le travail que PHP lui avait soumis et lui r�pond � O.K., c'est bon ! � ;

	PHP renvoie au serveur que MySQL a bien fait ce qui lui �tait demand�.
	Il peut donc renvoyer au client une page html.


