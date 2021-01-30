# Autentificación,Autorización y Control de Acceso 📄
## En está práctica,vamos a modificar los sitios virtuales para permitir o denegar accesos provenientes de una IP

El cliente de la red interna,podrá acceder a ambas páginas,pero el cliente externo solo podrá acceder a una de ellas

### Pasos

### 1. Mantenemos la configuración de **/etc/hosts**

### 2. Modificamos la configuración de los sitios virtuales:

  * **Web1**
  
    A dicha web solo podrán acceder las IP que provenga de la red **2.0 y 3.0** || *"Deny all"* es opcional
    
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.4-web1.png)
   
  * **Web2**
  
    Solo podrán acceder las ip que provengan de la red **3.0** y deniega las demás conexiones
    
    ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.4-web2.png)
    

### 3. Comprobamos que la configuración es correcta

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.6.png)

### 4. Reiniciamos el servidor para aplicar los cambios

```systemctl restart nginx```

### 4. Comprobaciones

  * **Cliente red externa** --> SÍ podrá acceder a web1.org pero NO a web2org
  
  ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.3.2-externa.png)
  ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.3.1-externa.png)
  
  * **Cliente red interna** --> Podrá acceder a ambas páginas
  
  ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.3.3-interna.png)
  ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.3.4-interna.png)
