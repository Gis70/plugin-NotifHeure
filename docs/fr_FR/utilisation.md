# Utilisation  
## Le widget  
Le widget est décopmosé en quatre zone , en fonction des options installés dans le notif'heure.  
  * Bloc 1 :  
  ![screenshot1](../images/partie1.png)  
  La partie haute représente l'etat du notif'heure en fonction des commandes envoyés .  
    * OFF   
        ![screenshot1](../images/off.png)   
    * Affichage des secondes  
        ![screenshot1](../images/partie1.png)
    * Masquage des secondes  
        ![screenshot1](../images/secoff.png)
    * Mode automatique ou Manuel  
        ![screenshot1](../images/manu.png)
    * Temoin led on / off  
        ![screenshot1](../images/ledon.png)   

  * Bloc 2 : Réglage de l'intensité pour le mode Manuel ( des que l'on modifie ce paramétrage le Notif'Heure passe en Mode Manuel pour la luminositée ).
  l'info Mode manuel  et valeur , s'affiche dans le bloc 1.  

  ![screenshot1](../images/partieint.png)

  * Bloc 3 : Options et Notification à envoyer.  

  ![screenshot1](../images/partienotif.png)

  Les Options possibles sont ( séparation possibles : , ou ; ou - ou : ) . Par exemple : _lum=8 , type=INFO , fio = 24 , important_   
  indiquera une luminosité de 8 , affichage de type INFO avec un effet en entrée et sortie de 24 , et ajoutera le tag important afin de le marquer pour l'historique.


  * **lum** : de 0 à 15 pour indiquer une valeur de luminositée  
  * **type** : Type d’animation ou de comportement BLINDS ,PAC ou OPENING : pour des effets d’animation avant la notification affiche l’info “txt” , contenu dans la variable txt.  
    * INFO : associé au champ “pause” permet d’afficher un texte court  entre 0 et 60 secondes.  
    * FIX : Affiche un texte court , en permanence . Une nouvelle notification envoyée , enleverra le texte. Si , on désire effacer sans afficher de texte , il faut utiliser le mot clé ” **!Clear!**” dans le champ message.  
  * **txt** : Un mot a afficher avant les effets d’animation ( la valeur par défaut renseigner dans la page de création sera utilisé si l'option txt n'existe pas ).  
  * **pause** : Associé à INFO , permet de définir un temps d’affichage entre 0 et 60 secondes.  
  * **flash** : pour activer le flash lumineux avant notification ( si LED présente )  
  * **fi**,**fo** ou **fio** : permet de choisir un effet pour la commande de type INFO . fi pour l’effet d’entrée , fo pour l’effet de sortie et fio pour définir le même effet en entrée et sortie. Par exemple fio=26,type=info permet un scrolling de la droite vers la gauche.  
  * **important** : Permet de rajouter un tag sur le message pour l’historisation et notification LED si présente.

  Vous pouvez retrouvez la documentation compléte sur mon site : https://byfeel.info

* Bloc 4 : Retrouvez les infos du DHT , si celui ci sont présentes dans le NotifHeure ( les infos sont réactualisés toutes les 30 minutes ).  

  ![screenshot1](../images/infodht.png)  

* Bloc 5 : Les commandes

  ![screenshot1](../images/commandes.png)   
   
  Dans l'ordre :
  * Off : Supprime affichage de l'Horloge  
  * On(reveil) : Affiche l'horloge  
  * Plus : Affiche les secondes si masqué
  * Moins : Masque les secondes  
  * Auto : Active le mode Auto  
  * Led On : Allume la led  
  * Led Off : Eteind la led  