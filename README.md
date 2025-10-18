[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21148405&assignment_repo_type=AssignmentRepo)
# Proyecto integrador 1ra Entrega

## Integrantes

- Heidy Nicol Sánchez Peña  
- David Mora  
- Federico Díaz Novoa

## Arquitectura propuesta



## Periférico a trabajar
## 🧩 Sensor TCS34725

El **TCS34725** es un módulo capaz de reconocer colores RGB (rojo, verde y azul), así como la intensidad de la luz blanca.  
Este sensor incluye un filtro infrarrojo (IR) que puede activarse o desactivarse para mejorar la sensibilidad y precisión, evitando interferencias del entorno.  

El TCS34725 se comunica mediante el protocolo **I2C**, lo que facilita su integración con el microcontrolador **ESP32**.  

---

### 🔧 Características técnicas
- **Voltaje de entrada:** 3.0 V a 5.0 V  
- **Corriente de entrada:** hasta 20 mA  
- **Chip base:** TCS3472   
- **Interfaz de comunicación:** I2C (SDA y SCL)  
- **Filtro IR:** integrado, mejora la precisión del color  

---

### 📷 Aplicaciones
- Detección y reconocimiento de color  
- Control automático de iluminación RGB  
- Clasificación de objetos por color  
- Sensado ambiental o corrección de balance de blancos en cámaras  

---

### 📟 Distribución de pines

La **Figura 1** muestra la distribución de pines del sensor **TCS34725**, donde se observan las conexiones necesarias para su correcto funcionamiento con el protocolo **I2C**.

| Pin | Nombre | Descripción |
|-----|---------|-------------|
| 1 | **VDD** | Alimentación del módulo (3 V – 5 V) |
| 2 | **SCL** | Línea de reloj I2C |
| 3 | **GND** | Tierra |
| 4 | **NC** | No conectado |
| 5 | **INT** | Pin de interrupción (opcional) |
| 6 | **SDA** | Línea de datos I2C |

---

### ⚙️ Proceso de calibración del sensor

Para poder realizar la calibración del sensor:

1. Se colocó una superficie **blanca** frente al sensor, registrando los valores RGB como referencia máxima.  
2. Luego se colocó una superficie **negra**, registrando los valores mínimos.  
3. Finalmente, se usaron esos valores como límites para ajustar las lecturas y obtener una medición más precisa de cualquier color intermedio.

---

#### Figura 1. Distribución de pines del sensor TCS34725

<img width="600" alt="Distribución de pines del sensor TCS34725" src="https://github.com/user-attachments/assets/99e27d8b-741d-4262-a29c-fb898426a1cf" />

**Fuente:** [TCS34725 Datasheet – ams OSRAM](https://electronilab.co/wp-content/uploads/2021/06/TCS34725.pdf)

## Avances

Figura 1

Calibración del color blanco:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/c5b0261c-2923-47ac-9b19-47354769f79d" />

Fuente: Elaboración propia

Figura 3

Calibración del color rojo:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/4c929b96-7b27-4aee-a1e2-fc13b9eb6241" />

Fuente: Elaboración propia

Figura 4

Calibración del color rosado:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/8355c986-4558-46e1-9508-38a08d673ca5" />

Fuente: Elaboración propia

Figura 5

Calibración del color amarillo:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/e13c201c-097d-4ca7-95a3-49f91f8ff034" />

Fuente: Elaboración propia

Figura 6

Calibración del color naranja:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/b7d7a13d-777b-4935-b0dc-ac85342d899b" />

Fuente: Elaboración propia


Figura 7

Calibración del color verde:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/be3471f5-dd6c-49cf-9a30-a733296db84e" />

Fuente: Elaboración propia

Figura 8

Calibración del color azul:
<img width="1064" height="521" alt="Image" src="https://github.com/user-attachments/assets/fe84b351-40aa-4a6c-b607-445a348fb76a" />

Fuente: Elaboración propia

<!-- Subir en una carpeta src los códigos que tienen hasta el momento y esta sección agregar lo que consideren necesario referente a sus avances. -->
