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

6. Cuando ya hayamos creado los tres ficheros, vamos 

