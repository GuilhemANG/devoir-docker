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
![image](https://user-images.githubusercontent.com/115996823/201777537-9a88954d-32b1-462d-a650-2e71a4e68038.png)
![image](https://user-images.githubusercontent.com/115996823/201777554-27bbddeb-0017-443d-85c3-78e53a769d74.png)
![image](https://user-images.githubusercontent.com/115996823/201777562-cb751dac-78e3-4624-9ab2-aa5bbe2af4b9.png)
![image](https://user-images.githubusercontent.com/115996823/201778044-264bff39-c20c-4490-820c-babf6109b4b7.png)

II) Docker Registry

1) Mettez en place un registre privé avec docker registry.

![image](https://user-images.githubusercontent.com/115996823/201862078-0de98866-fd89-4226-843a-482053bb5490.png)

2) Vous pourrez rajouter une interface web à ce registre

![image](https://user-images.githubusercontent.com/115996823/201862158-b6ddc09d-20dc-4bd2-9714-a73fbbba8e04.png)

Créons une interface web pour notre registre privé :

![image](https://user-images.githubusercontent.com/115996823/201872194-ef3734b2-86ce-44bc-ae16-2e0f9eaa31c5.png)

3) Une fois le test terminé, supprimez le container test et poussez votre image sur votre registre privé Docker, et aussi sur le registre dockerhub.

![image](https://user-images.githubusercontent.com/115996823/201872294-1a30a2df-e594-49e6-acf4-ff5aa4e625cb.png)

![image](https://user-images.githubusercontent.com/115996823/201907866-db0ae763-926b-4718-bed0-36d0bce45745.png)

![image](https://user-images.githubusercontent.com/115996823/201907891-bf72fe96-ecdf-4c47-a65e-86b8ec9bf39a.png)

![image](https://user-images.githubusercontent.com/115996823/201907940-0e681c65-477e-4047-b6db-ecbc3e48631d.png)





