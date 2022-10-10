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


### Crearem la base de dades de owncloud:

Entrarem a MariaBD:

![](Selecció_019.png)

Crearem al base de dades:

![](Selecció_020.png)

Crearem l'usuari i contraseña:

![](Selecció_021.png)

Li donem acces a l'usuari creat a la base de dades:

![](Selecció_022.png)

### Instal·lar PHP i els seus mòduls necessàris:

![](Selecció_023.png)

Actulitzem els paquets amb el repositori:

![](Selecció_024.png)

Instal·lem PHP i els mòduls necessaris.

![](Selecció_025.png)

Després editarem el fitcher php.ini i canviarem alguns valors: 
file_uploads = On allow_url_fopen = On memory_limit = 256M upload_max_filesize = 100M display_errors = Off date.timezone = Europe/Madrid

Comanda per accedir: ***sudo nano /etc/php/7.1/apache2/php.ini***

![](Selecció_026.png)

### Instal·larem Owncloud: 

Descargarem la última versió i canviarem el propietari i els directoris d'owncloud.:

![](Selecció_029.png)

### Configurar Apache:

Entrarema la configuració i posarem aquest text:

![](Selecció_030.png)

# Activitat 3

#### Canviar nom i correu:

![](Selecció_075.png)

![](Selecció_074.png)


