# Acerca de 
El labstreaminglayer es una herramienta desarrollada por el Swartz Center for Computational Neuroscience de la Universidad de California en San Diego con la intención de unificar los método de recolección de series temporales. El sistema fue desarrollado con el motivo en mente de desarrollar aplicaciones y experimentos para el area de BCI. El sistema se encarga de crear una red de transimisión de series temporales, así como de sincronizar eventos y proveer de acceso quasi-real a los datos obtenidos de diferentes dispositivos y sistemas. Para más información, referirse al [sitio de alojamiento del paquete.](https://github.com/sccn/labstreaminglayer)
El motivo de este documento consiste en presentar instrucciones paso a paso sobre como instalar el LSL y sus componentes dentro de los entornos Windows y macOS. 

## Instalación en Windows.
###### Requerimentos 
 - [Visual Studio 2019](https://visualstudio.microsoft.com/es/downloads/)
 - [CMake](https://cmake.org/download/)
 - [Git](https://git-scm.com/downloads) 
 - [OpenBCI_LSL](https://github.com/OpenBCI/OpenBCI_LSL) Una vez instalado git, se debe poner git clone link, para poder tener el repositorio en la computadora.
 - [Python](https://www.python.org/downloads/) Solo es necesario si no lo tienes instalado.
 
 La instalación especificada en este documento solamente comprende el build de la librería liblsl y no la de las múltiples aplicaciones. Más adelante se añadirán los detalles necesarios.
 
Una vez teniendo instalado esto se debe seguir lo siguiente en cmd de la computadora.
## Instalacione en python.
###### Siempre empezar con pip install -:
- pylsl
- pyserial
- numpy
- pyqtgraph
- scipy

##  Conectar y correr OpenBCI_LSL
#### Entrar al centro de comando de la computadora (cmd)
Para poder correr el programa deberás asegurarte de dondé está instalado el OpenBCI_LSL. Para poder correr esto el cmd deberá estar ubicado en el lugar del documento si es necesario cambiar de dirección se escribe cd: Lugaraelegir. Después de esto deberás poner OpenBCI/OpenBCI_LSL le das enter, después debes poner python openbci_lsl.py --stream, en caso de que depués de dar click te da un error, deberás olver a escribir python openbci_lsl.py [Port] --stream. Para saber que puerto esta usando el openbci, puedes entrar en panel de control> Hardware y sonido> Administrador de dispositivos> dispositivo conectado
Aqui podria aparecer USB o COM, comunmente el dispositivo cuenta con 2 puertos por lo que puede ser COM2/COM3 ó USB1/USB2
Entonces se puede escribe 
python openbci_lsl.py com2/3 --stream

 



