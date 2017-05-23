# DAWF (DragonJAR Automatic Windows Forensic)

DAWF (DragonJAR Automatic Windows Forensic) es el nombre que se le ha dado a una herramienta que automatiza la extracción de evidencia forense en Windows, (de la que hablamos hace un tiempo) pensada inicialmente para resolver una necesidad concreta que teníamos en un proceso forense y que ha resultado muy útil en otros procesos similares, por tal razón la hacemos pública.


Definimos DAWF como una herramienta DE BOTÓN GORDO, pensada para los siguientes entornos:

    Entorno Windows Vivo
    (Encendido, con procesos corriendo y en el cual debemos ejecutar lo mínimo necesario para extraer la memoria RAM y la información del sistema)
    
    Entorno Windows Revivido
    (Cuando tomamos una copia bit a bit, siguiendo toda la metodología del caso y ya con nuestro segundo original en manos, montamos esa imagen en una máquina virtual para “revivir” el equipo en un entorno controlado sin temor a modificar la evidencia)

Si lo ejecutas en un Entorno Vivo sin seleccionar la opción (“Dumpear solo la RAM y SisInfo”) estarías ejecutando una gran cantidad de procesos en esta máquina y posiblemente alternado la evidencia, pero debes determinar en cada caso puntual si puedes hacerlo o tienes autorización para ello.

DAWF-2
Por ejemplo en casos en los que NO se busca llevar a un tribunal lo sucedido y solo es necesario identificar por ejemplo la fuente de infección de un malware o los equipos involucrados en una fuga de información posiblemente no tengas problema con ejecutar la herramienta “en vivo”, pero cada caso debe ser evaluado.

Las funcionalidades del DAWF son las siguientes:

    Herramienta de BOTÓN GORDO:
    Está pensada para que sin importar si lo ejecuta una secretaria sin idea de computación, o el jefe de sistemas de una organización, ambos lleguen al mismo resultado, la herramienta exige ejecución como administrador y si por descuido o error no presionan el BOTÓN GORDO, el DAWF inicia sus labores automáticamente.
    
    Documenta Cada Acción Realizada:
    La herramienta documenta cada paso que da, con fecha y hora precisa, genera también las firmas de los archivos creados en 6 formatos distintos de hash para evitar cualquier tipo de colisión, lo que será muy útil a la hora de generar nuestro informe forense.
    
    Funciona en Entornos Muertos y Vivos:
    Tiene una opción para solo sacar la memoria RAM y la información del sistema cuando tenemos un entorno vivo y la opción principal de extraer toda la información para ejecutar en entornos “muertos” que han sido “revividos”.
    
    Portabilidad:
    La herramienta está pensada para ser ejecutada desde un medio de almacenamiento externo debidamente sanitizado y solo generar archivos nuevos en este medio, evitando tocar el equipo analizado y adaptándose a cualquier ruta donde se encuentre el ejecutable.
    
    Compatible con Windows XP-10:
    La herramienta es compatible con todas las versiones de Windows desde XP hasta Windows 10 y las aplicaciones integradas fueron cuidadosamente seleccionadas para que esto fuera posible (con un periodo de pruebas publico bastante positivo).
    
    Parametrizable y Personalizable:
    La herramienta puede ser ejecutada directamente en sus 2 modos, siempre y cuando se ejecute como administrador con las siguientes opciones “DAWF.exe /vivo” para extraer la RAM y la información del sistema y “DAWF.exe /muerto” para ejecutar la funcionalidad principal de extracción de información automatizada; Adicional a esto se incluyen diferentes perfiles específicos para extraer información concreta, como información de navegación, ejecución y manipulación de archivos o redes sociales y permite generar nuestros propios perfiles personalizando aún más la herramienta (Leer archivo “DAWF\Herramientas\1. Cambiar o Crear Perfiles.txt” ).
    
    Visual y Fácil de Entender:
    Todo analista forense que lleve un tiempo haciendo su trabajo posiblemente tenga un script en BAT que haga algo parecido a lo que se está presentando, pero algo que siempre da impotencia con este tipo de scripts es que no sabes cuánto va a tardar o en qué paso estamos en un momento determinado, con DAWF no pasa esto ya que supervisa constantemente cada proceso en ejecución y nos indica cual se está corriendo actualmente además de mostrar en una barra de progreso cuánto nos falta para terminar el proceso.

Esto es todo lo que ofrece el DAWF, como pueden ver es un software muy simple pero que cumple con su labor, el mayor aporte que hace DAWF no es tanto el programa como tal, sino la selección de herramientas que incluyen y que fueron puestas a prueba en casos reales.

Más Información:
http://www.dragonjar.org/dawf-dragonjar-automatic-windows-forensic.xhtml
