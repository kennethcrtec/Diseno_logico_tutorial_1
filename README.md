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
# 1 Inicializar la terminal del toolchain:

Primero que todo se debe ubicar el acceso a las herramientas.

Presione en FPGA Toolchain en la parte inferior derecha. Después presione en Open Terminal.

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/e1b67806-843e-4a66-8df2-098aff8c9dcb" />



