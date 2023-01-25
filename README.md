#  Proyecto-DNS

En este proyecto lo que haremos será crear un dominio principal, y a partir de ese dominio, crearemos tres subdominios, con sus correspondientes zonas, para ello hemos realizado un esquema que nos ayudará bastante, antes de realizar la práctica.

![Captura 1](https://user-images.githubusercontent.com/116157610/214312501-7d8f1f62-e481-42b3-9123-1d33f4b4324b.PNG)

1. Lo primero que hemos hecho, ha sido irnos a nuestra máquina ***Debian5-Pruebas***, una vez dentro nos vamos al siguiente fichero y crearemos nuestras zonas, como podemos ver en  ***Debian5-Pruebas*** tanto la  ***Zona directa*** como la ***Zona A*** , ***Zona B*** y la ***Zona inversa***, son masters, ya que ***Debian5-Pruebas***  es la máquina principial para estos dominios, y la ***Zona C*** es esclava, ya que su máquina principal es ***Debian6-Pruebas***, para nuestra máquina ***Debian6-Pruebas***, sería al contrario, ya que la ***Zona C***  sería maestra y las demás zonas esclavas.

   ***Debian5-Pruebas (Sara)***

   ![Captura 2](https://user-images.githubusercontent.com/116157610/214315719-c81c7055-a9ac-43c7-93b1-e6dc5c2b17c6.PNG)
   
   ![Captura 3](https://user-images.githubusercontent.com/116157610/214317706-8a9fc4c8-1c78-41c3-bca8-9b9c11fb0feb.PNG)ç
   
   ***Debian6-Pruebas (Sara)***
   
   ![Captura 2 2](https://user-images.githubusercontent.com/116157610/214636266-e47c3186-62aa-4c75-8a12-ff642567956b.PNG)

   ![Captura 2 3](https://user-images.githubusercontent.com/116157610/214636795-2293af9d-d88e-4031-bd56-9a2542f042b2.PNG)

   ***Debian5-Pruebas (Iván)***

   ![image](https://user-images.githubusercontent.com/91052724/214507522-85eb5142-9a98-4473-bd98-43745e9fa6f8.png)
   
   ![image](https://user-images.githubusercontent.com/91052724/214507660-f01c4039-3348-4fb3-8e6d-b557ceed4206.png)

   ***Debian6-Pruebas (Iván)***
   
2. Despúes hemos creado un fichero, que va ser nuestro dominio principal, al que le hemos llamado  ***iessanta.com***, en él hemos puesto la siguiente configuración: 

   ***Debian5-Pruebas (Sara)***
   
   ![Captura 4](https://user-images.githubusercontent.com/116157610/214359667-0975370b-8e81-4344-bb22-94f412749d16.PNG)
   
   ***Debian5-Pruebas (Iván)***

   ![image](https://user-images.githubusercontent.com/91052724/214508785-250f46eb-d5f2-4bc9-84f2-f5dee9025ad2.png)

3. Una vez creado el fichero ***iessanta.com***, lo que vamos hacer ahora es crear los subdominios a partir del dominio ***iessanta.com*** al primer fichero le hemos llamado ***biblioteca.com***, y para ello pondremos la siguiente configuración:
   
   ***Debian5-Pruebas (Sara)***
   
   ![Captura 5](https://user-images.githubusercontent.com/116157610/214361970-52e15f83-8784-4aac-8ae9-296cd8c43895.PNG)
   
   ***Debian5-Pruebas (Iván)***
   
   ![image](https://user-images.githubusercontent.com/91052724/214519743-2d23e27a-2fd3-4363-8598-75adfe916634.png)
   
4. Luego crearemos el segundo fichero, que le hemos llamado ***recreo.com***, y pondremos la siguiente configuración:

   ***Debian5-Pruebas (Sara)***

   ![Captura 6](https://user-images.githubusercontent.com/116157610/214362374-889987c8-6106-4044-9299-d6aa9f980f96.PNG)
   
   ***Debian5-Pruebas (Iván)***

   ![image](https://user-images.githubusercontent.com/91052724/214515234-f70a8bb0-b93d-4f5d-814b-9a6ed2d263dd.png)

5. Ahora crearemos el tercer fichero, que le hemos llamado ***consejeria.com***, y añadiremos la siguiente configuración:

   ***Debian5-Pruebas (Sara)***
   
   ![Captura 7](https://user-images.githubusercontent.com/116157610/214362619-787e8926-e5d0-4b44-b834-8aaf81744232.PNG)
   
   ***Debian5-Pruebas (Iván)***
   
   ![image](https://user-images.githubusercontent.com/91052724/214515304-121b3764-5b73-451d-9124-e95193c549ae.png)
   
6. Una vez ya creado los tres ficheros, lo que haremos será modificar el siguiente fichero, porque ahí es donde tendremos los registros PTR, y la configuración es la siguiente:

   ***Debian5-Pruebas (Sara)***
    
   ![Captura 8](https://user-images.githubusercontent.com/116157610/214366333-26eecaeb-286f-40a7-a2b2-a33d415c22f3.PNG)
   
   ***Debian5-Pruebas (Iván)***
   
   ![image](https://user-images.githubusercontent.com/91052724/214511268-58e5dceb-966a-4a3f-89e5-65fbad90e362.png)

7. Luego modificaremos el siguiente fichero, que también tendremos registros PTR, para ello haremos lo que se muestra a continuación:

   ***Debian5-Pruebas (Sara)***

   ![Captura 9](https://user-images.githubusercontent.com/116157610/214366837-4344f8f1-da84-400f-8248-8fabf4df898e.PNG)
   
   ***Debian5-Pruebas (Iván)***
   
   ![image](https://user-images.githubusercontent.com/91052724/214511586-f2cc3667-cbc6-405a-96c9-03dec5829134.png)

8. Ahora crearemos el siguiente fichero, que le hemos llamado ***iessantarrhh.com***, en él pondremos registros de direció IP, para ello, hemos añadido lo siguiente:

    ***Debian5-Pruebas (Sara)***
    
    ![Captura 10](https://user-images.githubusercontent.com/116157610/214368047-9b77a782-6b84-46bf-9bc5-3f5ab6a5b978.PNG)
    
    ***Debian5-Pruebas (Iván)***
    
    ![image](https://user-images.githubusercontent.com/91052724/214511763-ebf8505e-e33a-4f75-a3eb-f80c0d5fbd29.png)
    
9. Después de crear los ficheros, lo que vamos hacer es configurar en los ficheros de ***Debian5-Pruebas*** y ***Debian6-Pruebas***, porque lo que queremos hacer es que ***Debian1-Pruebas*** actúe como servidor de DNS, para ello haremos lo siguiente:
     
     ***Debian5-Pruebas (Sara)***
     
     ![Captura 21](https://user-images.githubusercontent.com/116157610/214651697-cedd7a1c-c9b4-4bb9-95af-133c481841c6.PNG)
     
     ***Debian6-Pruebas (Sara)***
      
     ![Captura 22](https://user-images.githubusercontent.com/116157610/214655893-32c75c04-efa9-49db-b74a-13c9efc45674.PNG)
      
     ***Debian5-Pruebas (Iván)***
     
     ![image](https://user-images.githubusercontent.com/91052724/214706779-239bbe05-33f1-4923-967c-e3be3dfbff78.png)

     ***Debian6-Pruebas (Iván)***

     ![image](https://user-images.githubusercontent.com/91052724/214706975-948e0562-1029-49aa-a9ad-41c20a9768f5.png)


10. Ahora vamos a modificar el siguiente fichero tanto en la máquinas ***Debian5-Pruebas*** como en ***Debian6-Pruebas***, para poder hacer las transferencias de zonas, desde ***Debian5-Pruebas*** a ***Debian6-Pruebas*** para ello hacemos lo siguiente:


    ***Debian5-Pruebas (Sara)***
     
    ![Captura 23](https://user-images.githubusercontent.com/116157610/214661778-af2ef455-efec-4b57-9e1b-50e92fcc4fcf.PNG)
     
    ***Debian6-Pruebas (Sara)***
      
    ![Captura 24](https://user-images.githubusercontent.com/116157610/214662653-acfdf470-a03b-43d2-b6a4-a0890f43177d.PNG)

    ***Debian5-Pruebas (Iván)***
     ![image](https://user-images.githubusercontent.com/91052724/214707428-953e7472-fed2-4e81-b488-0ff920ab68d9.png)

    *Debian6-Pruebas (Iván)**

![image](https://user-images.githubusercontent.com/91052724/214707727-64d9db66-0448-460f-8175-a8c3dd0ffe51.png)

11. A continuacón vamos a hacer las transferencias de zonas, para ello, tendremos nuestra máquina ***Debian5-Pruebas*** como en ***Debian6-Pruebas*** , encendidas, luego reiniciamos el servicio bind9 en ambas máquinas, poniendo el siguiente comando:

   ***Debian5-Pruebas (Sara)***
   
   ![Captura 11](https://user-images.githubusercontent.com/116157610/214371024-9d23750f-0999-4ae7-950e-25da0374754f.PNG)
   
   ***Debian6-Pruebas (Sara)***
    
   ![Captura 12](https://user-images.githubusercontent.com/116157610/214372317-069d3809-2bd9-4605-9105-17c390932def.PNG)
   
   ***Debian5-Pruebas (Iván)***
     
   ***Debian6-Pruebas (Iván)***

12. Ahora nos vamos a nuestra máquina ***Debian6-Pruebas*** nos vamos al directorio bind, haremos un ***ls*** para ver si se han copiado los ficheros, desde la máquina ***Debian5-Pruebas***, para ello haremos lo siguiente:

    ***Debian6-Pruebas (Sara)***
    
    ![Captura 13](https://user-images.githubusercontent.com/116157610/214373231-0727136a-a6f4-4c63-b899-742fc9899dbc.PNG)
    *Como podemos ver la transferencia se ha realizado correctamente.

    ***Debian6-Pruebas (Iván)***
    
13. Ahora comprobaremos en mi caso he realizado algunas pruebas tanto  en ***Debian5-Pruebas***, como en ***Debian6-Pruebas***, para ello haremos lo siguiente:

    ***Debian5-Pruebas (Sara)***
    
    ![Captura 25](https://user-images.githubusercontent.com/116157610/214708920-a7174b0b-7768-4b75-adc8-0f0f48979d91.PNG)

    ***Debian6-Pruebas (Sara)***
    
    ![Captura 26](https://user-images.githubusercontent.com/116157610/214709067-d246b5ba-cf67-4219-9e1f-c0e54ef20bd7.PNG)
    *Como podemos ver funciona correctamente.
    
    ***Debian5-Pruebas (Iván)***
     
    ***Debian6-Pruebas (Iván)***

14. Haremos dos reservas, en nuestra máquina ***Debian1-Pruebas***, en nuestro caso hemos elegido las siguientes máquinas con su configuración correspondiente:

    ***Debian1-Pruebas (Sara)***
    
    ![Captura 14](https://user-images.githubusercontent.com/116157610/214376449-a9887613-e69a-4768-9acb-fb1e3c4d7f50.PNG)

    ***Debian1-Pruebas (Iván)***

15. Vamos a empezar con ***Debian2-Pruebas***, en vez de conectarnos por terminator, nos vamos directamente a nuestra máquina, ya que cuando borramos la IP en terminator se desconecta directamente, así que lo primero que haremos será borrar la IP que teníamos, con el siguiente comando:

    ***Debian2-Pruebas (Sara)***

    ![Captura 15](https://user-images.githubusercontent.com/116157610/214379412-35a43590-adae-42ce-979a-5f50fecf17dd.PNG)

16. Después pediremos la IP con el comando que se muestra a continuación:

    ***Debian2-Pruebas (Sara)***
    
    ![Captura 16](https://user-images.githubusercontent.com/116157610/214379628-106b11b5-7f47-4cbe-bc57-f8cdba27d0e5.PNG)

17. Ahora comprobaremos que nos pone la IP deseada, poniendo el siguiente comando:

    ***Debian2-Pruebas (Sara)***

    ![Captura 17](https://user-images.githubusercontent.com/116157610/214380390-be884670-1d9c-4806-ae6d-ecf4aae291ce.PNG)

18. Una vez realizado los pasos anteriores, ahora lo haremos con ***Debian3-Pruebas***, borramos la IP que teníamos con el siguiente comando:

    ***Debian3-Pruebas (Sara)***
    
    ![Captura 18](https://user-images.githubusercontent.com/116157610/214385098-80270f37-e188-47bf-8002-2bba9c6bfbf4.PNG)

19. Ahora pediremos la IP con el siguiente comando:

    ***Debian3-Pruebas (Sara)***

    ![Captura 19](https://user-images.githubusercontent.com/116157610/214385208-2f527f03-8377-4f71-b29b-d2a6e9557f6e.PNG)

20. Finalmente comprobaremos que nos pone la IP deseada, con el siguiente comando:

    ***Debian3-Pruebas (Sara)***
    
    ![Captura 20](https://user-images.githubusercontent.com/116157610/214385277-c8168f72-f3cf-4b6c-9cee-055c2a988094.PNG)

21. Para acabar, lo que haremos será un commit, para guardar la configuración que hemos realizado, para ello pondremos el siguiente comando:

    ***Debian5-Pruebas (Sara)***
    
    ![Captura 27](https://user-images.githubusercontent.com/116157610/214710178-5c65d238-7cf4-49a9-9cbd-5faa0a66466b.PNG)


