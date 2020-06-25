# Tutorial-MaquinaVirtual-Google-Cloud


 TUTORIAL DE COMPUTE ENGINE: VIRTUAL MACHINES (VMS) | GOOGLE CLOUD, PARA GENERACIÓN DE MÁQUINAS VIRTUALES.

1)	OBJETIVOS 

	a)	Analizar las herramientas que nos ofrece Google Cloud para generar maquinas virtuales. 
	b)	Comprender el procedimiento correcto para crear una máquina virtual, respecto a las necesidades requeridas. 

2)	MARCO TEÓRICO 

¿Qué es Google Cloud?

Google Cloud (Nube de Google) es una plataforma que ha reunido todas las aplicaciones de desarrollo web que Google estaba ofreciendo por separado. Es utilizada para crear ciertos tipos de soluciones a través de la tecnología almacenada en la nube y permite por ejemplo destacar la rapidez y la escalabilidad de su infraestructura en las aplicaciones del buscador.
Google Cloud se refiere al espacio virtual a través del cual se puede realizar una serie de tareas que antes requerían de hardware o software y que ahora utilizan la nube de Google como única forma de acceso, almacenamiento y gestión de datos.
Google ofrece una variedad de servicios basados en la nube. Google Cloud Print permite imprimir desde la web, el escritorio o dispositivo móvil sin la necesidad de un sistema operativo en particular o controladores. En su lugar, envías el documento a cualquier impresora conectada a la nube. Google también ofrece espacio en la nube para desarrolladores de bases de datos SQL para crear aplicaciones, así como para los usuarios de Microsoft Office que deseen editar colaborativamente documentos de Word, PowerPoint y Excel, sin necesidad de la utilización de un cliente local

Recursos de GCP


GCP consta de un conjunto de recursos físicos, como computadoras y unidades de disco duro, y virtuales, como las máquinas virtuales (VM), que se encuentran en los centros de datos de Google de todo el mundo. Cada centro de datos está ubicado en una región. Las regiones están disponibles en Asia, Australia, Europa, América del Norte y América del Sur. Cada región es una colección de zonas aisladas entre sí dentro de cada región. Las zonas se identifican mediante nombres que combinan una letra identificadora con el nombre de la región. Por ejemplo, la zona a en la región de Asia Oriental se llama asia-east1-a.

Esta distribución de los recursos brinda varios beneficios, incluida redundancia en caso de fallas y menor latencia, ya que los recursos se encuentran más cerca de los clientes. La distribución también presenta algunas reglas sobre cómo se pueden usar los recursos en conjunto.

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/1.%20RECURSOS%20GSP.png)

 

Características que ofrece Google Cloud. 

•	Adopta entornos de nubes híbridas o múltiples sin depender de un solo proveedor
Compila tus aplicaciones solo una vez y ejecútalas en entornos de nubes híbridas o múltiples nubes con otros proveedores de 
servicios.

•	Moderniza tus cargas de trabajo en una infraestructura de primer nivel
Realiza migraciones con rapidez gracias a las soluciones de infraestructura de nube empaquetadas previamente para SAP, VMware, Windows, Oracle, migración de centros de datos y otras cargas de trabajo empresariales.

•	Protege tus datos con seguridad de varias capas
La infraestructura con diseño de seguridad integral protege tus datos, aplicaciones y usuarios mediante funciones avanzadas de detección de amenazas y herramientas potentes para combatir el software malicioso.


•	Impulsa la toma de decisiones con estadísticas inteligentes

Un conjunto de soluciones escalables para almacenes de datos, análisis, IA y aprendizaje automático te permiten descubrir estadísticas prácticas a partir de tus datos.

3)	DETALLES DE LICENCIA OBTENIDA 

Se obtuvo la licencia de Google Cloud Platform Gratuita, la cual nos proporciona los siguientes beneficios: 

•	Acceso a todos los productos de Cloud Platform
Consigue todo lo que necesitas para desarrollar y ejecutar tus aplicaciones, sitios web y servicios, incluidos Firebase y la API de Google Maps.

•	Crédito de 300 USD gratuito
Regístrate y consigue 300 $ para gastarlos en Google Cloud Platform durante los próximos 12 meses.

•	Sin cargos automáticos después del periodo de prueba gratuito
Solo te pedirá los datos de tu tarjeta de crédito para comprobar que no eres un robot. No se te cobrará nada a menos que actualices la cuenta de forma manual a una versión de pago.

CONDICIONES DE USO DE LA LICENCIA GRATUITA 

La prueba gratuita solo se aplica al uso de los Servicios.

Solo los nuevos clientes de Google Cloud Platform son elegibles para participar en la Prueba gratuita.

La Prueba gratuita comienza cuando el Cliente crea una cuenta de facturación en Google Cloud Console ("Fecha de inicio de la Prueba gratuita") y finaliza antes de (i) la fecha en que las tarifas de uso del Cliente exceden los $ 300 o (ii) 12 meses a partir del Fecha de inicio de prueba gratuita.


LIMITACIONES DE USO DE LA LICENCIA GRATUITA 

El uso de Google Compute Engine por parte del cliente está restringido a solo ocho núcleos de uso concurrente por prueba gratuita (como se describe más detalladamente en la Documentación).

El cliente no puede usar los Servicios para participar en la minería de criptomonedas.
Ciertos servicios y funciones no estarán disponibles en la versión de prueba gratuita, como se indica en Google Cloud Console; y los SLA no se aplican.

