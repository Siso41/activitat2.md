# Avtivitat 2
## Com instal·lar Owncloud

### Instal·lació Apache:
El primer pas serà instal·lar Apache.
Instal·larem apache server amb aquesta comanda: sudo apt install apache2

![](Selecció_012.png)

I tot segit desactivarem el llistat de directoris del servidor amb aquesta comanda: 
sudo sed -i "s/Options Indexes FollowSymLinks/Options FollowSymLinks/" /etc/apache2/apache2.conf

![](Selecció_013.png)

### Instal·lació MariaDB:

Seguirem amb la instal·lació de MariaDB.
Ho instal·larem amb aquesta comanda: sudo apt-get install mariadb-server mariadb-client -y

![](Selecció_014.png)

I configurarem la instal:lació:

![](Selecció_015.png)

I farem els següents canvis:

- Deshabilitar usuaris anònims.
- Deshabiliteu accés remot com a root.
- Eliminar les bases de dades de testeig i accedir-hi.
- Actualitzar les taules de privilegis.

![](Selecció_017.png)

I per últim reiniciarem el servidor MariaBD

![](Selecció_018.png)


