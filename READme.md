# ToIP téléphone

Objectif :La communauté d'agglomération souhaite ne plus avoir qu'un abonnement pour la téléphonie à la place de plusieurs par commune.

Il vous est demandé :

- de faire une collecte des solutions d'abonnement ToIP disponibles sur le marché et d'en faire un tableau comparatif de synthèse.

- de rechercher et mettre en oeuvre une solution interne de téléphonie SIP suivant le cahier des charges suivant :

*la solution doit être gratuite.

*permettre l'enregistrement et l'appel des postes  avec Qos  internes fixe IP et smartphones avec appli SIP via WiFi

*permettre l'enregistrement de messages vocaux l'ors de non réponses

*permettre l'accès à la téléphonie extérieure via un fournisseur (possibilité non mis en oeuvre)




# Installation Asterik
D'abord télécharge le fichier ISO sur: 
[https://asterisk.org/downloads/]()


![clipboard.png](lRol50Asg-clipboard.png)


Pourquoi choisir Asteriks au lieu de ses concurrents ?

| Service      | open-source | Gratuit?     | User Experience  |
| ------- | ------- | ------- | ------- |
| Asterik | OUI | OUI | Facile
| 3cx | OUI | OUI | Difficile
| Cloud Talk | NON | NON | Facile
| 8x8 | NON | NON | Facile


On va utiliser Hyper-V comme VM.

![clipboard.png](ZHPNrYLKu-clipboard.png)

Changer les ports ethernet en retirant le default switch principal et en ajoutant une carte réseau héritée **(ceci permet d'éviter le problème ultérieur avec Freepbx et le commutateur par défaut, pour une raison inconnue, il a des problèmes pour reconnaître le commutateur par défaut.)**
![clipboard.png](wm7oKGjX5-clipboard.png)



Choissisez < **Fully Automatic Installation - Output to VGA** >
![clipboard.png](wRwpoR_WC-clipboard.png)
mot de passe 'SangomaDefaultPassword'


Un address IP est fournis.
![clipboard.png](9NoDndLHF-clipboard.png)

Après avoir connu votre adresse IP , ping l'ip a l'aide de votre invite de commande (CMD).
![clipboard.png](6oRPtxzta-clipboard.png)

# Configuration Freepbx

Connecter vous a votre address IP et créer votre mot de passe.

Username: Shibuya 
Password : Jjk@2022
![clipboard.png](jdUTNycIB-clipboard.png)
Vous pouvez ensuite créer votre propre extension de VoIP.
![clipboard.png](9dfxHr4Z7-clipboard.png)

# VoIP phone configuration

Brancher votre téléphone VoIP en mode POE puis puis trouver l'adresse IP

![clipboard.png](A2IMSJb7G-clipboard.png)

Entrez l'ip dans votre navigateurs

login: admin

mot de passe: 22222


Vous pouvez maintenant configurer vos lignes téléphoniques.
![clipboard.png](m1tqghiGt-clipboard.png)