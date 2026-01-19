<p align="center">
  <img src="https://img.icons8.com/color/200/chess.png" alt="Chess Opening Trainer Logo" width="150"/>
</p>

<h1 align="center">♟️ Chess Opening Trainer</h1>

<p align="center">
  <strong>Entrenador Interactivo de Aperturas de Ajedrez</strong>
</p>

<p align="center">
  <a href="#características">Características</a> •
  <a href="#demo">Demo</a> •
  <a href="#instalación">Instalación</a> •
  <a href="#uso">Uso</a> •
  <a href="#tecnologías">Tecnologías</a> •
  <a href="#aperturas-incluidas">Aperturas</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version"/>
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License"/>
  <img src="https://img.shields.io/badge/status-active-success.svg" alt="Status"/>
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind"/>
</p>

---

## Descripción

**Chess Opening Trainer** es una aplicación web moderna e interactiva diseñada para ayudarte a dominar las aperturas de ajedrez mediante práctica repetitiva inteligente. Con un sistema de selección adaptativo que prioriza las variantes que menos has practicado, garantiza un aprendizaje equilibrado y eficiente.

<p align="center">
  <img src="https://raw.githubusercontent.com/lichess-org/lila/master/public/images/home-bicolor.png" alt="Chess Board Preview" width="400"/>
</p>

### ¿Por qué Chess Opening Trainer?

| Problema | Solución |
|----------|----------|
| Memorizar aperturas es tedioso | Práctica interactiva con feedback inmediato |
| Olvidar variantes menos comunes | Sistema inteligente que prioriza variantes poco practicadas |
| Interfaces de ajedrez complicadas | Diseño limpio y moderno con Tailwind CSS |
| Necesidad de conexión constante | Funciona offline después de la carga inicial |

---

## Características

### Gestión de Aperturas

| Característica | Descripción |
|----------------|-------------|
| **Aperturas Personalizadas** | Añade tus propias aperturas con nombre, color y PGN |
| **Biblioteca Incluida** | 6 aperturas clásicas listas para practicar |
| **PGN Manual** | Practica cualquier PGN sin guardarlo |
| **Persistencia Local** | Tus aperturas se guardan automáticamente en el navegador |

### Motor de Entrenamiento Inteligente

| Característica | Descripción |
|----------------|-------------|
| **Análisis PGN Avanzado** | Parsea variantes y líneas principales automáticamente |
| **Selección Adaptativa** | Prioriza variantes menos practicadas |
| **Estadísticas por Variante** | Seguimiento de intentos, aciertos y rachas |
| **Reintento Inteligente** | Si fallas, practicas la misma variante hasta dominarla |

### Interfaz de Usuario

| Característica | Descripción |
|----------------|-------------|
| **Tablero Interactivo** | Drag & drop de piezas con validación |
| **Diseño Responsive** | Se adapta a móviles, tablets y escritorio |
| **Feedback Visual** | Colores claros para aciertos, errores e información |
| **Orientación Dinámica** | El tablero se gira según el color que practiques |

---

## Demo

### Flujo de la Aplicación

```
┌─────────────────────────────────────────────────────────────────┐
│                      MENÚ PRINCIPAL                             │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  Seleccionar Apertura Guardada  ▼                       │    │
│  │  ┌─────────────────────────────────────────────────┐    │    │
│  │  │ > Defensa Siciliana (Negras)                    │    │    │
│  │  │   Defensa Caro-Kann (Negras)                    │    │    │
│  │  │   Juego Vienés (Blancas)                        │    │    │
│  │  └─────────────────────────────────────────────────┘    │    │
│  └─────────────────────────────────────────────────────────┘    │
│                                                                 │
│  ┌──────────────────┐  ┌──────────────────────────────────┐     │
│  │ Añadir Apertura  │  │        Practicar PGN Manual      │     │
│  └──────────────────┘  └──────────────────────────────────┘     │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    MODO ENTRENAMIENTO                           │
│                                                                 │
│    ┌─────────────┐          ┌─────────────────────────┐         │
│    │  ♜ ♞ ♝ ♛ ♚  │          │  Tu turno: Juega e4     │         │
│    │  ♟ ♟ ♟ ♟ ♟  │          │                         │         │
│    │             │          │  Movimiento correcto!   │         │
│    │             │          │  Rival juega: e5        │         │
│    │  ♙ ♙ ♙ ♙ ♙  │          │                         │         │
│    │  ♖ ♘ ♗ ♕ ♔  │          │  [Reiniciar] [Menú]     │         │
│    └─────────────┘          └─────────────────────────┘         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Estados de Feedback

```
┌──────────────────────────────────────────────────────────┐
│  ✓ ¡Correcto! Bien jugado.                    [Verde]    │
└──────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────┐
│  ✗ Incorrecto. Se esperaba: Nf3               [Rojo]     │
└──────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────┐
│  ℹ El rival juega: e5                         [Azul]     │
└──────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────┐
│  🏆 ¡Línea completada! Nueva variante...      [Morado]   │
└──────────────────────────────────────────────────────────┘
```

---

## Instalación

### Requisitos Previos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexión a Internet (solo para cargar librerías CDN)

### Opción 1: Descarga Directa

```bash
# Simplemente descarga el archivo y ábrelo en tu navegador
open chessQuizz.html
```

### Opción 2: Clonar Repositorio

```bash
# Clonar el repositorio
git clone https://github.com/UO291047/ChessOpeningLearning.git

