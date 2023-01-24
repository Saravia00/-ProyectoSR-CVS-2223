#  Proyecto-DNS

En este proyecto lo que haremos será crear un dominio principal, y a partir de ese dominio, crearemos tres subdominios, con sus correspondientes zonas, para ello hemos realizado un esquema que nos ayudará bastante, antes de realizar la práctica.

![Captura 1](https://user-images.githubusercontent.com/116157610/214312501-7d8f1f62-e481-42b3-9123-1d33f4b4324b.PNG)

1. Lo primero que hemos hecho, ha sido irnos a nuestra máquina ***Debian5-Pruebas***, una vez dentro nos vamos al siguiente fichero y crearemos nuestras zonas, como podemos ver en  ***Debian5-Pruebas*** tanto la  ***Zona directa*** como la ***Zona A*** , ***Zona B*** y la ***Zona inversa***, son masters, ya que ***Debian5-Pruebas***  es la máquina principial para estos dominios, y la ***Zona C*** es esclava, ya que su máquina principal es ***Debian6-Pruebas***.

   ![Captura 2](https://user-images.githubusercontent.com/116157610/214315719-c81c7055-a9ac-43c7-93b1-e6dc5c2b17c6.PNG)
   
   ![Captura 3](https://user-images.githubusercontent.com/116157610/214317706-8a9fc4c8-1c78-41c3-bca8-9b9c11fb0feb.PNG)

2. Despúes hemos creado un fichero, que le hemos llamado  ***iessanta.com***, en él hemos puesto la siguiente configuración: 

   ![Captura 4](https://user-images.githubusercontent.com/116157610/214359667-0975370b-8e81-4344-bb22-94f412749d16.PNG)

3. Una vez creado el fichero ***iessanta.com***, lo que vamos hacer ahora es crear el fichero ***biblioteca.com***, para ello pondremos la siguiente configuración:
   
   ![Captura 5](https://user-images.githubusercontent.com/116157610/214361970-52e15f83-8784-4aac-8ae9-296cd8c43895.PNG)
   
4. Luego crearemos el fichero ***recreo.com***, y pondremos la siguiente confiración:

   ![Captura 6](https://user-images.githubusercontent.com/116157610/214362374-889987c8-6106-4044-9299-d6aa9f980f96.PNG)

5. Ahora crearemos el fichero  ***consejeria.com***, y añadiremos la siguiente confiración:

   ![Captura 7](https://user-images.githubusercontent.com/116157610/214362619-787e8926-e5d0-4b44-b834-8aaf81744232.PNG)
   
6. Una vez ya creado los tres ficheros, lo que haremos será modificar el siguiente fichero, poniendo la siguiente configuración:

   ![Captura 8](https://user-images.githubusercontent.com/116157610/214366333-26eecaeb-286f-40a7-a2b2-a33d415c22f3.PNG)

7. Luego modificaremos el siguiente fichero, con la configuración que se muestra a continuación:

   ![Captura 9](https://user-images.githubusercontent.com/116157610/214366837-4344f8f1-da84-400f-8248-8fabf4df898e.PNG)

8. Ahora crearemos el siguiente fichero, que le hemos llamado ***iessantarrhh.com***, y hemos añadido lo siguiente:

    ![Captura 10](https://user-images.githubusercontent.com/116157610/214368047-9b77a782-6b84-46bf-9bc5-3f5ab6a5b978.PNG)
 
9. A continuacón vamos hacer transferencia de zonas, para ello, tendremos nuestra máquina ***Debian5-Pruebas*** como en ***Debian6-Pruebas***, encendidas, luego reiniciamos el servicio bind9 en ambas máquinas, poniendo el siguiente comando:

   ![Captura 11](https://user-images.githubusercontent.com/116157610/214371024-9d23750f-0999-4ae7-950e-25da0374754f.PNG)
    
   ![Captura 12](https://user-images.githubusercontent.com/116157610/214372317-069d3809-2bd9-4605-9105-17c390932def.PNG)

10. Ahora nos vamos a nuestra máquina ***Debian6-Pruebas*** nos vamos al directorio bind, haremos un ls para ver si se han copiado los ficheros, desde la máquina ***Debian5-Pruebas***, para ello haremos lo siguiente:

    ![Captura 13](https://user-images.githubusercontent.com/116157610/214373231-0727136a-a6f4-4c63-b899-742fc9899dbc.PNG)
    *Como podemos ver la transferencia se ha realizado correctamente

11. Ahora nos vamos a nuestra máquina ***Debian6-Pruebas*** nos vamos al directorio bind, haremos un ls para ver si se han copiado los ficheros, desde la máquina ***Debian5-Pruebas***, para ello haremos lo siguiente:
