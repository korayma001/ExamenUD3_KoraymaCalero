# ExamenUD3_KoraymaCalero

## Migracion de nuestra web a un hostig

![AWARDSAPACE](/img/awardspace.png)

### Explicamos paso a paso como hacerlo 

* 1. Primero buscaremos nuestro hosting en nuestro caso [www.awardspace.com](www.awardspace.com) en el cual iniciaremos sesion.

* 2. Creamos nuestro subdominio ya que nos lo permite de forma gratuita.
  
* 3. Configuraremos el FTP dandoloe un usuario y contraseña, en mi caso **FileZilla**.
Tras hacer a configuración nos descargaremos un fichero el cual tendra nuestra informacion de inicio de sesión el cual importaremos a nuestro cliente <u>FileZilla</u>

* 4. Una vez hayamos accedido desde FileZilla lo que haremos será subir todo el contenido de nuetrs web a hostear en la raiz, **No en una carpeta si no los ficheros** es decir si ca configuración de neusro *Worpress* esta en la carpeta worpress pondremos todos los fichero y carpetas quee estan dentro de el.

* 5. Crearemos una base de datos destro de nuestro hosting donde importaremos la base de datos exportada de nuestro localhost
  
* 6. Editamos el fichero ***wp_congig.php*** indicandole la nueba base de datos, el usuario, el host donde se encuenta y demas configuracones de seguridad como cambier los prefijos de la tabla
``` php
    $table_prefix = 'kcr_';
```
o la no edicion de ficheros php por cualquier usuario.

* 6. Una vez subido los ficheros y configurado la base de datos, accederemos al sumbdominio creado y veremos la pagina principal de nuestra web. 

AParetir de ahora Todas las configuraciones se haran desde nuestro hosting que ya es ajeno a nuestro localhost 

