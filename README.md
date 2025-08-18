# Diseno_logico_tutorial_1
Kenneth Aaron Campos Rodríguez
carnet---> 2021023141
Herramientos de codigo abierto para diseño digital utilizando fpga

---semana 2---

Date --> 12/08/2025


# Paso 1 ----> Instalacion de VS code

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/35c61694-ab98-4c33-8ead-aa086a83d917" />


# Paso 2  ----> Instalacion de liberias de Lushay Code.

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/757a80f9-0803-4e3f-88c4-c52f2debdea1" />

# Paso 3 ----> Instalacion de liberias de Verilog HDL

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/e27ed62c-3736-4ce5-83b3-62961f627ea7" />

# Paso 4 ----->  Instalacion de Make y editar variables de entorno

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/12cd1074-3f41-4742-9ddb-1c1a1ef8471a" />

# 2 Uso del toolchain para diseño en FPGA

Este proyecto utiliza una FPGA TangNano y está estructurado para facilitar el desarrollo, simulación y carga de diseños digitales. A continuación se describen los tipos de archivos necesarios y la jerarquía recomendada.

# 📁 Tipos de Archivos

- **Archivos de diseño (`.v`, `.sv`)**  
  Contienen el código RTL que será sintetizado. Representan la lógica del sistema.

- **Archivos de simulación (`.v`, `.sv`)**  
  Incluyen los testbench para verificar el comportamiento del diseño mediante simulación.

- **Archivo de constraints (`.cst`)**  
  Define la asignación de señales de entrada/salida del módulo top a los pines físicos de la FPGA TangNano.

- **Archivo Make (`Makefile`)**  
  Contiene comandos para automatizar etapas como síntesis, implementación, simulación y carga del diseño en la FPGA usando herramientas de código abierto.
# 2.1 Inicializar la terminal del toolchain:

Primero que todo se debe ubicar el acceso a las herramientas.

Presione en FPGA Toolchain en la parte inferior derecha. Después presione en Open Terminal.

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/e1b67806-843e-4a66-8df2-098aff8c9dcb" />

Esto nos permitirá ejecutar comandos personalizados para tener un control completo sobre nuestros diseños digitales. Además, podremos aprovechar los Makefiles como recetas automatizadas que simplifican y agilizan el flujo de trabajo.

Es importante haber iniciado una terminal compatible con OSS-CAD-Suite para utilizar estas herramientas correctamente.


<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/50c848dc-ce6e-4cd7-bcab-6a5d1d51eb1c" />

En esta terminal podremos hacer uso de las herramientas de síntesis, simulación e implementación.

Para comprobarlo ingrese el comando por ejemplo -----> yosys

##  yosys ejecuta la suite para síntesis y desarollo de Yosys.

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/f1079ee2-ebeb-4645-93ff-71d34625e124" />

Para salir de la suite de Yosys ingrese el siguiente comando -----> exit

# 2.2 Uso básico de la extensión con recetas:

El conjunto de herramientas incluye una gran variedad de comandos, opciones y banderas. No obstante, cubrir todos estos detalles excede el alcance de este tutorial. Por ello, se ha preparado una plantilla de receta que contiene todo lo necesario para desarrollar cualquier proyecto de forma estructurada.

Dentro de la carpeta `build` de los ejemplos, encontrarás un archivo `Makefile` que reúne los comandos correspondientes a cada etapa del desarrollo. Al crear tus propios proyectos, se recomienda generar un `Makefile` personalizado en tu carpeta `build`, tomando como referencia las plantillas proporcionadas.

Para poner esto en práctica, accede a la carpeta `build` del ejemplo **BlinkyLed**. Puedes hacerlo utilizando el comando `cd`, que permite navegar hacia una ruta relativa desde tu ubicación actual. En este caso, el comando sería:

Seguidamente, De la dirección actual (rojo) se sigue la ruta indicada por la dirección al destino (verde)

- Para la verificación de los diseños y simulación tenemos los siguientes comandos:

- Para ejecutar el testbench y simular el diseño, señalado en color morado------> **Make test** 

- Ejecutando este comando en la terminal, esto generará en la carpeta build un archivo .vcd que contiene las señales simuladas en función del tiempo que se marcan en color morado. Además se mostrará en la consola los resultados o tareas del testbench.

- Para visualizar los diagramas de tiempo con GTKwave ------> **Make wv**



<img width="1067" height="386" alt="image" src="https://github.com/user-attachments/assets/d65d8930-b530-4d2f-ac24-98909aa3404b" />


