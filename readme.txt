Bienvenue dans l'édition du menu PSM pour "portable splash menu"

    1. Comment utiliser ce menu ?
    2. Les éléments éditables :
        2.1. La position du menu
        2.2. Le logo
        2.3. La liste de liens
    3. Licence

////////////////////////////////////////
1. Comment utiliser ce menu ?

1. Ouvrir le fichier menu.html
2. Copier les balises comprises entre les commentaires <!-- START PSM --> et <!-- END PSM --> ;
3. Coller ces balises dans votre fichier php directement après l'ouverture de la balise <body> ;
4. Copier le dossier files qui contient les dépendances dans le dossier où vous gérez vos dépendances ;
5. Ajouter une balise <link rel="stylesheet" href=""> dans le fichier php qui définit le contenu de la balise <head> ;
6. Renseigner le contenu de l'attribut href pour qu'il pointe sur le dossier files dans votre dossier de dépendances ;
7. Il restera à modifier le chemin d'accès au fichier du logo dans le dossier files dans votre dossier de dépendances (voir chapitre 2.2.).

////////////////////////////////////////
2.1. La position du menu

Il est réglable en modifiant les classes de la balise :
    <nav class="PSM_splash-menu">

Elle est repérable dans le fichier menu.html grâce au commentaire :
<!-- START positionnement du menu -->

On y ajoute les classe suivantes :
- PSM_top OU PSM_bottom
- PSM_left OU PSM_right

Le CSS prend le relai et ancrera automatiquement le menu en bas ou en haut, à gauche ou à droite.

////////////////////////////////////////
2.2. Le logo

Il est modifiable en modifiant la source et le contenu alternatif de la balise :
    <img class="PSM_logo-menu" src="logo.png" alt="Le projet CEC" />

Elle est repérable dans le fichier menu.html grâce au commentaire :
<!-- START logo -->

Etapes :
1. Créer un fichier image intitulé logo.png ;
2. Dans le dossier files du menu PSM, remplacer le fichier PNG intitulé logo.png, par votre image avec le même nom ;
3. Dans le fichier PSM_menu.html, modifier l'attribut alt de la balise <img class="PSM_logo-menu> afin qu'il corresponde à votre logo et fasse office de titre pour ce menu.

////////////////////////////////////////
2.3. La liste de liens

Il est modifiable en supprimant et ajoutant des balises :
    <li class="PSM_app-link-item">
        <a class="PSM_app-link" href="https://votre-url.com">Titre de votre lien</a>
    </li>

dans la balise :
    <ul  class="PSM_app-link-list" title="les applications du projet CEC">

La liste de lien est repérable dans le fichier menu.html grâce au commentaire :
<!-- START liens vers les applis -->

Etapes :
1. Modifier l'attribut title de la balise <ul  class="PSM_app-link-list"> afin qu'il décrive correctement l'ensemble des liens de votre menu ;
2. Supprimer et ajouter des balises <li class="PSM_app-link-item">...</li> ;
3. Modifier le contenu et l'attribut href de chacune des balises <a class="PSM_app-link"> de votre liste.

////////////////////////////////////////
3. Licence

Menu créé sous licence CCBY par Margot Nadot d'après le menu de Brad Traversy : https://codepen.io/bradtraversy/details/vMGBjQ