# Navegar al directorio
cd ChessOpeningLearning

# Abrir en el navegador
open chessQuizz.html
```

### Opción 3: Servidor Local (Recomendado)

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js
npx http-server

# Con PHP
php -S localhost:8000
```

Luego visita: `http://localhost:8000/chessQuizz.html`

---

## Uso

### 1. Añadir una Nueva Apertura

```
1. Click en "Añadir Nueva Apertura"
2. Rellena el formulario:
   - Nombre: Defensa Siciliana
   - Color: Negras
   - PGN: 1. e4 c5 2. Nf3 d6 3. d4 cxd4...
3. Click en "Guardar"
```

### 2. Practicar una Apertura Guardada

```
1. Selecciona la apertura del desplegable
2. Click en "Practicar Selección"
3. El tablero se orientará según tu color
4. ¡Realiza los movimientos correctos!
```

### 3. Practicar PGN Manual

```
1. Pega tu PGN en el área de texto
2. Selecciona el color con el que quieres jugar
3. Click en "Practicar PGN Manual"
```

### Formato PGN Soportado

```pgn
1. e4 e5 2. Nf3 Nc6 3. Bb5 (3. Bc4 Nf6) a6 4. Ba4 Nf6
```

> **Nota:** Se soportan variantes entre paréntesis `()` y líneas principales.

---

## Tecnologías

### Frontend

| Tecnología | Uso |
|------------|-----|
| **HTML5** | Estructura de la aplicación |
| **CSS3** | Estilos y animaciones |
| **JavaScript ES6** | Lógica de la aplicación |
| **Tailwind CSS** | Framework de utilidades CSS |
| **jQuery 3.5.1** | Manipulación del DOM |

### Librerías de Ajedrez

| Librería | Versión | Propósito |
|----------|---------|-----------|
| **Chess.js** | 0.10.3 | Motor de lógica de ajedrez |
| **Chessboard.js** | 1.0.0 | Tablero visual interactivo |

### Almacenamiento

| Tecnología | Propósito |
|------------|-----------|
| **LocalStorage** | Persistencia de aperturas y progreso |

---

## Aperturas Incluidas

El proyecto incluye 6 aperturas clásicas listas para practicar:

| Apertura | Archivo | Movimientos Iniciales | Color |
|----------|---------|----------------------|-------|
| **Siciliana Dragón Acelerada** | `AcceleratedDragonSicilian.txt` | 1. e4 c5 | Negras |
| **Defensa Benoni** | `BenoniDefense.txt` | 1. d4 c5 | Negras |
| **Defensa Caro-Kann** | `CaroKannDefense.txt` | 1. e4 c6 | Negras |
| **Juego Vienés** | `ViennaGame.txt` | 1. e4 e5 2. Nc3 | Blancas |
| **Gambito Rousseau** | `RousseauGambit.txt` | 1. e4 e5 2. Nf3 Nc6 3. Bc4 f5 | Negras |
| **Defensa Schliemann** | `SchliemannDefense.txt` | 1. e4 e5 2. Nf3 Nc6 3. Bb5 f5 | Negras |

---

## Estructura del Proyecto

```
ChessOpeningLearning/
│
├── chessQuizz.html              # Aplicación principal (HTML + CSS + JS)
│
├── AcceleratedDragonSicilian.txt    # Apertura: Siciliana Dragón
├── BenoniDefense.txt                # Apertura: Defensa Benoni
├── CaroKannDefense.txt              # Apertura: Caro-Kann
├── RousseauGambit.txt               # Apertura: Gambito Rousseau
├── SchliemannDefense.txt            # Apertura: Defensa Schliemann
├── ViennaGame.txt                   # Apertura: Juego Vienés
│
└── README.md                        # Este archivo
```

