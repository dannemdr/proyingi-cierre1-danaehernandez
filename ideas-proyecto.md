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