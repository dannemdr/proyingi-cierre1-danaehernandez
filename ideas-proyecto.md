# Tres ideas de proyecto

**Autor:** Danae Hernández Saavedra
**Fecha:** 20 de septiembre de 2026

---

## Criterios de viabilidad

Una idea es viable para esta materia si cumple los cuatro criterios:

1. Atiende un **problema concreto de mi entorno** (mi casa, la IBERO, mi colonia, mi municipio), no un tema general.
2. Tiene una **parte física fabricable** con impresión 3D, corte láser o router CNC.
3. Usa **al menos un sensor o un actuador** controlado por un microcontrolador pequeño.
4. Lo puede construir un **equipo de principiantes en unas ocho sesiones**, con materiales accesibles.




---

## Idea 1: Radiant (Generador Físico de Side-Quests)

**Problema.** La falta de estructura cuando tenemos impulsos de energía o ganas de cambiar la rutina provoca que nos abrumemos antes de empezar. Al ver una meta gigante, la mente se satura con tanto detalle y termina dispersándose en 20 cosas distintas a la vez sin completar ninguna.

**A quién le pasa.** A personas con sobrecarga de tareas, hiperactividad o estudiantes que quieren avanzar en sus metas pero sufren de fatiga mental ante el exceso de información.

**Dónde lo he visto.** En mi propia habitación y en mi casa durante las noches. Muchas veces me entra un ataque repentino de energía a medianoche o a mitad del día con ganas de ordenar todo mi cuarto, ponerme fit o aprender algo nuevo, pero al ver todo el desorden o no saber por dónde empezar, me abrumo, me disperso y no hago nada.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Perilla / Encoder rotativo (KY-040) para seleccionar la meta principal e interactuar con el menú, y un botón mecánico/táctil para presionar "Misión Cumplida".
- Qué hace con eso (actuador, aviso, pantalla): El ESP32-S3 se conecta por Wi-Fi a la API de Gemini para descomponer la meta en mini-misiones de 10 minutos dependiendo de la mision (mostrando solo la misión actual en una pantalla OLED 1.3"). Utiliza un anillo/tira LED NeoPixel como temporizador visual y un buzzer pasivo para emitir sonidos retro de 8-bits al ganar XP, ósea al completar la misión.
- Qué pieza habría que fabricar: Carcasa estilo retro-arcade/cyberpunk en acrílico con corte láser, con los orificios para la pantalla, el dial, los LEDs y el botón físico.

---

## Idea 2: ShoobyKey (Llave Biométrica de Seguridad Físico-Digital)

**Problema.** La vulnerabilidad de nuestras cuentas personales al depender únicamente de contraseñas de texto, las cuales pueden ser filtradas o robadas en ataques a servidores, dejando desprotegidas nuestras redes sociales e información privada.

**A quién le pasa.** A usuarios de internet, estudiantes y cualquier persona que maneje redes sociales y servicios digitales sin un factor de autenticación físico.

**Dónde lo he visto.** En mi vida personal recientemente. Sufrí un ataque al entrar a un servidor de Discord desde el cual lograron extraer mis contraseñas de varias redes sociales y cuentas personales. Ahí me di cuenta de lo fácil que es perder el control de tus accesos digitalmente si no tienes una capa de seguridad física.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Sensor de huella dactilar capacitivo (FPM10A/R307) para validar biométricamente la identidad del usuario antes de liberar cualquier acceso.
- Qué hace con eso (actuador, aviso, pantalla): El ESP32-S3 procesa el protocolo FIDO2 / WebAuthn por USB nativo. Una pantalla OLED de 0.96" muestra qué sitio está solicitando acceso y un anillo LED NeoPixel indica si el acceso fue seguro (Verde) o si hubo un intento no autorizado (Rojo).
- Qué pieza habría que fabricar: Chasis compacto tipo llavero rígido con conectores reforzados, fabricado en acrílico con corte láser.

---

## Idea 3: Chobic (Escáner y Diagnóstico Térmico Portátil)

**Problema.** La falta de atención a los detalles en nuestra rutina diaria, como olvidar si dejamos aparatos encendidos, conexiones eléctricas calientes o sobrecalentamientos en equipos, lo que representa un riesgo alto de incendios o fallas sin que nadie se dé cuenta a tiempo.

**A quién le pasa.** A personas que viven solas, familias o trabajadores en oficinas que, por el ajetreo diario y la prisa, no se percatan de anomalías térmicas en su entorno.

**Dónde lo he visto.** En mi casa, en oficinas y en departamentos donde las personas salen con prisa y no recuerdan si apagaron todo o dejaron algo encendido. Al no haber alguien al pendiente o no prestar atención a la rutina, los riesgos de un corto o sobrecalentamiento pasan desapercibidos hasta que ya es tarde.

**Cómo funcionaría.**
- Qué mide o detecta (sensor): Sensor térmico infrarrojo (AMG8833 o MLX90640) conectado por bus I2C para capturar la matriz de temperaturas.
- Qué hace con eso (actuador, aviso, pantalla): El ESP32-S3 procesa la matriz térmica y la despliega en una pantalla TFT a color de 1.8". Al detectar un punto crítico o brecha de calor, activa un motor de vibración (alerta háptica), un buzzer pasivo y LEDs NeoPixel que cambian de color según la gravedad del riesgo.
- Qué pieza habría que fabricar: Carcasa en capas de acrílico humo mediante corte láser con diseño ergonómico estilo "GameBoy" táctico y ventana protectora para el sensor térmico.

---

## Tabla de viabilidad

| Criterio                                                  | Idea 1 (Radiant) | Idea 2 (ShoobyKey) | Idea 3 (Chobic) |
| --------------------------------------------------------- | ---------------- | ------------------ | --------------- |
| Problema concreto de mi entorno                           | Sí               | Sí                 | Sí              |
| Parte física fabricable                                   | Sí               | Sí                 | Sí              |
| Sensor o actuador                                         | Sí               | Sí                 | Sí              |
| Construible en ocho sesiones por principiantes            | Sí               | Medio              | Sí              |
| Qué tan seguro estoy de lo anterior (alto / medio / bajo) | Alto             | Medio              | Medio           |

## Mi elección

**Idea elegida:** Idea 1: Radiant (Generador Físico de Side-Quests).

**Por qué.** Es la idea más viable y balanceada para el tiempo del curso. Afronta de manera directa el problema de la fatiga mental y la dispersión en el hogar sin saturar con apps de celular. Además, el costo de los componentes es muy accesible y la integración del ESP32-S3 con la API gratuita de Gemini se adapta perfectamente a las 8 sesiones de trabajo sin requerir infraestructura compleja. Asimismo, a partir de la inmersión que tuvimos durante el Día del Programador, me pareció sumamente interesante el taller que usted impartió. Quedé muy motivada para seguir trabajando con inteligencia artificial y desarrollar un bot capaz de generar misiones personalizadas adaptadas a cada usuario. Al conectarlo con Gemini, como lo trabajamos esa ocasión, no solo cubriremos un amplio espectro de aprendizaje, sino que pondremos en práctica los conocimientos adquiridos este parcial en esta y otras asignaturas.

**Qué todavía no sé.** Falta probar la latencia exacta de respuesta entre el ESP32-S3 y la API de Google al enviar y recibir el JSON mediante Wi-Fi, y el cómo realizar una carcasa, no se bien de diseño, pero siempre es bueno aprender nuevas cosas y al final para eso vivimos, para aprender. En diseño me imagino algo así como un BMO. 

---

## Declaración de uso de IA

- **Herramienta utilizada:** Google Gemini (Modelo Gemini 1.5 Pro).
- **Qué le pedí:** Apoyo como asistente para revisar la ortografía, dar formato Markdown a mis borradores y organizar los textos en la plantilla requerida. 
- **Qué modifiqué o rechacé de su respuesta, y por qué:** Reescribí completamente las descripciones de los problemas, las vivencias personales, la lógica de los dispositivos (con ayuda de deepseek, para ver si mi lógica estaba bien y era viable) y las razones de elección para asegurar que el contenido reflejara al 100% mis ideas, experiencias y decisiones técnicas.