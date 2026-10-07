# Changelog — El Descenso

Todos los cambios notables del proyecto se documentan aquí.
Formato basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/).

---

## [v0.6.2] — 2026-10-07

### Añadido
- Nombres de los círculos del Infierno de Dante en el HUD (Limbo, Lujuria, Gula, Avaricia, Ira, Herejía, Violencia, Fraude, Traición)
- Sistema de bengalas (🔥) desde el Círculo IV: 12s de luz amplia
- Sistema de velas (🕯️) desde el Círculo VI: +8s si llevas bengala, +3s si no
- Bonus de velocidad: cuanto más rápido resuelves, más brasas aparecen
- Pantalla de ayuda (CÓMO JUGAR)
- Pantalla de pausa con opciones (Seguir, Abandonar partida, Salir del juego)
- Pantalla de despedida al salir del juego
- Pantalla final con estrellas y cita de Dante («E quindi uscimmo a riveder le stelle»)
- Ranking local con firma en el libro de los condenados
- Efectos de sonido: latido de corazón, susurros, stinger al completar nivel, boom final, chime de victoria
- Puerta del Infierno animada en pantalla de inicio con inscripción dantesca
- Controles táctiles (swipe) para móvil
- Silenciado con tecla M
- Pausa con ESC / P

### Técnico
- Laberinto generado proceduralmente con algoritmo DFS + bucles aleatorios
- 10 niveles de dificultad creciente (8×8 hasta 32×32)
- Sistema de iluminación dinámica con flickering y viñeta
- Movimiento suave con interpolación (lerp)
- Audio procedural con Web Audio API (sin archivos externos)
- Ranking persistido en localStorage
- Diseño responsive con devicePixelRatio

---

## [v0.6.1] — 2026-10-06

### Cambiado
- Ajustes de dificultad y balance de niveles
- Mejoras en el sistema de iluminación

---

*Versiones anteriores no documentadas.*
