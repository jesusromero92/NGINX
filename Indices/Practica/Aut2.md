# Autentificación,Autorización y Control de Acceso
## Vamos a configurar el sitio virtual de **web1.org** para que cuando accedamos a la ruta **/privado**,nos pida autentificación.
La autentificación sirve para proteger el contenido de nuestra página web

### Pasos

### 1. Creamos el directorio **privado** de nuestra página web
   Para ello,vamos a su **Directorio Raíz** y creamos la carpeta
    
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.png)
   
### 2. Instalamos el siguiente paquete
   Dicho paquete nos servirá para crear usuarios en texto plano pero encripta la contraseña
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.1.png)
   
### 3. Creamos los usuarios que podrán acceder a dicha ruta
   Creamos una carpeta donde se guardará el archivo con los usuarios autentificados y luego los creamos
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.2.png)
   
   
### 4. Configuramos el sitio virtual de WEB1 para habilitar la autentificación
   Añadimos el último párrafo,donde especificamos que ruta queremos proteger con contraseña
   
   **auth_Basic** Es el mensaje a mostrar cuando nos pida autentificarnos
   
   **auth_basic_user_file** Es el archivo que guarda los usuarios que podran acceder
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.3.png)
   
### 5. Comprobamos que la configuración es correcta

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.6.png)

### 6. Reiniciamos el servicio

```systemctl restart nginx```

### 7. Comprobaciones

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.4.png)
![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.5.png)