4)	TUTORIAL DE REGISTRO EN GOOGLE CLOUD 

a)	Ingresaremos a google Cloud, ahí accedemos a la pestaña comenzar gratis. 
	Link: https://cloud.google.com/

 
b)	Una vez ingresemos se nos solicitara que iniciemos sección en Google, pidiendo nuestro correo como nuestra contraseña. 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/2.1%20REGISTRO%20GOOGLE%20CLOUD.png)

 
c)	Ingresada a la cuenta nos solicitara que aceptemos las condiciones del servicio, como también nos solicitara información personal como nuestros nombres y residencia, el tipo de cuenta que se va a usar (Particular o de empresa). También será necesaria Ingresar un método de pago como una tarjeta, esto para comprobar que no somos bots. Podemos encontrar más información en condiciones del sistema. 
	Link: https://cloud.google.com/terms/free-trial/?_ga=2.143533493.-1204134252.1591333727&_gac=1.15393666.1591335662.EAIaIQobChMI8rTho_vp6QIVCbSzCh2dpwGJEAAYASAAEgI7Q_D_BwE

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/2.2%20REGISTRO%20GOOGLE%20CLOUD.png)

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/2.3%20REGISTRO%20GOOGLE%20CLOUD.png)


 
 

d)	Finalmente, una vez ingresados todos los datos le damos a “INICIAR PRUEBA GRATUITA”. 
  							
	
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/2.4%20REGISTRO%20GOOGLE%20CLOUD.png)



5)	TUTORIAL DE CREACIÓN DE LA MÁQUINA VIRTUAL 

	a)	Una vez nos encontramos en la consola principal, ingresaremos a la pestaña “Menú de navegación”. Seleccionaremos “Compute Engine” y se nos abrirá otra pestaña en la cual seleccionaremos “Instancias de VM”

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)

 


	b)	Nos mostrara la siguiente pantalla, a lo cual seleccionáremos “Crear”.

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.1%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)

 
	c)	Aquí inicia el proceso de detalles de nuestra máquina virtual. 

i)	Primero será necesario ingresar un nombre a nuestro equipo. 

ii)	Colocaremos la región en la cual se va a encontrar los servidores de alojamiento de nuestra máquina virtual. 
 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.2%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)

iii)	En la tercera ventana se seleccionarán las características de nuestra máquina virtual. Como el tipo de maquina disponibles. 
 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.3%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)

d)	Seleccionaremos el disco de arranque de la máquina virtual.
 
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.4%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.5%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)
  
e)	Una vez seleccionado todos los detalles de nuestra máquina virtual “Creamos” esta mencionada, tomara alrededor de un minuto. 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.6%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/3.7%20REGISTRO%20M%C3%81QUINA%20VIRTUAL.png)

 

 



6)	PROCESO PARA INICIAR E INGRESAR A NUESTRA MÁQUINA VIRTUAL MEDIANTE CONEXIÓN REMOTA.


	a)	Una vez nos encontramos en la ventana principal de “Instancias VM”, observamos la maquina antes creada. 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

 
	b)	Sera necesario almacenar algunos datos para su posterior uso. 

i)	Es necesario almacenar la ip externa 

ii)	Sera necesario tener la contraseña, o en todo caso se deberá restablecerla, para hacer esto se deberá elegir en la pestaña “RDP”, ver comando gcloud para restablecer la contraseña

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.1%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

 
iii)	Se mostrará las siguientes ventanas, en la cual podremos modificar el nombre de usuario y nos entregará una contraseña aleatoria. 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.2%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.3%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

  

c)	 Con los datos antes mencionados, abrimos “Remote Desktop Connection”.

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.4%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

 
d)	Al abrir este programa, nos solicitara la ip externa.
 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.5%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)


e)	La siguiente ventana nos solicitara el nombre de usuario y la contraseña antes adjudicada. 

![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.6%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.7%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

 
 
f)	Finalmente, nos mostrara nuestra máquina virtual. 

 
![]( https://github.com/JorgeCruzV/Tutorial-MaquinaVirtual-Google-Cloud-/blob/master/Imagenes/4.8%20INICIAR%20M%C3%81QUINA%20VIRTUAL.png)

7.- CONCLUSIONES:

Se evidencio lo útil que podrían a llegar a ser este tipo de máquinas virtuales, debido a que nos brindan una gran posibilidad de crear servidores, o maquinas personales y poder usarlas desde cualquier lugar, siendo como requisito que la maquina donde se va a trabajar tenga una conexión a internet. 

Mediante la comparación entre google cloud y Microsoft Azure, se evidencio una mayor libertad de trabajo y acciones en Microsoft Azure. Aunque las dos cuentan con una infinidad de herramientas.

Posiblemente en un futuro este tipo de herramientas sigan mejorando, debido a que las conexiones de internet son cada vez mejores, mejorando la conexión con el usuario. Incluso se tiene la perspectiva a futuro que puedan ser usadas como consolas de videojuegos, siendo los computadores virtuales maquinas con las características necesarias, esto se lograra siempre y cuando las conexiones a internet mejoren contundentemente.

Se podria 

8.- BLIBLIOGRAFÍA

Emprendices (26 de octubre de 2014). Recuperado de ”https://www.emprendices.co/que-es-google-cloud-platform/.

Google Cloud(Last updated 2020-05-26.) Recuperado de “https://cloud.google.com/docs/overview?hl=es-419”