### Arquitectura del Código

```
chessQuizz.html
├── HEAD
│   ├── Meta tags
│   ├── Tailwind CSS (CDN)
│   ├── jQuery (CDN)
│   ├── Chess.js (CDN)
│   ├── Chessboard.js (CDN)
│   └── Estilos personalizados
│
├── BODY
│   ├── Pantalla del Menú Principal
│   │   ├── Selector de aperturas
│   │   ├── Input PGN manual
│   │   └── Botón añadir apertura
│   │
│   ├── Modal de Nueva Apertura
│   │   ├── Campo nombre
│   │   ├── Selector de color
│   │   └── Textarea PGN
│   │
│   └── Pantalla de Entrenamiento
│       ├── Tablero interactivo
│       ├── Área de feedback
│       └── Controles
│
└── SCRIPT
    ├── Variables globales
    ├── Funciones de parsing PGN
    ├── Motor de entrenamiento
    ├── Gestión de localStorage
    └── Event handlers
```

---

## Algoritmo de Selección Inteligente

El sistema utiliza un algoritmo sofisticado para seleccionar qué variante practicar:

```javascript
// Pseudocódigo del algoritmo
function seleccionarVariante(variantes) {
    // 1. Ordenar por éxitos consecutivos (menor primero)
    // 2. Luego por intentos totales (menor primero)
    // 3. Finalmente aleatorio para empates

    return variantes.sort((a, b) => {
        if (a.consecutiveSuccesses !== b.consecutiveSuccesses)
            return a.consecutiveSuccesses - b.consecutiveSuccesses;
        if (a.made !== b.made)
            return a.made - b.made;
        return Math.random() - 0.5;
    })[0];
}
```

**Beneficios:**
- Las variantes difíciles se practican más
- Las variantes dominadas se revisan ocasionalmente
- Práctica equilibrada de todo el repertorio

---

## Contribuir

¡Las contribuciones son bienvenidas! Si quieres mejorar Chess Opening Trainer:

1. **Fork** el repositorio
2. **Crea** una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** tus cambios (`git commit -m 'Add: Amazing Feature'`)
4. **Push** a la rama (`git push origin feature/AmazingFeature`)
5. **Abre** un Pull Request

### Ideas para Contribuir

- [ ] Añadir más aperturas predefinidas
- [ ] Implementar modo oscuro
- [ ] Añadir sonidos para movimientos
- [ ] Crear sistema de estadísticas avanzadas
- [ ] Exportar/importar repertorio completo
- [ ] Añadir temporizador para práctica con tiempo
- [ ] Integración con Lichess/Chess.com

---

## Roadmap

| Fase | Características | Estado |
|------|-----------------|--------|
| **v1.0** | Funcionalidad core, 6 aperturas | ✅ Completado |
| **v1.1** | Modo oscuro, más aperturas | 📋 Planificado |
| **v1.2** | Estadísticas avanzadas | 📋 Planificado |
| **v2.0** | Backend + sincronización | 💡 Idea |

---

## FAQ

<details>
<summary><strong>¿Funciona sin internet?</strong></summary>

Sí, después de cargar la página una vez, la aplicación funciona offline. Sin embargo, las imágenes de las piezas requieren conexión inicial.
</details>

<details>
<summary><strong>¿Dónde se guardan mis aperturas?</strong></summary>

En el localStorage de tu navegador. Los datos persisten entre sesiones pero son específicos de cada navegador/dispositivo.
</details>

<details>
<summary><strong>¿Puedo importar desde Lichess/Chess.com?</strong></summary>

Actualmente puedes copiar el PGN manualmente. La importación directa está en el roadmap.
</details>

<details>
<summary><strong>¿Qué formato de PGN se soporta?</strong></summary>

PGN estándar con variantes entre paréntesis. Se ignoran comentarios y anotaciones.
</details>

---

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

```
MIT License

Copyright (c) 2026 UO291047

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## Autor

<p align="center">
  <strong>Desarrollado con ♟️ por UO291047</strong>
</p>

---

<p align="center">
  <sub>Si este proyecto te ha sido útil, considera darle una ⭐ en GitHub</sub>
</p>

<p align="center">
  <a href="#️-chess-opening-trainer">⬆️ Volver arriba</a>
</p>
