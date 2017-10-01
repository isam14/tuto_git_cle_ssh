# tutoriel d'installation git et clé ssh

>**NOTE:**  Pour linux ubuntu chacune des commandes est a faire dans la terminal



## 1 - Installer Git sur sa machine :

### <i class="icon-file"></i> Mettre a jour les dépôts : 
 Commencer par un **SUDO APT-GET UPDATE** dans la console

### <i class="icon-file"></i> Installer git :
Ensuite faite un **SUDO APT-GET INSTALL GIT** dans la console



### L'installation de git sur votre machine est faite !


## 2 - Ajouter une clé SSH a son compte github relié a sa machine :


#### Tout d'abord verifié si une clé SSH n'est pas déjà présente sur votre système

faite un **cd ~/.ssh**
ensuite un **ls**

* dans ce dossier **ssh** vérifier la présence des fichiers **id_rsa** ou **id_dsa** qui sont vos clés privée , vérifier aussi si vous avez les fichiers en **.pub** qui sont elles vos clés publique !
 ### /!\ SI VOUS NE LES AVEZ PAS**
 
* IL SUFFIT DE LES CRÉER EN LANÇANT LE PROGRAMME **SSH-KEYGEN**

* UNE CONFIRMATION DE L'ENDROIT OU SAUVEGARDER LA CLÉ VOUS SERA DEMANDÉ APPUYER SUR ENTRÉ LAISSER PAR DÉFAUT

* ENSUITE IL VOUS DEMANDERA A DEUX REPRISE D'ENTRER UN MOT DE PASSE QUI PEUT RESTER VIDE POUR ÉVITER D'AVOIR À RETAPER LE MOT DE PASSE A CHAQUE FOIS QUE VOUS UTILISEREZ LA CLÉ !


#### Une fois tout cela fait :

* il vous suffit de vous rendre dans le dossier **ssh** en question de la manière suivant  **cd ~/.ssh/**

* d'ouvrir le fichier **id_rsa.pub** ou **id_dsa.pub**    
**(sudo gedit id_rsa.pub)**

* de copier le contenu y compris le **-rsa** au tout début

## Rendez vous sur github :


**Une fois sur gituhb**

* Cliquez sur l'onglet **"SETTINGS"** de votre profil .

* Une fois sur votre profil, sur la gauche vous verrez des onglets Selectionnez **"SSH and GPG KEYS"**  .

* Une fois sur l'onglet cliquez en haut à droite sur le **bouton vert** **"NEW SSH KEY"** .

*  Une zone de texte **"TITLE"** et **"KEY"** apparait en bas. dans le titre entrez par exemple **"mon pc personnel"** ou comment vous souhaitez appeler votre clé ssh .

* Dans la zone **"KEY"** Coller la clé précédemment copier dans le fichier **id_rsa.pub** 

* Puis validez en cliquant sur le bouton vert **"ADD SSH KEY"**


## Voila vous y êtes, vous pouvez désormais utiliser git sur votre machine relié à votre compte github. 


>- NOTE : **si vous rencontrez un problème au moment d'un commit ou d'un push il vous suffit d'entrez votre adresse mail et votre pseudo dans la config de git sur votre machine**

#### * La démarche a suivre :

* tapez dans votre console **git config --global user.email "Votre email"**
* et **git config --global user.name "Votre pseudo"**

**J'espère vous avoir aider, Bon versionnage !**