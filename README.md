# Parcial Ucompensar

## Elaborado por 
- Karen Jhojana Camacho Castellanos
- Edwin Soto Escarraga
- Diego Esteban Lopez Rico

  # Parte conceptual
- ¿Cual es la diferencia entre las diferentes topologías de RAID?, explique con un esquema cada arquitectura y su funcionamiento.

#### Raid 
Sigmifica "Redundant Array of Independent Disks" es la combinacion de varios discos duros para mejorar aspectos tales como 

- Velocidad
- Seguridad
- Ambas

#### Tipos de RAID 

#### 1. RAID 0 (Striping)

Divide los datos en bloques y los reparte entre varios discos 

#### Funcionamiento:

Los archivos se parten y se escriben en paralelo.
 
#### Características:

- Muy rápido

- No tiene redundancia

- Si falla un disco → Se pierde la información

#### Uso:
- Edición de video
- Juegos
- Procesos donde importa la velocidad

#### 2. RAID 1 (Mirroring)

Duplica la información en dos discos

#### Funcionamiento:

Todo lo que se escribe en un disco, se copia en el otro.

#### Características:
- Alta seguridad

- Baja capacidad útil (se duplica todo)

- Lectura rápida, escritura normal
  
 #### Uso:
 
- Sistemas críticos
  
- Bases de datos pequeñas

#### 3. RAID 5 (Paridad distribuida)

Combina velocidad + tolerancia a fallos 

#### Funcionamiento:

- Los datos se distribuyen

- Se agrega información de paridad (permite recuperar datos si falla un disco)

#### Características:

- Buen rendimiento
  
- Soporta fallo de 1 disco

- Uso eficiente del espacio

- Escritura un poco más lenta

#### Uso:
- Servidores

- Empresas

#### 4. RAID 10 (1+0)

Combinacion del RAID 1 + RAID 0

#### Funcionamiento:

- Primero se duplican los datos (RAID 1)

- Luego se distribuyen (RAID 0)

#### Características:

- Muy rápido
- Alta tolerancia a fallos
- Costoso (necesita más discos)
#### Uso:

- Sistemas críticos de alto rendimiento

- Bases de datos grandes

#### Resumen 

RAID 0 → máximo rendimiento, sin protección

RAID 1 → máxima seguridad, duplicación

RAID 5 → equilibrio entre rendimiento y seguridad

RAID 10 → alto rendimiento + alta seguridad


- ¿Qué es docker? Y ¿Qué es una máquina virtual?, comentar las características arquitectura de cada una, además de sus diferencias y aplicaciones.
  
#### Docker

El docker es una plataforma que sirve para crear y ejecutar contenedores
Un contenedor es un tipo de aplicación que contiene todo lo que necesita para hacer funcionar un sistema tales como (Código, librerías, dependencias) Cabe aclarar que este no incluye un sistema operativo completo

#### Componentes clave Docker:
- Docker Engine → motor que gestiona los contenedores
  
- Contenedores → donde corre la app

- Imágenes → plantillas para crear contenedores

- Docker Hub → repositorio de imágenes

#### Aplicaciones de Docker:

- Desarrollo de software

- Microservicios

- DevOps y CI/CD

- Despliegue rápido de apps

#### Máquina virtual

Una maquina virtual (VM = Virtual machine) Es una emulación completa de un computador con su respectivo sistema operativo Se ejecuta sobre un software llamado hipervisor.
Ejemplo de software: VirtualBox, VMware

#### Características de las VM:
- Aislamiento completo

- Cada VM tiene su propio sistema operativo

- Más seguras (a nivel de aislamiento)

- Consumen más recursos

- Arranque más lento


#### Aplicaciones de las VM

- Ejecutar distintos sistemas operativos

- Pruebas de software

- Servidores empresariales

- Seguridad informática

#### Diferencias clave: 

<img width="492" height="168" alt="image" src="https://github.com/user-attachments/assets/b79de902-9a27-4b0d-8a3d-1b79924a19da" />

