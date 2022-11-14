I) Conteneurisation de l’application web

1) Création de l'image

![image](https://user-images.githubusercontent.com/115996823/201756623-0dfaccc1-0aad-4b00-aa6b-64621ac71aee.png)

2) Définir le répertoire /opt comme répertoire de travail

![image](https://user-images.githubusercontent.com/115996823/201757658-98769b13-334c-4426-aae7-922176f413d5.png)

3) Installer le module Flask version 1.1.2 à l’aide de pip install flask==1.1.2

![image](https://user-images.githubusercontent.com/115996823/201757418-777e4175-8b1d-4c3f-96b7-2b59e3d6c778.png)

4) Exposer le port 8080 qui est celui utilisé par défaut par l'application

![image](https://user-images.githubusercontent.com/115996823/201758381-af8d7698-02e6-478b-b3f4-63ab44c09afa.png)


5) Créer les variables d’environnement ODOO_URL et PGADMIN_URL afin de permettre la définition de ces url lors du lancement du container

ODOO_URL :

![image](https://user-images.githubusercontent.com/115996823/201757903-83d80dcc-5e2f-4dd7-9d35-98c6cd87ab78.png)

PGADMIN :

![image](https://user-images.githubusercontent.com/115996823/201757957-fffa8296-91ac-4aa0-9cb6-3f2ed3ed3158.png)

6) Lancer l’application app.py dans le ENTRYPOINT grâce à la commande python

![image](https://user-images.githubusercontent.com/115996823/201765710-4b4652a7-4d57-40cc-8aed-856b01eb9785.png)
![image](https://user-images.githubusercontent.com/115996823/201765724-79800a78-fd06-4aca-968a-1d11361de5b6.png)
![image](https://user-images.githubusercontent.com/115996823/201765852-3fea4159-6687-4a26-b2ab-e8c3ee9d641e.png)



