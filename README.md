# 🎱 Bingo Master

> La app de bingo familiar, multijugador y multilingüe — sin instalación, directo desde el navegador.

![HTML](https://img.shields.io/badge/HTML-5-orange?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS-3-blue?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?style=flat-square&logo=javascript)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-green?style=flat-square)
![Idiomas](https://img.shields.io/badge/idiomas-4-purple?style=flat-square)

---

## 📱 Pantallas

| ① Configuración | ② Bombo | ③ Cartilla del jugador |
|:-:|:-:|:-:|
| Elige idioma, nombres y cartillas por jugador | El presentador canta números con voz | Cada jugador marca sus números en su móvil |

---

## ✨ Características

- 🎲 **Bombo automático** — sortea los 90 números sin repetición y los canta en voz alta
- 📲 **QR por jugador** — genera un código QR único para que cada jugador acceda a sus cartillas desde su móvil
- 🗣️ **Voz natural** — pronuncia los números en el idioma seleccionado usando el motor TTS del sistema
- 🎯 **Detección automática** — detecta línea y bingo en tiempo real al marcar números
- 🎉 **Confeti** — animación de celebración al conseguir línea o bingo
- 🌍 **4 idiomas** — español, inglés, italiano y francés (interfaz + voz + mensajes)
- 📱 **Sin instalación** — un solo archivo `.html`, funciona en cualquier navegador

---

## 🎮 Cómo se juega

### Para el presentador

1. Abre `index.html` en el navegador de tu ordenador o tablet
2. Elige el **idioma** del juego
3. Escribe los **nombres** de los jugadores separados por coma
4. Indica cuántas **cartillas** quiere cada jugador (1–3)
5. Pulsa **"Generar Juego"**
6. Comparte el **QR** con cada jugador para que acceda a sus cartillas
7. Pulsa **"¡Cantar!"** para sacar números — la app los dice en voz alta automáticamente

### Para los jugadores

1. Escanea el QR con la cámara del móvil
2. Se abre tu cartilla directamente en el navegador — sin instalar nada
3. Toca los números cuando el presentador los cante para marcarlos
4. La app te avisa automáticamente si haces **línea** o **bingo** 🎉

---

## 📋 Reglas

### El bombo
- Sortea números del **1 al 90** sin repetición
- Una vez cantado un número no vuelve a salir
- El contador muestra las **bolas restantes** en todo momento

### Las cartillas
- Cada cartilla tiene **15 números aleatorios** del 1 al 90
- Distribuidos en **3 filas de 5 números**
- Cada jugador puede tener hasta **3 cartillas** distintas por partida

### Marcar números
- Cuando se canta un número que tienes en tu cartilla, **tócalo** para marcarlo
- Los números marcados se muestran en **verde**
- Puedes desmarcar un número volviendo a tocarlo

### 🎯 ¡Línea!
Se consigue cuando se marcan los **5 números de una misma fila**

```
[ 7 ] [14 ] [28 ] [45 ] [63 ]   ← ¡LÍNEA! (fila completa)
  3     11    19    32    70
 21     36    51    58    82
```

### 🏆 ¡Bingo!
Se consigue cuando se marcan los **15 números de la cartilla completa**

```
[ 7 ] [14 ] [28 ] [45 ] [63 ]
[ 3 ] [11 ] [19 ] [32 ] [70 ]   ← ¡BINGO! (cartilla entera)
[21 ] [36 ] [51 ] [58 ] [82 ]
```

En ambos casos se lanza una **animación de confeti** y aparece el mensaje de victoria en el idioma del juego.

---

## 🌍 Idiomas

| Bandera | Idioma | ¡Línea! | ¡Bingo! |
|:---:|---|---|---|
| 🇪🇸 | Español | ¡LÍNEA! | ¡BINGO! |
| 🇬🇧 | English | LINE! | BINGO! |
| 🇮🇹 | Italiano | TERNO! | BINGO! |
| 🇫🇷 | Français | QUINE! | BINGO! |

La voz, la interfaz y los mensajes de victoria se adaptan automáticamente al idioma seleccionado. Los números se pronuncian **escritos en palabras** para mayor claridad (ej: "cinco" en lugar del dígito "5").

---

## 💻 Requisitos

| | |
|---|---|
| **Navegador** | Cualquier navegador moderno (Chrome, Safari, Firefox, Edge) |
| **Instalación** | Ninguna — solo abre `index.html` |
| **Internet** | No necesario para jugar |
| **Red local** | Necesaria para que los jugadores escaneen el QR desde sus móviles (misma WiFi) |
| **Voz** | Motor TTS del sistema operativo (mejor calidad en iOS/macOS) |

> 💡 **Consejo para la voz en Android:** ve a *Ajustes → Accesibilidad → Texto a voz → Motor de Google → Instalar datos de voz* y descarga español e italiano para mejor pronunciación.

---

## 🚀 Uso rápido

```bash
# Clona o descarga el repositorio
git clone https://github.com/tu-usuario/bingo-master.git

# Abre directamente en el navegador
open index.html
# o en Windows:
start index.html
```

No necesitas ningún servidor, npm install ni dependencias externas.

---

## 📁 Estructura

```
bingo-master/
└── index.html    ← toda la app en un solo archivo
```

---

## 🛠️ Tecnologías

- **HTML5 / CSS3 / JavaScript** vanilla — sin frameworks
- **Web Speech API** (`speechSynthesis`) — para la voz del bombo
- **QRCode.js** — generación de códigos QR (cargado desde CDN)
- **Google Fonts** — tipografías Fredoka One y Nunito

---

## 📄 Licencia

MIT — úsalo, modifícalo y compártelo libremente.

---

<div align="center">

Creado en BCN con ❤️ por **Mirko**

</div>
