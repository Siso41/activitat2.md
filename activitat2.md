# Avtivitat 2
## Com instal·lar Owncloud

### Instal·lació Apache:
El primer pas serà instal·lar Apache.
Instal·larem apache server amb aquesta comanda: sudo apt install apache2
-foto-

I tot segit desactivarem el llistat de directoris del servidor amb aquesta comanda: 
sudo sed -i "s/Options Indexes FollowSymLinks/Options FollowSymLinks/" /etc/apache2/apache2.conf
-foto-

### Instal·lació MariaDB:

Seguirem amb la instal·lació de MariaDB.
Ho instal·larem amb aquesta comanda: sudo apt-get install mariadb-server mariadb-client -y

