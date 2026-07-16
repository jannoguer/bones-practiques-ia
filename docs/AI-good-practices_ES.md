# BUENAS PRÁCTICAS CON LA IA

<p align="center"><i>"La IA no es inteligente, es culta."</i></p>

Guía breve para sacar más partido a la IA en el día a día. Las respuestas de la IA no son siempre correctas: puede cometer errores incluso teniendo la información correcta.

## Estructura de los prompts

Persona *(opcional)* → **Contexto** → **Tarea** → **Formato**

> [!TIP]
> ¡La misma IA puede hacerte los prompts!

**Ejemplo:** Eres un experto en atención al cliente *(←Persona)*. Nuestra empresa acumula retrasos graves en los pedidos por un problema con la mensajería y varios clientes se han quejado *(←Contexto)*. Redacta un mensaje de disculpa para calmarlos *(←Tarea)* presentado como una plantilla con espacios para rellenar *(←Formato)*.

> [!NOTE]
> El primer prompt raramente da el resultado deseado a la primera, hay que seguir la conversación pidiendo ajustes hasta llegar a él.

> [!NOTE]
> Adjuntar ejemplos mejora los prompts significativamente.

## Trabajos pesados

<p align="center"><i>"No dejes que la IA haga el trabajo, utilízala para crear las herramientas que lo harán."</i></p>

### Mal

**Ejemplo:** "Elimina los duplicados y ordena alfabéticamente los correos de esta lista: ..."

**Resultado:** Omisión de información, alucinaciones, imprecisión, degradación de la atención, truncamiento de la respuesta, etc.

### Correcto

**Ejemplo:** "Crea un programa en Python para eliminar los duplicados y ordenar alfabéticamente los correos de esta lista: ..."

**Resultado:** Lista correctamente estructurada y con todos los datos. Además, puedes repetir el mismo procedimiento con una nueva lista (si mantiene el formato, claro).

<p align="center">EL PROGRAMA NO LEE LA INFORMACIÓN, LA PROCESA.</p>

## Cambios en archivos grandes

No puedes esperar que la IA te genere un archivo de 2.000 líneas entero, sin errores y de golpe a través del chat.

Si los cambios son pequeños, **pide solo las líneas modificadas**.

Si son muchos cambios, hay **dos opciones**:
* **Pedir el archivo actualizado para descargar:** Solicita que te ofrezca un botón de descarga con el documento listo (no todas las IA lo permiten).
* **Trabajar en local:** Plantéate utilizar la IA directamente desde el escritorio (en lugar de la versión web) para poder editar los archivos directamente desde el disco duro.

## Reglas de la sesión

A medida que la conversación crece, la ventana de contexto se llena y la calidad de las respuestas se degrada. Por eso conviene empezar de cero a menudo:

* **Tarea finalizada**: Iniciar una **nueva sesión**.
* **La IA alucina**: Desplegar **prompt "handoff"** → Iniciar una **nueva sesión** *(con resumen + archivos requeridos)*.

> [!NOTE]
> Un **prompt "handoff"** es una instrucción que le pides a la IA antes de cerrar la sesión para que resuma el estado del trabajo (qué se ha hecho, qué queda y qué archivos hacen falta), de manera que puedas pegar ese resumen en la sesión nueva y continuar sin perder contexto.

## Glosario

* **Prompt**: la instrucción o texto que le escribes a la IA.
* **Ventana de contexto**: todo lo que la IA "recuerda" dentro de una misma conversación. Tiene un límite y, cuando se llena, la calidad de las respuestas baja.
* **Token**: la unidad en la que la IA mide el texto. El cálculo real es complicado, pero como regla simple: unas 3 palabras equivalen aproximadamente a 4 tokens (según el idioma).