#### Resumen:

#### Docker: Ejecuta aplicaciones en contenedores ligeros compartiendo el mismo sistema operativo

#### Máquina virtual: Simula un computador completo con su propio sistema operativo

- ¿Cuáles son las capas del modelo OSI?. Explicar cada una y dar ejemplos rea
de aplicación
## Modelo OSI 
#### Aplicación:
Interfaz directa con el usuario final (navegadores, correo).

#### Presentación: 
Traduce, cifra y comprime los datos para asegurar su legibilidad.

#### Sesión: 
Gestiona y controla las conexiones (inicia, mantiene y finaliza) entre dispositivos.

#### Transporte:
Asegura la transferencia de datos de extremo a extremo, controlando flujo y errores.

#### Red:
Determina el mejor camino (enrutamiento) para los datos a través de diferentes redes.

#### Enlance de datos:
Detecta y corrige errores físicos, gestionando el direccionamiento físico (MAC).

#### Física: 
Transmite bits puros a través de cables, fibra o radiofrecuencia.


<img width="382" height="471" alt="image" src="https://github.com/user-attachments/assets/4d3abde7-d055-477f-8379-6a3b5f4fa6ff" />

### Cita 
Josan, M. (2021, enero 15). Modelo de capas OSI y TCP/IP. Curso de redes dede 0. NASeros. https://naseros.com/2021/01/15/modelo-de-capas-osi-y-tcp-ip/


- ¿Cuáles son los tipos de nube?. Explicar cada uno y exponer sus respectivas características y un diagrama sencillo de funcionamiento.

#### Nube publica

Se accede por medio de internet, la más común algunas como Amazon Web Services, Microsoft Azure, Google Cloud Platform

#### Características:

- Acceso desde cualquier lugar con internet

- Pago por uso (tipo suscripción o consumo)

- Escalable (subes o bajas recursos fácilmente)

- No necesitas mantener hardware

- Compartida entre múltiples usuarios

#### Nube privada 

Esta se le ve más en entornos como empresas o en cierto proveedor 

#### Características:
- Mayor control y seguridad

- Personalización total

- Más costosa

- Requiere gestión técnica

- Ideal para datos sensibles

#### Nube Híbrido 

La mezcla entre la nube pública + nube privada.

Depende de que quiera la empresa usar. 

#### Características:

- Flexibilidad total

- Permite mover datos entre entornos

- Balance entre seguridad y escalabilidad

- Más compleja de gestionar

#### Nube comunitaria 
La menos comun, varias empresas comparten los intereses en esta nube empresas o lugares como Hospitales, Universidades, Entidades gubernamentales

#### Características:

- Compartida entre organizaciones

- Costos distribuidos

- Seguridad enfocada en un sector específico

- Menos flexible que la pública
  
# Parte de diseño
- ¿Cuáles son las partes de un computador? Hacer un dibujo y explicarlas.
Parte de Diseño
- Desarrolle el parcial en un repositorio de github y anexe la información solicitada
paso a paso.

- Analice Y observe la siguiente ecuación

<img width="543" height="69" alt="image" src="https://github.com/user-attachments/assets/8ddee2ed-b870-4eb0-a234-8a50e2a533a2" />


obtener lo siguiente:
Dibujar el circuito

<img width="1843" height="1050" alt="image" src="https://github.com/user-attachments/assets/7d2c2353-ecde-4669-b44f-f0c0546c7968" />

Desarrollar tabla de verdad a partir de la ecuación


# Desarrollar

