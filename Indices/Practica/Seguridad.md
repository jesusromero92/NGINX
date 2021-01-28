# Seguridad
## Procedemos a instalar un certificado para que nuestro sitio web sea **seguro**

### Pasos

### 1. Creamos una carpeta para guardar los certificados,e instalamos el paquete para crear los certificados
Nos pedirá una frase,introducimos la que nosotros queramos,pero debemos recordarla

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.1.png)

### 2. Generamos la clave privada con la más tarde cifraremos el certificado

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.2.png)

### 3. Generamos el certificado *aun sin firmar*
   Rellamos los datos y es **importante introducir correctamente el *FQDN***
   
![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.4.png)

### 4. Firmamos el certificado con la clave privada que generamos antes
Debemos introducir la frase que pusimos en la clave privada

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.5.png)

### 5. Debemos tener los siguientes archivos:

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.9.png)

### 5. Configuramos el sitio virtual de la siguiente manera para activar la navegación segura

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.8.png)

### 6. Comprobamos que la configuración es correcta

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/5.6.png)

### 7. Comprobaciones

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.6.png)

![](https://github.com/jesusromero92/NGINX/blob/main/Fotos/9.7.png)

