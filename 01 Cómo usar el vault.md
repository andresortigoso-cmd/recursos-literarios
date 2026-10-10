---
tags: [guia]
---

# Cómo usar el vault

Base de consulta para localizar recursos literarios en una obra concreta. Contiene **1.569 recursos** en **31 familias**, todos con definición, ejemplo en español y explicación de por qué el ejemplo encaja.

## Estructura

| Archivo | Para qué sirve | Coste de lectura |
|---|---|---|
| [[00 Índice]] | Mapa navegable: cada recurso enlaza a su ficha | Medio |
| [[02 Pistas de detección]] | Marcadores formales (palabras, puntuación, patrones) para buscar recursos sin leer el texto entero | Bajo |
| [[03 Lista compacta]] | Una línea por recurso: `familia \| nombre \| detección` | Muy bajo |
| `Familias/` | 31 fichas con definición, ejemplo y explicación de cada recurso | Alto (se consultan solo cuando hace falta) |

## Niveles de detección

Cada recurso está marcado con uno de tres niveles:

- `auto` (302): se puede localizar mecánicamente con un script. Son repeticiones, rimas, aliteraciones, preguntas y exclamaciones, enumeraciones, cómputo silábico, formas estróficas y juegos gráficos.
- `pistas` (334): hay marcadores que permiten preseleccionar candidatos, como «como», «cual», «¡oh!», vocativos, diminutivos, negaciones o verbos de habla. Después hay que confirmarlos leyendo el contexto.
- `lectura` (933): solo se identifican interpretando el texto. Entran aquí los tropos, la ironía, los tópicos, la narratología, los símbolos, la argumentación y los estilos de época.

## Flujo de análisis de una obra (ahorro de tokens)

1. **Recibir la obra** en un archivo de texto (`.txt` o `.md`) y guardarla en la carpeta `Obras/`.
2. **Pasada automática:** un script recorre la obra con las reglas de [[02 Pistas de detección]] y devuelve solo los fragmentos candidatos, con su número de línea. Claude no lee la obra completa en esta fase.
3. **Confirmación:** Claude revisa únicamente los candidatos y descarta los falsos positivos. Si duda, consulta la ficha concreta en `Familias/`.
4. **Pasada de lectura:** para los recursos `lectura`, Claude lee la obra por bloques y la contrasta con [[03 Lista compacta]], no con las fichas completas. Solo abre una ficha cuando tiene que confirmar una definición dudosa.
5. **Informe:** se genera un `.md` en `Análisis/` con cada recurso encontrado, la cita, la línea o la página y un enlace a su ficha (`[[Familias/…#Recurso]]`).

## Convenciones de las fichas

- Cada recurso es un encabezado `##`. Se enlaza desde cualquier nota con `[[Familias/03 Figuras de dicción por repetición (adiectio)#Anáfora]]`.
- La línea en cursiva bajo el nombre recoge la etimología y las variantes terminológicas.
- En los ejemplos, «(trad.)» marca una traducción; «(a partir de…)», una cita adaptada o resumida; «(ejemplo construido)», un ejemplo inventado.
- «semilla» indica que el recurso estaba en la lista inicial de referencia.
