# GIT & GITHUB

**Git** est un logiciel de contr�le de version, ce qui signifie qu�il g�re les modifications d�un projet sans �craser n�importe quelle partie du projet.

**GitHub** fournit une interface visuelle pour vous aider � g�rer localement vos projets avec les contr�les de version. Deuxi�mement, cr�er un compte sur GitHub.com apporte les contr�les de versions � vos projets web, et leur conf�re des fonctionnalit�s de r�seaux sociaux.

**Ligne de Commande** : 
Le programme de l�ordinateur que nous utilisons pour entrer des commandes Git.(Git Bash)

**D�p�t** : 
Un r�pertoire ou de l�espace de stockage o� vos projets peuvent vivre. Parfois les utilisateurs GitHub raccourcissent �a en � repo �. Il peut �tre local sur un r�pertoire de votre ordinateur, ou ce peut �tre un espace de stockage sur GitHub ou un autre h�bergeur en ligne. � l�int�rieur d�un d�p�t, Vous pouvez conserver des fichiers de code, des fichiers texte, des images.

**Contr�le de Version**:
Git conserve des � instantan�s � de chaque point dans l�historique d�un projet, de sorte que vous ne pouvez jamais le perdre ou l��craser.

**Commit** : C�est la commande qui donne � Git toute sa puissance. Quand vous � committez �, vous prenez un � instantan� �, une � photo � de votre d�p�t � ce stade, vous donnant un point de contr�le que vous pouvez ensuite r��valuer ou restaurer votre projet � un �tat pr�c�dent.

**Branche** : Habituellement, elles se � d�branchent � du projet principal avec leurs propres versions compl�tes des modifications qu�elles ont chacune produites de leur c�t�. Apr�s avoir termin�, il est temps de � fusionner � cette branche pour la ramener vers la branche � master �, le r�pertoire principal du projet.


## Liste des commandes git

**init** : 
Cr�e un dossier git vide, ou (r�)initialise un dossier d�j� existant

**status** :
R�cup�re l'�tat actuel du dossier git
Voir quels fichiers sont � l�int�rieur, quelles sont les modifications � commiter, et sur quelle branche du repository on est en train de travailler.

**add**: 
cela porte de nouveaux fichiers � l�attention de Git. Apr�s avoir ajout� des fichiers, ils sont inclus dans les � instantan�s � du d�p�t Git.

**commit**: 
la commande la plus importante de Git. Apr�s avoir effectu� toute sorte de modification, on entre �a afin de prendre un �instantan� du d�p�t. G�n�ralement cela s��crit sous la forme git commit -m �Message ici�. Le -m indique que la section suivante de la commande devrait �tre lue comme un message.

**log**:
Affiche  tous les changements enregistr�s (les commit)
Historique du projet.

**remote add origin**:
Ajoute au dossier git un "repository" distant, et le lie a udossier 'origin'

**push** :
envoie sur le repo distant les modifications enregistr�es dans le dernier commit.

**push -u origin master**:
-u permet de se rappeler, das ce contexte d'utilisation, quels sont les param�tres de la fonction push :
	origin : l'�l�ment � push (notre repo local)
	master : le nom de la 'branch' dans laquelle nous allons push notre �l�ment

**pull** :
r�cup�re les changements du repo distant sur notre repo local

**pull origin master**:
'pull' dans origin ce qui vient de master

**diff**:
Montre les diff�rences entre l'�tat actuel de notre repo local et un �tat 'committ�'

**diff HEAD**:
Pr�cise que l'�tat auquel on veut comparer est le dernier commit

**reset**:
inverse de add sur un �l�ment. Si c'est un �l�ment qui a �t� 'add' au pr�sent commit, il ne le sera plus.

**checkout** :
remet l'�l�ment � l'�tat du pr�c�dent commit

**checkout <BranchName>**:
change de "branch" de travail, on travaille d�sormais sur la branch <BranchName>

**branch <NewBranchName>**:
cr�e une "branch" sur notre "arbre". On cr�e ainsi un nouveau contexte, ind�pendant de la branch "master", dans lequel nous allons travailler. on poura les merge �ventuellement plus tard

**branch**:
Liste l'ensemble des branch actuellement disponibles.

**rm**:
remove -> supprime de notre repo local le(s) �l�ment(s).

**merge <BranchToMerge>**:
fusionne la branch dans laquelle on travaille avec la branch <BranchToMerge>

**branch -d <BranchToDelete>**:
supprime la branch <BranchToDelete>

![schema](https://cdn.dribbble.com/users/138252/screenshots/2389144/github_dri.png)