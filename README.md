# Recursos literarios: inventario y vault

Base de datos en Markdown con **1.569 recursos literarios y figuras retóricas**, organizados en **31 familias**: tropos, figuras de dicción y de pensamiento, recursos fónicos y métricos, narratología, argumentación, tópicos, intertextualidad, estilos de época, procedimientos de vanguardia, recursos gráficos, enunciación y poéticas no grecolatinas (nórdica, árabe-persa, sánscrita, china, japonesa, hebrea y céltica).

> **Todos los ejemplos están en castellano.** Los textos originales en otras lenguas (latín, griego, inglés, francés, italiano, árabe, japonés…) se dan traducidos al castellano y van marcados con «(trad.)».

## Contenido de cada recurso

Cada entrada tiene:

- **Nombre**, con su etimología y las variantes terminológicas.
- **Definición** en una a tres frases.
- **Ejemplo** en castellano, dado como texto directo y con una atribución breve.
- **Por qué encaja**: el rasgo concreto del ejemplo que corresponde a la definición.
- **Detección**: cómo se localiza el recurso en un texto (`auto`, `pistas` o `lectura`).

Marcas de los ejemplos:

| Marca | Significado |
|---|---|
| «(trad.)» | Traducción al castellano de un original en otra lengua |
| «(a partir de…)» | Cita adaptada o resumida de la obra indicada |
| «(ejemplo construido)» | Ejemplo inventado para ilustrar el recurso, cuando no hay uno canónico breve o el recurso depende de la lengua original |

## Estructura del repositorio

```
├── README.md
├── Inventario_recursos_literarios.pdf   # Inventario completo maquetado (292 páginas)
├── 00 Índice.md                         # Mapa navegable de los 1.569 recursos
├── 01 Cómo usar el vault.md             # Flujo de análisis de una obra
├── 02 Pistas de detección.md            # Reglas formales para localizar recursos en un texto
├── 03 Lista compacta.md                 # Una línea por recurso: familia | nombre | detección
├── Familias/                            # 31 fichas, una por familia; cada recurso es un encabezado ##
├── Obras/                               # Textos que se van a analizar
└── Análisis/                            # Informes de análisis generados
```

## Niveles de detección

| Nivel | Recursos | Descripción |
|---|---|---|
| `auto` | 302 | Se localizan mecánicamente: repeticiones, rima, aliteración, preguntas y exclamaciones, medida del verso, formas estróficas, acrósticos |
| `pistas` | 334 | Hay marcadores léxicos o de puntuación que permiten seleccionar candidatos («como», «¡oh!», «no diré», diminutivos, deícticos) |
| `lectura` | 933 | Requieren interpretación: tropos, ironía, tópicos, narratología, argumentación, estilos |

## Uso

- **Con Obsidian:** abre la carpeta como vault. Los enlaces `[[Familias/…#Recurso]]` llevan directamente a la ficha de cada recurso.
- **Sin Obsidian:** son archivos Markdown normales y se pueden leer en GitHub o en cualquier editor.
- **Para analizar una obra:** sigue el flujo descrito en [`01 Cómo usar el vault.md`](01%20Cómo%20usar%20el%20vault.md).

## Fuentes principales

Aristóteles (*Poética*, *Retórica*), *Retórica a Herenio*, Cicerón, Quintiliano, Hermógenes, H. Lausberg (*Manual de retórica literaria*), B. Mortara Garavelli (*Manual de retórica*), J. A. Mayoral (*Figuras retóricas*), H. F. Plett, Grupo μ (*Retórica general*), G. Genette (*Figures III*, *Palimpsestes*), E. R. Curtius, M. Bajtín, T. Todorov, D. Cohn, W. Booth y otros. La bibliografía completa está al final del PDF.

## Aviso

Las citas proceden de ediciones de uso común y se han revisado durante la redacción, pero no se han cotejado una por una con ediciones críticas. Conviene verificar las que vayan a citarse textualmente en un trabajo académico.
