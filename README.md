# Sistema de transacciones financieras por voz en dispositivos móviles iOS

**Alexis Geraldine Barniquez Piñero**
Carrera de Especialización en Inteligencia Artificial
Laboratorio de Sistemas Embebidos — Facultad de Ingeniería, UBA
Director: Ing. Sergio Ivaldi

---

## Descripción del proyecto

Este repositorio contiene la memoria del Trabajo Final de la Carrera de Especialización en Inteligencia Artificial. El trabajo presenta una prueba de concepto de una aplicación móvil nativa para iOS que integra un pipeline de Inteligencia Artificial capaz de procesar comandos de voz e interpretar intenciones transaccionales de forma 100% local, sin enviar datos a servidores externos.

El sistema fue diseñado para eliminar barreras de accesibilidad y promover la inclusión financiera, orientado a los usuarios de banca minorista del Banco Galicia, con especial foco en personas con diversidades funcionales visuales o motoras.

### Tecnologías utilizadas

- **Swift / Xcode** — desarrollo nativo iOS
- **AVFoundation** — captura segura de audio
- **Core ML** — ejecución local de modelos de IA
- **Procesamiento de Lenguaje Natural (NLP)** — reconocimiento automático de habla y comprensión de intenciones transaccionales

---

## Estructura del repositorio

```
├── memorianueva.tex          # Documento principal LaTeX
├── portada.tex               # Portada del documento
├── memorianueva.bib /
│   references.bib            # Referencias bibliográficas
├── MastersDoctoralThesis.cls # Clase LaTeX de la plantilla
├── Chapters/
│   ├── Chapter1.tex          # Introducción general
│   ├── Chapter2.tex          # Marco teórico / Estado del arte
│   ├── Chapter3.tex          # Diseño e implementación
│   ├── Chapter4.tex          # Resultados y validación
│   └── Chapter5.tex          # Conclusiones
├── Appendices/
│   └── AppendixA.tex         # Apéndices (opcional)
├── Figures/                  # Imágenes y figuras del documento
├── Instructivo Overleaf.md   # Guía para compilar en Overleaf
└── LICENSE
```

---

## Cómo usar esta plantilla

> Esta plantilla está basada en la [plantilla oficial del LSE-FIUBA](https://github.com/TTAA-TTFB/Plantilla-para-memoria). Si querés usarla para tu propia memoria, seguí estos pasos.

### Opción A: compilar en Overleaf (recomendado)

Consultá el instructivo detallado en [`Instructivo Overleaf.md`](./Instructivo%20Overleaf.md). En resumen:

1. Crear una cuenta en [Overleaf](https://www.overleaf.com).
2. Descargar este repositorio como `.zip`.
3. En Overleaf: **New Project → Upload Project** y subir el `.zip`.
4. Compilar con el botón **Recompile**.
5. Descargar el PDF generado.

### Opción B: compilar localmente

Requiere una distribución LaTeX instalada (TeX Live, MiKTeX, etc.) y el compilador `pdflatex` o `lualatex`.

```bash
pdflatex memorianueva.tex
biber memorianueva
pdflatex memorianueva.tex
pdflatex memorianueva.tex
```

---

## Personalizar la plantilla para tu memoria

### 1. Portada — `portada.tex`

Completar los siguientes campos:

| Campo | Descripción |
|---|---|
| Título | Título del trabajo final |
| Autor | Nombre completo con título de grado |
| Carrera | Descomentar la carrera correspondiente |
| Director | Nombre, título y pertenencia |
| Jurados | Nombres y pertenencia de los tres jurados |
| Fecha | Ciudad, mes y año de presentación |

### 2. Resumen — `memorianueva.tex`

Dentro del entorno `\begin{abstract}...\end{abstract}`, reemplazar el texto con el resumen propio. Debe ser conciso y sin formato (sin negritas ni cursivas).

### 3. Capítulos — carpeta `Chapters/`

Cada archivo `ChapterN.tex` corresponde a un capítulo. Editarlos según la estructura de la memoria:

- `Chapter1.tex` — Introducción general
- `Chapter2.tex` — Marco teórico
- `Chapter3.tex` — Diseño e implementación
- `Chapter4.tex` — Resultados
- `Chapter5.tex` — Conclusiones

### 4. Figuras

Colocar todas las imágenes en la carpeta `Figures/` e incluirlas en el texto con:

```latex
\begin{figure}[h]
    \centering
    \includegraphics[width=0.8\textwidth]{Figures/nombre_imagen}
    \caption{Descripción de la figura}
    \label{fig:etiqueta}
\end{figure}
```

### 5. Bibliografía

Agregar las referencias en `references.bib` en formato BibTeX e incluirlas en el texto con `\cite{clave}`.

---

## Licencia

Este proyecto está bajo la licencia incluida en el archivo [`LICENSE`](./LICENSE).
