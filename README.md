# 🔥 EL DESCENSO

> *«Lasciate ogne speranza, voi ch'intrate»* — Dante Alighieri, Infierno III

Un juego de laberintos en HTML5 puro inspirado en el **Infierno de la Divina Comedia**. Desciende por los nueve círculos del Infierno, resuelve cada laberinto antes de que la oscuridad te trague, y firma tu nombre en el libro de los condenados si logras salir.

**[▶ Jugar ahora](https://mangelsnc.github.io/el-descenso/el-descenso.html)** *(activar GitHub Pages en Settings)*

---

## 🎮 Cómo se juega

| Control | Acción |
|---------|--------|
| **Flechas / WASD** | Moverse por el laberinto |
| **ESC / P** | Pausa |
| **M** | Silenciar |
| **Swipe** (móvil) | Moverse |

**Objetivo:** Llega hasta la 💀 en cada nivel. Al cruzar la meta, el siguiente círculo empieza **sin avisar**. Diez niveles de dificultad creciente, de 8×8 hasta 32×32.

---

## 🔥 Los nueve círculos

Cada círculo lleva el nombre del pecado que Dante castiga en él:

| # | Círculo | Pecado | Tamaño |
|---|---------|--------|--------|
| 0 | La Puerta | — | 8×8 |
| I | Limbo | No bautizados | 10×10 |
| II | Lujuria | Lujuriosos | 12×12 |
| III | Gula | Glotones | 15×15 |
| IV | Avaricia | Avaros y pródigos | 18×18 |
| V | Ira | Iracundos | 21×21 |
| VI | Herejía | Herejes | 24×24 |
| VII | Violencia | Violentos | 27×27 |
| VIII | Fraude | Fraudulentos | 30×30 |
| IX | Traición | Traidores | 32×32 |

---

## ✨ Mecánicas

### 💡 Iluminación dinámica
Tu luz se apaga a cada círculo. El radio de visión se reduce progresivamente — en los últimos niveles apenas ves un par de celdas a tu alrededor.

### 🔥 Bengalas (desde Círculo IV)
Brasas naranjas que iluminan durante **12 segundos** con radio ampliado. Aparecen más si resuelves rápido.

### 🕯️ Velas (desde Círculo VI)
Brasas azules que **extienden el fuego**: +8s si llevas bengala activa, +3s de luz propia si no.

### 🏃 Bonus de velocidad
Cuanto más rápido resuelvas un nivel, más probabilidad de que aparezcan ítems en el siguiente. La velocidad se premia; la lentitud se castiga con oscuridad.

### 🏆 Ranking local
Al completar el descenso, firma tu nombre y tu tiempo. Los mejores tiempos se muestran en la pantalla de inicio.

---

## 🔊 Audio procedural

Todo el sonido se genera en tiempo real con **Web Audio API** — sin archivos de audio:

- **Latido de corazón** que se acelera con cada círculo
- **Susurros** aleatorios con paneo estéreo
- **Stinger** disonante al completar nivel
- **Boom** grave al llegar al final
- **Chime** de victoria al ver de nuevo las estrellas

---

## 🛠️ Técnica

- **Un solo archivo HTML** — sin dependencias, sin build, sin servidor
- Canvas 2D con rendering por celdas
- Laberintos generados proceduralmente (DFS + bucles aleatorios)
- Movimiento suave con interpolación
- Iluminación con gradientes radiales y flickering
- Tipografías: [Nosifer](https://fonts.google.com/specimen/Nosifer) + [Special Elite](https://fonts.google.com/specimen/Special+Elite)
- Compatible con móvil (controles táctiles, responsive, DPR)

---

## 🚀 Roadmap

Ideas en exploración para futuras versiones:

- **🐺 Cerbero** — Un guardián errático en el Círculo IX que deambula por el laberinto. No te persigue, pero cruzarte con él es... problemático.
- **⏱️ Modo contrarreloj** — Niveles individuales con leaderboard global para competir por el mejor tiempo.
- **⛵ Caronte** — El barquero del Aqueronte aparece aleatoriamente y te teletransporta a otro punto del mapa. ¿Riesgo o salvación?

---

## 📁 Estructura

```
el-descenso/
├── el-descenso.html    # El juego completo (HTML + CSS + JS)
├── CHANGELOG.md        # Historial de versiones
└── README.md           # Este archivo
```

---

## 📜 Licencia

Proyecto personal de [Miguel Ángel Sánchez Chordi](https://github.com/mangelsnc). Todos los derechos reservados.

---

> *«E quindi uscimmo a riveder le stelle»*
> — Dante Alighieri, Infierno XXXIV (último verso)
