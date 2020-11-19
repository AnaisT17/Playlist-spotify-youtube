# Générateur de playlists Spotify


Mise en place d'un script qui permet de prendre nos vidéos Youtube simple et générer une liste 
de lecture Spotify, basée sur la chanson de nos vidéos préférées. 

### Technologies

* Youtube Data API v3
* Spotify Web API
* Requests Library v 2.22.0
* Youtube_dl v 2020.01.24

- Environnement virtuel :

`python3 -m venv env`

- Activer environnement virtuel :

`source env/bin/activate`


### Configuration Locale : 

1. Installer les dépendances : 
`pip3 install -r requirements.txt`

2. Récupérez votre identifiant d'utilisateur Spotify et votre token Oauth à partir de Spotfiy et ajoutez-le au fichier **secrets.py**
- Pour récupérer votre identifiant d'utilisateur, connectez-vous à Spotify puis allez ici: [Account overview][1] et Username

![Compte Spotify](https://anaist17.github.io/Blog-Python/images/spotify.png)

- Pour récupérer votre token Oauth, visitez cette URL ci: [Get Oauth][2] et cliquez sur le bouton **Get token**.


![Token Youtube](https://anaist17.github.io/Blog-Python/images/youtube.png)

3. Activez Oauth pour Youtube et téléchargez le client_secrets.json
- Pour vous aidez suivez le [guide.][3]

4. Exécutez le fichier : 
`python3 create_playlist.py`

- Vous verrez immédiatement, depuis votre terminal : `Please visit this URL to authorize this application: <some long url>`
- Cliquez dessus et connectez-vous à votre compte Google pour collecter le `authorization code`



[1]: https://www.spotify.com/us/account/overview/
[2]: https://developer.spotify.com/console/post-playlists/
[3]: https://developers.google.com/youtube/v3/getting-started/

