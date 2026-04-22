# Parcial Ucompensar

## Elaborado por 
- Karen Jhojana Camacho Castellanos
- Edwin Soto Escarraga
- Diego Esteban Lopez Rico

  # Parte conceptual
- ¿Cual es la diferencia entre las diferentes topologías de RAID?, explique con un esquema cada arquitectura y su funcionamiento.



- ¿Qué es docker? Y ¿Qué es una máquina virtual?, comentar las características arquitectura de cada una, además de sus diferencias y aplicaciones.
  
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

- Exponer el paso a paso de creación de un archivo por medio de un terminal de Ubuntu, donde se cree un directorio, luego un archivo donde se escriba algo, se modifique, luego se mueva de carpeta y se elimine la carpeta que queda vacía.
  ## Solución
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








  
  
- Desarrollar la configuración del PCO y del PC6 para que tenga internet.
Adicionalmente configurar los switchs 1 y 2, con el router.

- ¿Cuáles son los pasos para crear el repositorio remoto, sincronizar, clonar ese repositorio a nivel local, para luego subir información y corroborar su estado a través de la terminal de github bash?
- Si yo quiero crear una máquina virtual de Ubuntu en el pc 1, qué debo seguir para crearla?

# Parte empirica 

- Diseñe una red que tenga cuatro vlans, dos vlans en cada switch que luego van conectados a un router, exponga el paso a paso de configuración y haga:

- Esquema de la topología de red.
  
- Desarrollo de los comandos a utilizar
  
- ¿Como se verifica que las subredes tengan conexión entre ellas?
  
- Si yo quiero ver la tabla mac, las ip y vlans qué comandos debo usar?
  
- Si yo quiero tener una copia de seguridad en los servidores. ¿Qué raid me recomienda para la red? Y ¿Por qué?
  
- Será que es bueno comprar cpu, gpu y tpu para cada una de mis sub-redes si la primera es para diseño gráfico, la segunda para recursos humanos, la tercera para físicos y matemáticos y la cuarta para el área TIC?. ¿Qué tecnologías debería usar cada equipo?
