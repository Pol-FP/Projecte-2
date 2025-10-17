 

#### 

- Per entrar al mode **GRUB**, premerem la tecla **Shift** i qualsevol altra tecla mentre s’inicia la màquina.Un cop aparegui el menú, seleccionarem l’opció **Advanced options for Zorin**.
![Menu inicial GRUB Zorin OS](img/image1.png)
- Quan siguem dins, escollirem **Zorin (recovery mode)**.  
  (se me olvido la foto)  
- A continuació, se’ns mostrarà el menú de recuperació, on triarem l’opció **root**.  
![Menu de recuperacion de Zorin amb diverses opcions](img/image2.png) 
- Executarem la següent comanda per muntar el disc i poder editar arxius:  
  `mount -rw -o remount /`  
![Terminal Con la comanda mount](img/image3.png)  
- Després, canviarem la contrasenya de l’usuari amb la comanda següent:  
  `passwd miquel`  
![Terminal Con la comanda passwd](img/image4.png) 
- Un cop feta la modificació, reiniciarem el sistema. En tornar a iniciar, ja podrem entrar amb la nova contrasenya.  
  ![Escritori Zorin](img/image5.png)
- A la terminal, escriurem la comanda següent `grub-mkpasswd-pbkdf2` Aquesta comanda generarà un hash per a la contrasenya que indiquem. Com que no volem escriure tot el hash manualment, podem utilitzar la comanda tee per desar-lo en un fitxer  
  `grub-mkpasswd-pbkdf2 | tee hash.txt`  
  ![Terminal Con la comanda grub](img/image6.png)  
  ![Terminal Con la comanda grub i tee](img/image7.png)
- Ara editarem l’arxiu `/etc/grub.d/40_custom` amb:  
  `sudo nano -F /etc/grub.d/40_custom`  
  ![Terminal Con la comanda sudo nano](img/image8.png) 
- Dins de *nano*, premerem **Ctrl \+ R** per obrir el fitxer on tenim el hash.  
  ![Interfaz NANO escribiendo buffer](img/image9.png)  
- Quan aparegui, ens situarem on comença el hash, premerem **Alt \+ A** per començar a seleccionar i marcarem tot el contingut. Després, premerem **Alt \+ 6** per copiar-lo. Tanquem l’arxiu amb **Ctrl \+ X**.  
  ![Interfaz NANO copiando el hash](img/image10.png)  
- A continuació, escriurem aquestes dues línies dins del fitxer `40_custom`  
  `set superusers="nom_usuari"`  
  `password_pbkdf2 nom_usuari hash`  
  A la primera línia hi posarem el nom de l’usuari, i a la segona escriurem el nom de l'usuari i enganxarem el hash copiat anteriorment amb **Ctrl \+ U**.  
  Guardarem i tancarem el fitxer.  
  ![Interfaz NANO con las dos lineas escritas i el hash pegado](img/image11.png)
- Finalment, aplicarem els canvis amb la comanda:  
  `sudo grub-mkconfig -o /boot/grub/grub.cfg`  
  ![Termianl Con la comanda grub](img/image12.png)  
- Ara, quan tornem a entrar al **recovery mode**, després de seleccionar *Advanced options for Zorin*, el sistema ens demanarà un usuari.  
  ![Menu grub Zorin](img/image13.png)  
- A més, en engegar la màquina, també se’ns sol·licitarà usuari i contrasenya per accedir.  
  ![Pantalla de que se requiere usuario y contrsaeña](img/image14.png)

R