## Exponer el paso a paso de creación de un archivo por medio de un terminal de Ubuntu, donde se cree un directorio, luego un archivo donde se escriba algo, se modifique, luego se mueva de carpeta y se elimine la carpeta que queda vacía.
  ### Solución
  ### Creación de directorios
  - Se creó un directorio principal llamado Practica_Linux y dentro de este los subdirectorios Documentos y Backup.
    
    mkdir → crear carpetas
    
    cd → ingresar a un directorio
    
    <img width="921" height="88" alt="image" src="https://github.com/user-attachments/assets/3652db77-9537-4e86-86ea-f51db5d4648c" style="margin-bottom:10px;" />

  ### Creación y edición de archivos
  - Se creó un archivo de texto y se editó con contenido usando el editor nano.
    
    touch → crear archivos
    
    nano → editar archivos
    
    <img width="921" height="94" alt="image" src="https://github.com/user-attachments/assets/74e27e0f-da3f-4785-895c-00cd5e63606f" style="margin-bottom:10px;" />
    <img width="920" height="132" alt="image" src="https://github.com/user-attachments/assets/4c5e69eb-20b9-4584-993c-8bce0f7130d0"  />
    
  ### Copia y renombrado de archivos
  - Se realizó la copia de un archivo y posteriormente su cambio de nombre.
    
    cp → copiar archivos
    
    mv → mover o renombrar
    
    <img width="921" height="68" alt="image" src="https://github.com/user-attachments/assets/a4900151-9bcf-497a-9a11-3b954a3eac58" /> <br>
    <img width="921" height="280" alt="image" src="https://github.com/user-attachments/assets/a6754f41-9825-46b8-a56a-10e341e48da2" /><br>

  ###  Eliminación y permisos
  - Se eliminaron directorios, se visualizó contenido y se modificaron permisos de acceso.
    
    rm -r → eliminar carpetas
    
    cat → ver contenido
    
    chmod → cambiar permisos
    
    ls -l → ver detalles
    
    <img width="921" height="327" alt="image" src="https://github.com/user-attachments/assets/6ae5540a-e2e1-4d56-b932-b2ef69dabb2d" /> <br>
  ### Búsqueda de archivos y contenido
  - Se realizaron búsquedas de archivos y palabras dentro de ellos.
    
    find → buscar archivos
    
    grep → buscar texto
    
    <img width="921" height="161" alt="image" src="https://github.com/user-attachments/assets/ebc551ba-0e01-4c7c-b7ec-22d0d638c414" /> <br>
  
