# Raccordement à Internet

## Raccordement au réseau informatique

![Capture d’écran](../../assets/raccordement-a-internet/image2020-2-9-22-16-1.png){ width=942 }

Suite à l'installation "physique" de la passerelle, il procéder au raccordement au réseau informatique ainsi qu'à Internet.  Le schéma suivant donne un aperçu des liens qui doivent être établis:

## Raccordement à Internet

Par la suite, vous devez configurer les "ports" d'accès Internet qui utilise le même système d'adresse IP que votre réseau local (couramment appelé LAN pour Local Area Network).  L'adresse IP de "votre site" sur Internet est assignée par votre fournisseur de services Internet (ex.: ExploreNet, Vidéotron, Bell, Xbox, etc.).  En comparaison, votre routeur voit réseau Internet comme un réseau "étendu" (couramment appelé WAN pour Wide Area Network).

Tous les PC, cellulaires ou tablettes raccordés à votre réseau local, et qui ont chacun une adresse IP spécifique, est vue sur Internet comme ayant une seule adresse IP, soit celle qui vous a été assignée par votre fournisseur.  Donc, si vous désirez accéder à vos données lorsque vous êtes à l'extérieur, il faut "router" les communications vers la passerelle Simplicollect.  Pour se faire, vous devez accéder à la configuration de votre routeur et ouvrir certains "ports" de communication.

| Veuillez noter que l'adresse IP publique qui vous est assignée est "temporaire" et peut être changée en tout temps, sans avertissement, par votre fournisseur.  Voir la section ci-dessous intitulée **DNS Dynamique**. |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

La première chose à savoir est de déterminer l'adresse IP que votre fournisseur vous a assignée:

1.  Sur votre PC ou laptop, ouvrez Chrome et tapez l'adresse suivante: <http://www.mon-ip.com>  et l'écran suivant apparaitra:

    ![Capture d’écran](../../assets/raccordement-a-internet/image2020-2-10-12-51-7.png){ width=1047 }

2.  Ceci est l'adresse IP de votre routeur... Il faut maintenant être capable de "router" les accès externes vers la passerelle Simplicollect;

3.  Pour ce faire, sur Chrome, tapez l'adresse IP de votre routeur et accéder à la page de "transfert de ports" (ou IP Forwarding en anglais) et inscrire les ports définit dans le tableau ci-dessous;

4.  Une fois que la configuration est faite, branchez-vous à l'aide d'une application Simplicollect (ex.: Dataview sur iOS ou Android) et entrez l'adresse IP de votre routeur (tel que trouvé ci-dessus) et le numéro de port défini ci-dessous.  Par exemple, l'application Dataview utiliserait le port 53333 pour accéder à votre passerelle à partir de l'extérieur... Voir la capture suivante:

5.  Sur cet exemple, cliquez sur le bouton Connecter... Si le message de bienvenue apparait et que vous passez au contenu de l'application, c'est que vous avez configuré correctement vos ports sur votre routeur.

![Capture d’écran](../../assets/raccordement-a-internet/2020-02-10-13-22qq-56.png){ width=226 }

#### Tableau des ports à ouvrir sur votre routeur vers l’adresse IP de la passerelle.

| Service             | Port sur la passerelle | Port sur Internet | Adresse IP de la passerelle |
|---------------------|------------------------|-------------------|-----------------------------|
| Service Dataview    | 3333                   | 53333             |                             |
| Service DataREST    | 3334                   | 53334             |                             |
| Service MAEREST     | 3335                   | 53335             |                             |
| RDP                 | 3389                   | 53389             |                             |
| Web (non-chiffré)   | 80                     | 8081              |                             |
| Web https (chiffré) | 443,4430               | 4430              |                             |
| FTP et SSH          | 22                     | 22                |                             |
| DATA                | 1433                   | 14333             |                             |

La difficulté dans la configuration des ports externes réside dans la multitude des marques et modèle de routeur sur le marché.  Les marques les plus populaires de routeur sont D Link, Asus, Netgear, Linksys.  Idéalement, achetez cet appareil chez un fournisseur qui peut vous donner des conseils techniques ou même en faire l'installation (ex.: Bureau en gros, Best Buy, La Source, etc.).  **Nous vous déconseillons d'acheter cet appareil directement sur Internet, car vous n'aurez pas l'assistance technique dont vous auriez besoin.**

| **Le service d'assistance technique de Simplicollect n'offre pas l'assistance technique sur vos équipements de réseau.  Soyez prévoyant de vous trouver un fournisseur de service dans votre région.** |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Sécurité de la passerelle

La passerelle Simplicollect contient un système d'exploitation complet fourni par Simplicollect. Cet appareil est pleinement sécurisé et ne peut être diagnostiqué ou mis à jour que par le personnel d'assistance technique de Simplicollect.  Les comptes d'utilisateur Simplicollect sont maintenus grâce à la fonction de sécurité que vous pouvez consulter au lien suivant: Sécurité Simplicollect

- [Modules](../../manuel-d-utilisation/configuration/modules.md)
- [Configuration](../../manuel-d-utilisation/configuration/index.md)
- [Tags](../../manuel-d-utilisation/configuration/tags.md)
- [Remplacement SIM sur MaestrEau](../module-maestreau-et-irrigation/remplacement-sim-sur-maestreau.md)
- [Configuration de la connexion Wifi et de l'adresse IP](../module-maestreau-et-irrigation/configuration-de-la-connexion-wifi-et-de-l-adresse-ip.md)
