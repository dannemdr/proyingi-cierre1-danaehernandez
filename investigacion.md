# Investigación: ¿esto ya existe? ¿quién lo dice?

**Autor:** Danae Hernández Saavedra
**Fecha:** 18 de septiembre de 2026
**Ideas analizadas:** ver [[ideas-proyecto]] o [ideas-proyecto.md](ideas-proyecto.md)

---

## Parte 1. Un ejemplo que ya existe, por cada idea

### Idea 1: Radiant

- **Qué encontré:** SelfQuest.
- **Enlace:** https://selfquest.net/
- **Qué hace:** Es una plataforma web que dirije a la app orientada en misiones (mayormente fitness) y tareas con elementos de juego.
- **Por qué no resuelve mi caso:** Porque depende 100% de usar el celular o la computadora. Al ser solo una app más en el teléfono, genera distracción con las notificaciones, es muy fácil ignorarla o cerrarla después de unos días y termina olvidándose. Mi propuesta busca un dispositivo físico de escritorio que esté presente en tu entorno, pase desapercibido en tu rutina sin obligarte a usar la pantalla del celular, te recuerde físicamente actuar y que no te obligue a estar en el celular todo el tiempo. 

### Idea 2: ShoobyKey

- **Qué encontré:** Llaves de seguridad YubiKey (Yubico).
- **Enlace:** https://www.yubico.com/products/
- **Qué hace:** Dispositivos USB de autenticación por hardware para iniciar sesión de forma segura.
- **Por qué no resuelve mi caso:** Tuve la oportunidad de usar una en un trabajo de computación previo, pero era muy poco intuitiva y realmente no entendía bien qué hacía al conectarla. Para uso personal le falta ser mucho más interactiva, explicarle claramente al usuario qué sitio está pidiendo acceso a través de una pantalla y ser más flexible y accesible para personas comunes (son bastante caras, en mi trabajo si es que la dañabas tenía un costo de $70 dólares).

### Idea 3: Chobic

- **Qué encontré:** Cámaras térmicas industriales para prevención de incendios (JideTech).
- **Enlace:** https://www.jidetech.com/es/collections/thermal-camera/products/lc008-plus-heavy-duty-thermal-camera-for-forest-fire-prevention
- **Qué hace:** Cámaras de termografía para inspección pesada e industrial.
- **Por qué no resuelve mi caso:** Son equipos de muy difícil obtención, sumamente caros e inaccesibles para la gente común. Falta alternativa comercial accesible para el hogar o la oficina cotidiana de manera especifica con alarmas, cámara, bajo costo y que no sea la típica cámara resuelvetodo de Amazon (Que no suelen funcionar al 100). La idea de Chobic es hacer que la seguridad térmica preventiva sea accesible, portátil e interactiva para cualquier persona.

---

## Parte 2. Fuentes de la idea que elegí

### Fuente 1

| Campo                | Contenido                                                                                                                                      |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Autor u organización | Google AI for Developers                                                                                                                       |
| Título               | Documentación oficial de la API de Gemini y Google AI Studio                                                                                   |
| Año                  | 2026                                                                                                                                           |
| Enlace               | https://ai.google.dev/docs                                                                                                                     |
| Tipo                 | documentación técnica                                                                                                                          |
| Por qué le creo      | Es la documentación técnica oficial que brinda el proveedor directamente.                                                                      |
| Qué dato me dio      | El procedimiento para generar la API Key gratuita y cómo estructurar los Prompts para recibir respuestas estrictamente en formato JSON ligero. |


---

### Fuente 2

| Campo | Contenido |
|---|---|
| Autor u organización | Espressif Systems |
| Título | Guía de hardware y especificaciones del ESP32-S3 |
| Año | 2025 |
| Enlace | https://www.espressif.com/en/products/socs/esp32-s3 |
| Tipo | documentación técnica |
| Por qué le creo | Es el fabricante del microcontrolador que se utilizará en el proyecto. |
| Qué dato me dio | La información de pines I2C/SPI y la capacidad de la memoria SRAM para procesar solicitudes HTTP/HTTPS con Wi-Fi. |


---

### Fuente 3

