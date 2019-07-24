# python
installer python 3.x


# installer mon environnement virtuel 
# pip3 install virtualenv



# je creer mon dossier 
# a l'interieur du dossier

# python3 -m venv venv_nom_de_mon_environnement_virtuel 


# django 

# activer mon env virtal 
# source ./bin/activate

# desactiver mon env virtual
# source ./bin/deactivate


# dans mon environnement virtuel (env)$

# pip install django (pas esoin de faire pip3 car mon environnement utilise python3 et pip3 )

# django-admin --version (voir la version )

# django-admin startproject nomDeMonProjet . ( le point pour rester dans le dossier courant et ne peas creer un autre repertoire pacha
 
 # a linterieur de mon projet ./manage.py runserver 127.0.0.1:8090 (permet de lancer mon projet dans le navigateur )
 
 
from io import  BytesIO

from PIL import Image
import requests

# je creer une instance de mon object
#im = Image.open("test.png")
#print(im.size, im.width, im.height )
#print(im.format, im.info)
#print(im.mode)
#im.save("tary-1.bmp", "BMP")

# resize the image

#nouvel_taille = im.resize((100, 300))
#nouvel_taille.show()



def download_img(url, file_name):
    r = requests.get(url)
    img = Image.open(BytesIO(r.content))
    img.save(file_name)



if __name__ == "__main__":
    url_img = 'https://fr.ubergizmo.com/wp-content/uploads/2017/03/python-royal-smileys.jpeg'
    file = 'python.png'
    download_img(url_img, file)


-programmation
- la robotiaue 
- 

formation vendredi qpres midi (formation)



alex n'guessan fondateur qfrica connect digital
yao partir oprerationnel
