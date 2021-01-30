# Autentificación,Autorización y Control de Acceso 📄
## Procedemos a configurar la autentificación mediante las IP
Si accedemos desde la red externa pedirá autorización,pero desde la red interna no

### Pasos

### 1. Mantenemos todas las configuraciones anteriores

### 2. Configuramos el sitio virtual de nuevo

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/8.1.png)

### 3. Comprobamos que la configuración es correcta

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.6.png)

### 4. Reiniciamos el servicio

```systemctl restart nginx```

### 5. Comprobaciones

   * Cliente red externa
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/8.2.png)
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/8.3.png)
   
   * Cliente red interna

   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/7.5.png)
