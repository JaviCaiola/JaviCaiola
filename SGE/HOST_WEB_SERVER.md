# CREAR SERVIDOR WEB CON IIS (FRONT END):    
##Con dominio:    
 ip publica : *https://www.cual-es-mi-direccion-ip.com/**    
https://www.cualesmiip.com/    
https://nordvpn.com/es/what-is-my-ip/  :   
DNS REMOTA: https://www.cloudflare.com/es-es/plans/free/     
https://www.domain.com/
     

desde el gestor de dominio configurar el apartado del DNS para que apunte a la ip Publica de nuestra red

CONFIGURAR DNS EN SERVER MANAGER:
pestaña de herramientas, seleccionar DNS.   
luego crear una nueva zona de busqueda con click derecho en la carpeta.    
crear la paridad entre la direccion ip y el nombre de la web. asignando el dominio.    
luego desde iis dirigirse al proyecto en publicacion, en el dashboad derecho seleccionar la opcion 'enlaces', y cambiar el puerto establecido

CREACION DE SERVIDOR PRIVADO.

SERVER MANAGER
INTERNET INFORMATION SERVICE (IIS).
-Configuracion de medidas de Seguridad.
-Congiguracion de complementos necesarios para el host de aplicacion web.
-Establecer DNS.

1. **Instalación de Internet Information Services (IIS):**
   - "Panel de control" > "Programas" > "Programas y características".
   - clic en "Activar o desactivar las características de Windows".
   - Seleccionar "Servicios de Internet Information Services" y marcar todas las opciones que necesitas (por ejemplo, "Servidor web (IIS)" y sus características).

2. **Abrir IIS:**
   - Una vez instalado, abre el Administrador de IIS. buscar "Administrador de Internet Information Services (IIS)" en el menú de inicio o ejecutar `inetmgr` en el cuadro de búsqueda de Windows.

3. **Crear un nuevo sitio web:**
   - En el Administrador de IIS, expande el nombre de tu computadora en el panel izquierdo.
   - Haz clic derecho en "Sitios" y selecciona "Agregar sitio web".
   - Se abrirá un asistente. Ingresa un nombre para tu sitio web, por ejemplo, "MiSitioWeb".
   - Especifica la ruta física donde estarán los archivos del sitio web.
   - Asigna un número de puerto (por ejemplo, 80 para HTTP estándar).
   - Opcionalmente, puedes asignar una dirección IP específica o dejar que sea "Todas no asignadas".
   - Configura otros ajustes según tus necesidades y finaliza el proceso.

4. **Configuración adicional (opcional):**
   - Puedes ajustar la configuración de tu sitio web, como la autenticación, la dirección IP, los certificados SSL, entre otros, desde el Administrador de IIS.

5. **Prueba tu sitio web:**
   - Abre un navegador web e ingresa la dirección IP de tu máquina seguida por el número de puerto que asignaste al sitio web (por ejemplo, `http://localhost` o `http://localhost:80`).

Estos pasos básicos te permitirán configurar un sitio web local utilizando IIS en Windows. Recuerda que los detalles pueden variar dependiendo de tus necesidades específicas y la versión de Windows que estés utilizando.    

MAS DOMINIOS
Freenom: Ofrece dominios gratuitos con extensiones como .tk, .ml, .ga, .cf, .gq. Sin embargo, estos dominios gratuitos pueden tener ciertas restricciones y a veces se utilizan para redireccionar tráfico a páginas publicitarias.

Dot.tk: Es parte de Freenom y ofrece dominios con extensión .tk de forma gratuita.

InfinityFree: Ofrece servicios de alojamiento web gratuito y también proporciona dominios gratuitos con extensiones .epizy.com o .rf.gd para sus clientes.


