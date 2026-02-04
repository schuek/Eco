# Abuelos Viajeros - Taller de Ecodiseño Digital

![Estado del Proyecto](https://img.shields.io/badge/Estado-Terminado-success)
![Sostenibilidad](https://img.shields.io/badge/CO2-0.11g-green)
![Lighthouse](https://img.shields.io/badge/Lighthouse-100-orange)

## 1. Descripción del proyecto
En este taller hemos trabajado en equipo para optimizar la landing page "Abuelos Viajeros", una web inicialmente pesada y poco eficiente. Aplicando principios de ecodiseño digital, hemos transformado el sitio para reducir el consumo de recursos, mejorar drásticamente el rendimiento y disminuir el impacto ambiental.

La web final ha sido desplegada en Netlify, simulando un entorno de hosting eficiente y alineado con buenas prácticas de sostenibilidad digital.

---

## 2. Análisis inicial (El Problema)
En la versión original detectamos varios problemas de alto impacto digital:
* **Imágenes gigantes:** Archivos JPG sin optimizar (algunos superiores a 5MB) y sin atributos de carga diferida.
* **Peso innecesario:** Código CSS redundante y estilos antiguos (Times New Roman por defecto).
* **Bloqueo de renderizado:** Carga de todos los elementos al inicio, bloqueando la visualización en dispositivos móviles.
* **Huella de Carbono:** Emisiones estimadas de 1.20g de CO2 por visita.

Estas características provocaban una mala experiencia de usuario y un alto consumo energético.

---

## 3. Acciones de optimización realizadas
Durante el proceso de ecodiseño se aplicaron las siguientes mejoras técnicas:

### 3.1. Optimización de imágenes
* **Conversión a WebP:** Pasamos de JPG/PNG a WebP, reduciendo el peso en un 85% sin pérdida visual.
* **Lazy Loading:** Implementamos el atributo loading="lazy" en las imágenes secundarias para ahorrar ancho de banda.
* **Atributos de dimensión:** Definimos width y height para evitar saltos de contenido (CLS).

### 3.2. Optimización del código (Tailwind CSS)
* **HTML Semántico:** Estructura simplificada y limpia.
* **Tailwind CSS:** Uso de arquitectura "Utility-First". El archivo output.css generado está minificado y purgado, conteniendo solo las clases que realmente se usan.
* **JavaScript:** Scripts diferidos (defer) y eliminación de código bloqueante.

### 3.3. Gestión de recursos
* Reducción drástica de peticiones HTTP.
* Control de versiones con Git/GitHub, evitando subir archivos pesados (node_modules) gracias a una correcta configuración de .gitignore.

---

## 4. Resultados obtenidos (Métricas)

| Métrica | ANTES | DESPUÉS |
| :---                          | :---:      | :---: |
| **Tiempo de Carga**           | +3.4 s     | **0.8 s** |
| **Peso de Página**            | ~5 MB      | **< 500 KB** |
| **Lighthouse (Rendimiento)**  | Bajo (<50) | **100 / 100** |
| **Huella de Carbono**         | 1.20 g     | **0.11 g** |
| **Clasificación Ecológica**   | F          | **A+ (Top 5% mundial)** |

*Datos verificados con Google Lighthouse y Website Carbon Calculator.*

## 7. Créditos y Autores
Trabajo realizado para el Taller de Ecodiseño Digital.
* **Diseño y Optimización:** Diego
* **Gestión de Reservas:** Karen
* **Módulo Social:** Dani