# Virtual Hosting
## En esta práctica,voy a crear 2 sitios virtuales con nombres diferentes y vamos a poder acceder desde un dominio local

### 1. Procedemos el directorio de ambos sitios virtuales **(Document Root)**
   Dicho directorio es donde se guardará toda la informacion a mostrar en el navegador
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.2.png)
   
   
   
   
   
   
   
   
   
   
   
### 2. Creamos el archivo de configuración de cada sitio virtual de la siguiente manera:
   Copiamos el default,ya que servirá como **base** para la configuración de nuestro sitio virtual
   
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.1.png)
     
### 3. Configuramos los archivos de configuración de la siguiente forma:

   * **Web 1**
    
        ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.1.2.png)
         
   * **Web 2**
    
        ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.1.3.png)
          
### 4. Comprobamos que la configuración es correcta
 
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.6.png)
   
### 5. Los sitios virtuales,están disponibles,pero están habilitados,para ello hacemos un enlace duro hacia la siguiente ruta

   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.3.png)

   
### 6. Reiniciamos el servicio para que se aplique la configuración

```systemctl restart nginx```

### 7. Solo queda configurar los DNS Locales para poder acceder

   * Cliente con red interna **(192.168.3.10)**
    
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/6.2-interna.png)
    
   * Cliente con Modo puente
    
   ![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.7.png)
    
### 8. Comprobaciones

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.8.1.png)

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.8.2.png)
