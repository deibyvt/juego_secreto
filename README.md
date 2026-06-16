# 🎮 Juego del Número Secreto

Un juego interactivo desarrollado con **HTML, CSS y JavaScript** donde el usuario intenta adivinar un número secreto aleatorio entre 1 y 50.

---

## 📋 Descripción del Proyecto

El **Juego del Número Secreto** es una aplicación web educativa que implementa la lógica de un juego clásico de adivinanzas. El jugador debe adivinar un número generado aleatoriamente mientras recibe pistas sobre si el número secreto es mayor o menor que su intento.

### Características Principales

- ✅ Generación aleatoria de números sin repetición
- ✅ Sistema de pistas dinámicas (número mayor/menor)
- ✅ Contador de intentos realizados
- ✅ Interfaz visual atractiva con degradados y animaciones
- ✅ Posibilidad de jugar múltiples rondas
- ✅ Rango de números configurable (1-50)

---

## 📁 Estructura del Proyecto

```
juego-secreto/
├── index.html          # Estructura HTML de la aplicación
├── app.js              # Lógica del juego en JavaScript
├── style.css           # Estilos y diseño de la interfaz
├── img/                # Carpeta de imágenes
│   ├── ia.png          # Imagen de persona (IA)
│   ├── code.png        # Fondo de código
│   └── Ruido.png       # Textura de ruido
└── README.md           # Este archivo
```

---

## 🛠️ Tecnologías Utilizadas

| Tecnología | Descripción |
|-----------|-------------|
| **HTML5** | Estructura y semántica del documento |
| **CSS3** | Estilos, gradientes y diseño responsivo |
| **JavaScript (ES6+)** | Lógica del juego e interactividad |
| **Google Fonts** | Fuentes: Chakra Petch y Inter |

---

## 🚀 Cómo Usar

### Requisitos
- Un navegador web moderno (Chrome, Firefox, Safari, Edge, etc.)
- No requiere instalación ni dependencias externas

### Pasos para Ejecutar

1. **Descargar o clonar** el proyecto en tu máquina
2. **Abrir el archivo** `index.html` en tu navegador
3. **Ingresar un número** entre 1 y 50 en el campo de entrada
4. **Hacer clic** en el botón "Intentar"
5. **Recibir pistas** y continuar intentando hasta adivinar el número
6. **Hacer clic** en "Nuevo juego" para jugar nuevamente

---

## 📝 Funcionalidades del Código

### Variables Principales

```javascript
let numeroSecreto = 0;           // Almacena el número a adivinar
let intentos = 0;                // Contador de intentos realizados
let listaNumerosSorteados = [];  // Lista para evitar repeticiones
let numeroMaximo = 50;           // Límite superior del rango
```

### Funciones Clave

#### `asignarTextoElemento(elemento, texto)`
Asigna texto a un elemento HTML del DOM.
- **Parámetros:**
  - `elemento`: Selector CSS del elemento
  - `texto`: Texto a asignar

#### `verificarIntento()`
Valida el número ingresado por el usuario.
- Compara con el número secreto
- Proporciona pistas si no es correcto
- Habilita el botón "Nuevo juego" cuando se acierta

#### `generarNumeroSecreto()`
Genera un número aleatorio sin repeticiones.
- Evita números que ya han sido sorteados
- Implementa recursión para reintentar si el número ya existe

#### `condicionesIniciales()`
Inicializa los parámetros del juego.
- Asigna el texto de bienvenida
- Genera un nuevo número secreto
- Reinicia el contador de intentos

#### `reiniciarJuego()`
Reinicia completamente el juego.
- Limpia el campo de entrada
- Llama a `condicionesIniciales()`
- Deshabilita el botón de nuevo juego

#### `limpiarCaja()`
Limpia el campo de entrada numérico.

---

## 🎨 Estilos y Diseño

### Características de CSS

- **Gradiente de fondo**: Degradado azul oscuro a negro
- **Contenedor principal**: 1200px × 600px con borde degradado
- **Fuentes**: 
  - Chakra Petch (títulos)
  - Inter (texto general)
- **Efectos visuales**: Sombras, opacidad y fondos con texturas

---

## 📱 Compatibilidad

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Microsoft Edge
- ✅ Dispositivos móviles (responsive design)

---

## 🎯 Objetivo Educativo

Este proyecto fue desarrollado como parte de la **Nivelación ONE AI FOR TECH** de Oracle Alura, con enfoque en:

- Fundamentos de JavaScript
- Manipulación del DOM
- Manejo de eventos
- Algoritmos de generación aleatoria
- Buenas prácticas de código
- Diseño responsivo

---

## 💡 Posibles Mejoras Futuras

- [ ] Agregar nivel de dificultad (rangos diferentes)
- [ ] Implementar sistema de puntuación
- [ ] Agregar sonidos de efectos
- [ ] Guardar historial de juegos
- [ ] Modo multijugador
- [ ] Animaciones más complejas
- [ ] Temas de color personalizables

---

## 📄 Licencia

Este proyecto es de código abierto y se proporciona con propósitos educativos.

---

## 👨‍💻 Autor

Desarrollado como parte del programa de formación **Oracle Alura - Nivelación ONE AI FOR TECH**

**Fecha**: 2026

---

## 📞 Soporte

Para reportar problemas o sugerencias, contacta al desarrollador o revisa el código fuente.

---

**¡Diviértete jugando y aprendiendo!** 🎮✨
