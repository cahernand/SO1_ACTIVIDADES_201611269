### Actividad 1
- Nombre: Carlos Augusto Hernández Ordoñez
- Carnet: 201611269
- Fecha: 23/01/2023
- Tema: Tipos de kernel & sus diferencias
- User vs Kernel Mode



# Tipos de kernel
## Exonúcleos
Este tipo de kernel se denomina también sistema operativo verticalmente estructurado, simboliza un acercamiento nuevo y radical a la producción de sistemas operativos. La noción profunda es facilitar que el productor tome todas las decisiones vinculdas a la productividad del hardware.

Los exonúclos son muy diminutos, debido a que su funcionalidad se vincula únicamente al resguardo y el multiplexado de los materiales. Se denominan de esta forma debido a que toda la funcionalidad deja de estar presente en la memoria y pasa a estar en el exterior, en librerías activas.

## Micronúcleos
Consisten en núcleos de reducido tamaño que fueron generados solo con los requerimientos más sencillos del sistema operativo. Las demás funciones son agregadas a través de la suma de módulos exteriores al núcleo, lo que les otorga flexibilidad y permite la extensión. Se consideran más seguros que el kernel monolítico.

## Kernel de Poisson
El kernel de Poisson es un núcleo completo que se emplea para poder solucionar en dos extensiones el problema de Dirchlet. este tipo de kernel tiene su nombre debido al físico Siméon Poisson, quien nació en Francia.

## Núcleos monolíticos
Estas estructuras poseen un núcleo enorme y complicado, que abarca todos los servicios del sistema. Está diseñado de manera no modular,  y tiene un funcionamiento mayor que el micronúcleo.
Pero, cualquier modificación realizada en un servicio necesita un compendio del núcleo y el inicio del sistema para ejecutar nuevas modificaciones.

El sistema operativo con un kernel monolítico agrupa todas las funcionalidades probables (sistema de archivos, gestión de almacenamiento, reguladores de dispositios, entre otros) en el interior de una aplicación. El mismo puede tener una dimensión considerable, y deberá ser agrupado totalmente al agregar una funcionalidad nueva.

## Núcleos híbridos
Consiste en una estructura fundamentada en la unión de microkernel y el núcleo monolíico, dichos sistemas son emplados dentro de los ordenadores mediante los sistemas operativos.

Una cualidad esencial que tiene el núcleo híbrido es que insertan un código extra con el propósito de mejorar la productividad.

Al contrario de los núcleos monoliticos comunes, los controladores de ordenadores y las dimensiones al sistema operativo se puede descargar o cargar de forma fácil como si fueran módulos, mientras la estructura sigue funcionando sin inconvenientes.

De igual forma, al contrario del kernel monolítico tradicionl, es posible que los controladores sean prevolcados (retenidos de forma breve por ejercicios más esenciales) bajo diversas estipulaciones. Esta capacidad fua añadida para trabajar de forma apropiada las suspensiones de hardware, y para beneficiar la base del multiproceso propocionado.

## Kernel panic
Consiste en una actividad realizada por un sistema operativo al descubrir una equivocación interna grave de la que no puede librarse.

El vocablo es usado en especial en los sistemas UNIX. sin embargo, es posible que se observen en los sistemas MAC OSX. Una de las causas del kernel painc, e manifiesta cuando un sistema operativo trata de leer una dirección de almacenamiento incorrecto.


# User mode vs Kernel Mode
## user mode
Cuando un programa es iniciado en un isistema operativo, el programa se lanza en modo usuario, y cuando el corre un proceso en una dirección virtual de espacio, es creado por windows, el sistema, los programas de modo usuario tienen menos privilegios que u no tiene permitido el acceso directo a los recursos del sistema. Por consecuencia si una aplicación de modo usuario quiere acceder a los recursos del sistema, tendrá que primero ir a través del **kernel** del sistema operativo.

## kernel mode
es el corazón de un sistema operativo que permite conectar acceder al hardware directamennte, en todos los proceso debe correr un sistema, cuando administra las aplicaciones y componentes, la interacción del hardware y software entre si, cuando un programa corre bajo el modo usuario necesita acceder a la camara, tiene que hacerlo a través de un **syscall** y llevar esos cambios al CPU del usuario de nuevo, en tiempo de ejecución.

|Criterio | Kernel Mode | Usermode|
| -------  | -------------- | ----------- |
| kernel vs user |el programa tiene directa y no tiene restricciones para acceder al sistema operativo|el programa executa y e inicia|
|interrupciones| todo el sistema operativo viene abajo si una interrupción ocurre| un simple proceso falla si una interrupción ocurre|
|Modo| es conocido como master mode, privilgeciado o system mode| unpriviliged mode, restringido y esclavo modo|
|Virtual dirección| todos los procesos comparten una simple dirección de espacio| todo los procesos obtienen direcciones de espacio diferentes|
|nivel de privilgecios|las aplicaciones tiene más priviligecios| tienen menos privilegios|
|restricciones|ambos pueden acceder  los programas de usuario también los programas no tienen restricciones | necesita acceder al kernel directamente|
|Referencias de memoria| es capaz de referencir a ambas áreas de memoria| solo puede referenciar a la memoria localizada al user-mode|
|system crash| si el kernel falla, vuelve las cosas complicadas| si esl sistema falla puede recuperarse de la ultima sesión|
| acceso| solo las funcionalidades esenciales son permitidas en este modo| los programas pueden acceder y ejecutarse en algunos sistemas dados|