## Desarrollar la configuración del PCO y del PC6 para que tenga internet. Adicionalmente configurar los switchs 1 y 2, con el router.
### Solución y explicación de la configuración de red
<img width="381" height="360" alt="image" src="https://github.com/user-attachments/assets/ea897f65-a436-4a51-aa83-db5aa5aa02bd" />

  ### Configuración de PC0 (PC0)
  - IP Address: 192.168.10.2 255.255.255.0: Define la dirección única del equipo dentro de la red.
  - La máscara indica que pertenece a la red 192.168.10.0.
  - Default Gateway: 192.168.10.1: Es la puerta de enlace. Permite que el PC se comunique con otras redes (como Internet).
  - DNS: 8.8.8.8: Servidor que traduce nombres de dominio (como google.com) a direcciones IP.
    
    <img width="848" height="870" alt="Captura de pantalla 2026-04-25 103535" src="https://github.com/user-attachments/assets/15c29e64-01f0-4738-8fdd-49e12ed2a90c" /> <br>

    
  ### Configuración de PC1

  - IP Address: 192.168.20.2 255.255.255.0: Dirección IP del equipo dentro de la VLAN 20.
  - Default Gateway: 192.168.20.1: Dirección del router para salir a otras redes.
  - DNS: 8.8.8.8: Permite resolver nombres de dominio.

    <img width="857" height="833" alt="Captura de pantalla 2026-04-25 103717" src="https://github.com/user-attachments/assets/d9aa7b62-788c-4a8d-9b22-40d44c25dc32" /> <br>


   ### Configuración del SWITCH 1 (SW1)
  - enable: Activa el modo privilegiado para poder configurar el switch.
  - configure terminal: Permite ingresar al modo de configuración global.
  - vlan 10: Crea la VLAN 10 en el switch. 
  - name VLAN10: Asigna un nombre a la VLAN para mejor identificación.
  - interface fa0/1: Selecciona el puerto donde está conectado el PC1.
  - switchport mode access: Configura el puerto como acceso (solo una VLAN).
  - switchport access vlan 10: Asigna ese puerto a la VLAN 10.
  - interface fa0/24: Selecciona el puerto que conecta al router.
  - switchport mode access
  - exit: Sale del modo actual.

    <img width="544" height="190" alt="image" src="https://github.com/user-attachments/assets/9aa3e27b-f1c4-40b8-ad6f-c933e55ae7cb" /> <br>

  
  ### Configuración del SWITCH 2 (SW2)
  - enable: Activa el modo privilegiado.
  - configure terminal: Modo de configuración global.
  - vlan 20: Crea la VLAN 20.
  - name VLAN20: Asigna nombre a la VLAN.
  - interface fa0/1: Puerto donde está conectado el PC6.
  - switchport mode access: Configura el puerto como acceso.
  - switchport access vlan 20: Asigna el puerto a la VLAN 20.
  - interface fa0/24: Puerto que conecta al router.
  - switchport mode access: 
  - exit: Salir del modo.

    <img width="574" height="163" alt="image" src="https://github.com/user-attachments/assets/12ef9b8c-e112-4e64-876a-c433f6bf2f7a" /> <br>

  
  ### Configuración del ROUTER 
  - enable: Activa modo privilegiado.
  - configure terminal: Modo configuración.
  - interface GigabitEthernet0/0: Selecciona la interfaz física conectada al switch.
  - no shutdown: Activa la interfaz (por defecto está apagada).
  - ip address 192.168.10.1 255.255.255.0: Asigna IP para servir como gateway de la VLAN 10.
  - interface GigabitEthernet0/1: Selecciona la interfaz física conectada al switch.
  - ip address 192.168.20.1 255.255.255.0: Gateway para la VLAN 20.
  - no shutdown: Activa la interfaz (por defecto está apagada).

    <img width="806" height="505" alt="image" src="https://github.com/user-attachments/assets/d7fd9327-2c9b-4985-8f0b-0fe7872e63dc" />

  
  ### Verificación de conectividad
  - ping 192.168.10.1: Prueba conexión entre PC1 y el router.
    
    <img width="473" height="203" alt="image" src="https://github.com/user-attachments/assets/d219ce6e-519d-4882-a1d8-f9cd3c548960" /> <br>

  - ping 192.168.20.1: Prueba conexión entre PC6 y el router.

    <img width="492" height="213" alt="image" src="https://github.com/user-attachments/assets/0f6bd568-2f18-4a0d-9a97-5b47e5a523d9" /> <br>



## ¿Cuáles son los pasos para crear el repositorio remoto, sincronizar, clonar ese repositorio a nivel local, para luego subir información y corroborar su estado a través de la terminal de github bash?
  ### Solución
  ### Crear repositorio remoto en GitHub
  1. Entra a GitHub
  2. Clic en "New repository"
  3. Nombre del repo (ej: mi-proyecto)
  4. Público o privado
  5. Clic en Create repository
  6. Al final se obtiene una URL
  ### Clonar el repositorio en local (Git Bash)
  1. git clone https://github.com/usuario/mi-proyecto.git
  2. cd mi-proyecto
  ### Crear o agregar archivos: Edita y escribe contenido.
  1. touch archivo.txt
  ### Ver estado del repositorio: Te muestra archivos modificados o nuevos.
  1. git status
  ### Agregar archivos al staging
  1. git add .
  2. específico: git add archivo.txt
  ### Hacer commit
  1. git commit -m "Primer commit"
  ### Subir cambios al repositorio remoto
  1. git push origin main
  2. Si existen ramas en el repositorio git push origin master
  ### Verificar estado después de subir
  1. git status
  ### Sincronizar
  1. git pull origin main
  
