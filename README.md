# Calculadora de Cálculo de Texto Tipográfico | UTP

Herramienta interactiva y recurso didáctico diseñado para facilitar la comprensión y el cálculo de la extensión de texto compuesto en el diseño editorial. 

---

## 📖 Descripción General

Esta aplicación web de un solo archivo (*Single-Page Application*) permite a los estudiantes de Diseño Editorial calcular de manera precisa cuántas páginas o espacio físico ocupará un manuscrito una vez diagramado. A través de una interfaz interactiva, la herramienta no solo automatiza el cálculo matemático, sino que desglosa visualmente la **fórmula tipográfica paso a paso**, fomentando la competencia técnica, analítica y creativa del alumno.

Soporta los dos estándares principales de medición tipográfica:
* **Sistema Anglosajón (PostScript):** Medición en picas y puntos (1 pt = 0.353 mm).
* **Sistema Francés (Didot):** Medición en cíceros y puntos (1 pt = 0.376 mm).

## ✨ Características Principales

* **Calculadora Dinámica:** Procesamiento en tiempo real de variables como modelo de letra, puntaje, interlineado, cantidad de golpes del manuscrito y ancho de columna.
* **Simulador Visual de Columna:** Representación gráfica en vivo de la mancha de texto, mostrando la distribución de renglones y caracteres por línea (C.c.p.l.).
* **Narrativa de Fórmula (Paso a Paso):** Desglose pedagógico de las conversiones matemáticas (de golpes a renglones, a puntos, a milímetros, a centímetros y finalmente a la extensión en páginas).
* **Anatomía Interactiva del Interlineado:** Un entorno visual para manipular la línea base, altura x, ascendentes y descendentes, ilustrando de forma práctica la relación directa entre el tamaño de cuerpo y el interlineado.
* **Módulo de Factor Puntaje (F.p.):** Incluye tablas de referencia integradas y una mini-herramienta auxiliar para calcular empíricamente el F.p. directo desde Adobe InDesign.
* **Sistema de Envío:** Generación automática de reportes de evaluación vía correo electrónico o exportación nativa a PDF (con hoja de estilos de impresión optimizada) para la entrega de trabajos prácticos.

## 🛠️ Arquitectura Técnica

El proyecto está construido bajo una arquitectura *Zero-Dependency* (sin librerías de terceros) en un único archivo fuente, ideal para garantizar su portabilidad y fácil distribución en entornos académicos:

* **HTML5:** Estructura semántica.
* **CSS3:** Uso de variables nativas (`:root`), diseño responsivo (Grid/Flexbox), efectos *glassmorphism* y estilos específicos para impresión (`@media print`).
* **Vanilla JavaScript (ES6):** Lógica de cálculo, manipulación del DOM, validación de formularios, *Intersection Observers* para animaciones de lectura y codificación de URL para el protocolo `mailto:`.
* **Tipografía (Google Fonts):** Uso estratégico de *Syne* (titulares), *DM Sans* (cuerpo de lectura) y *JetBrains Mono* (datos técnicos, métricas y fórmulas).

## 🚀 Instalación y Uso

Dado que es un documento estático, no requiere servidor local, base de datos ni configuración de entorno.

1.  **Ejecución:** Simplemente abre el archivo `index.html` (o el nombre que le hayas asignado) en cualquier navegador web moderno (Chrome, Firefox, Safari, Edge).
2.  **Implementación en clase:** Proporciona el archivo a los alumnos o alójalo en una plataforma LMS (como Canvas o Moodle). 
3.  **Evaluación:** Al finalizar un ejercicio, el alumno utiliza el botón **"Enviar por Correo"**. La herramienta agrupará las variables de entrada y los pasos del resultado en un cuerpo de texto estructurado, abriendo el cliente de correo predeterminado del estudiante listo para enviar.

## 👨‍🏫 Contexto Académico

* **Curso:** Diseño Editorial
* **Unidad:** Semana 2
* **Docente / Autor:** Mg. Mario Quiroz (`d3magindesign`)
* **Institución:** Universidad Tecnológica del Perú (UTP) - 2026

> *Esta herramienta forma parte de una iniciativa de innovación educativa orientada a transformar conceptos editoriales abstractos en experiencias visuales e interactivas para la educación superior tecnológica.*