| Campo | Contenido |
|---|---|
| Autor u organización | Interaction Design Foundation |
| Título | Gamification: How to Design Engaging Experiences |
| Año | 2024 |
| Enlace | https://www.interaction-design.org/literature/topics/gamification |
| Tipo | artículo técnico/educativo |
| Por qué le creo | Es un instituto de diseño con prestigio internacional especializado en experiencia de usuario. |
| Qué dato me dio | Los principios para descomponer objetivos complejos en pequeñas metas con retroalimentación visual inmediata sin generar saturación. |

---
### Fuente 4

| Campo | Contenido |
|---|---|
| Autor u organización | Adafruit Industries |
| Título | Adafruit NeoPixel Library Documentation |
| Año | 2026 |
| Enlace | https://learn.adafruit.com/adafruit-neopixel-uberguide |
| Tipo | documentación de librería open-source |
| Por qué le creo | Es el fabricante y creador de la librería estándar para tiras LED programables en Arduino/ESP32. |
| Qué dato me dio | El consumo energético en miliamperios (mA) de cada LED NeoPixel para calcular el requerimiento de la fuente de alimentación. |

---

### Fuente 5

| Campo | Contenido |
|---|---|
| Autor u organización | Random Nerd Tutorials |
| Título | ESP32-S3 HTTP GET / POST Requests using Arduino IDE |
| Año | 2025 |
| Enlace | https://randomnerdtutorials.com/esp32-http-get-post-arduino/ |
| Tipo | tutorial técnico especializado |
| Por qué le creo | Es un portal de referencia muy reconocido en proyectos de electrónica y microcontroladores. |
| Qué dato me dio | El código base para realizar peticiones HTTP POST seguras enviando y leyendo objetos JSON mediante Wi-Fi. |

---

### Fuente 6

| Campo                | Contenido                                                                                                                                                                                                                  |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autor u organización | brenpoly (YouTube)                                                                                                                                                                                                         |
| Título               | I made a real BMO local AI agent with a Raspberry Pi and Ollama                                                                                                                                                            |
| Año                  | 2026                                                                                                                                                                                                                       |
| Enlace               | https://www.youtube.com/watch?v=l5ggH-YhuAw                                                                                                                                                                                |
| Tipo                 | video tutorial / proyecto maker                                                                                                                                                                                            |
| Por qué le creo      | Muestra todo el proceso práctico de ensamble físico de un robot/agente de escritorio interactivo con pantalla, botones y un agente de IA.                                                                                  |
| Qué dato me dio      | La arquitectura para integrar botones mecánicos, pantalla y un microcontrolador enviando estados visuales y respuestas de IA en un dispositivo físico y ver mas o menos como funcionan ideas similares en cuanto a físico. |

---

### Fuente 7

| Campo                | Contenido                                                                                                                                                                                       |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autor u organización | Thanh-y David Nguyen (YouTube)                                                                                                                                                                  |
| Título               | How to build a JARVIS AI Voice Agent for FREE \| Full Livekit Tutorial                                                                                                                          |
| Año                  | 2026                                                                                                                                                                                            |
| Enlace               | https://www.youtube.com/watch?v=Fhm8goKN6rM                                                                                                                                                     |
| Tipo                 | video tutorial técnico                                                                                                                                                                          |
| Por qué le creo      | Explica paso a paso cómo conectar la API gratuita de Gemini (Gemini Flash) con un flujo de interacción de voz en tiempo real.                                                                   |
| Qué dato me dio      | El procedimiento para configurar la API Key de Google Gemini y utilizar llamadas a funciones (Tool Calling / Function Tools) para ejecutar tareas externas y darme ánimos de que si es posible  |


---

## Parte 3. Qué haría distinto

A diferencia de las plataformas exclusivamente digitales como SelfQuest que se quedan como una app más en el celular y se olvidan rápidamente, mi propuesta crea un gadget físico de escritorio. El dispositivo no requiere que uses tu celular para funcionar, eliminando distracciones. Además, utiliza la API de Gemini o alguna parecido como la que vimos el viernes  para que el usuario solo reciba la misión secundaria actual, engañando al cerebro para cumplir objetivos paso a paso sin abrumarse, acompañando la experiencia con luces Neopixel y sonido retro, porque como vimos en las fuentes, tras una investigación todo se trata de la experiencia del usuario, por eso hasta esta de moda y es tan buen negocio las alarmas Hatch se centra en brindar un  experiencia al usuario.