## Si yo quiero crear una máquina virtual de Ubuntu en el pc 1, qué debo seguir para crearla?
  ### Solución
  ### Paso inicial
  Abrimos Virtual Box
    <img width="680" height="712" alt="image" src="https://github.com/user-attachments/assets/51e5f69d-faf5-4b0a-8d89-3fa9fb062336" />
 ### Crear nombre y establecer ISO
  Le agregamos un nombre, tenemos que tener previamente la ISO de Ubuntu para que nos aparezca en "Type" = Linux y en version "Ubuntu(64-bit)"
      
  <img width="813" height="403" alt="image" src="https://github.com/user-attachments/assets/752d4509-7480-4797-8bac-04599befecf7" />
      
      
  ### Crear perfil de usuario
      
  Creamos el nombre de usuario y la respectiva contraseña, en "Hostname no permite guiones bajos, por esa razon tiene un guion"
      
  <img width="815" height="409" alt="image" src="https://github.com/user-attachments/assets/dc74e006-591a-45c5-9171-56076909e96f" />
      
  También se recomienda marcar la casilla de Guest Additions para instalar la imagen ISO predeterminada de Guest Additions que se descarga junto con VirtualBox. Guest     Additions habilita varias funciones que mejoran la experiencia de usuario, como el cambio de resolución y el redimensionamiento dinámico de la pantalla
      
  ### Recursos de la maquina virtual 
      
  En la siguiente imagen se evidencia como se establece los recursos de la maquina virtual, como es una simulacion corta no es necesaria usar tantos recursos del sistema, tambien depende del equipo con el que cuente el usuario
      
  <img width="815" height="404" alt="image" src="https://github.com/user-attachments/assets/ce969419-1f4b-4c46-b34a-45e396e189f1" />
      
   ### Resumen de la maquina virtual 
      
  A continuacion se evidencia el resumen de los recursos, nombres, ISO etc...
      
  <img width="818" height="409" alt="image" src="https://github.com/user-attachments/assets/a3f2e0da-bd7f-4452-a42d-ac0727b82a5a" />
      
  ### Inicio de la maquina 
      
  Nos arroja la siguiente interfaz, donde debemos darle clic en iniciar para comenzar la simulacion de nuestra maquina virtual en VB
      
  <img width="702" height="710" alt="image" src="https://github.com/user-attachments/assets/a0a78614-7cf5-4420-8777-93bbee3fd59a" />
      
  ### Instalacion de Ubuntu 
  No se debe interactuar con la maquina, ella misma comenzara el proceso de instalacion
      
  <img width="642" height="569" alt="image" src="https://github.com/user-attachments/assets/751b2087-9495-444e-b86e-2c31c30b1dab" /> <br>
      
  <img width="616" height="462" alt="image" src="https://github.com/user-attachments/assets/ce8fa526-a750-4271-8568-7230c6c98b6c" /> <br>
      
  <img width="606" height="462" alt="image" src="https://github.com/user-attachments/assets/2cacf7a1-9169-447c-970a-2d3c16dd446b" /> <br>
      
  <img width="625" height="483" alt="image" src="https://github.com/user-attachments/assets/d0035d69-28d1-462d-b1e7-c382137e722c" /> <br>

# Parte empirica 

- Diseñe una red que tenga cuatro vlans, dos vlans en cada switch que luego van conectados a un router, exponga el paso a paso de configuración y haga:

- Esquema de la topología de red.
  
- Desarrollo de los comandos a utilizar
  
- ¿Como se verifica que las subredes tengan conexión entre ellas?
  
- Si yo quiero ver la tabla mac, las ip y vlans qué comandos debo usar?
  
- Si yo quiero tener una copia de seguridad en los servidores. ¿Qué raid me recomienda para la red? Y ¿Por qué?
  
- Será que es bueno comprar cpu, gpu y tpu para cada una de mis sub-redes si la primera es para diseño gráfico, la segunda para recursos humanos, la tercera para físicos y matemáticos y la cuarta para el área TIC?. ¿Qué tecnologías debería usar cada equipo?
