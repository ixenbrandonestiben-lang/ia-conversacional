# ¿Cómo funciona un Transformer en la IA?

## El “cerebro” detrás de ChatGPT, Claude y Gemini

Un Transformer es una arquitectura de IA que permite a los modelos de lenguaje entender texto, relacionar palabras y generar respuestas.

---

## Flujo del funcionamiento

```text
ENTRADA DE TEXTO
        ↓
TOKENIZACIÓN
        ↓
EMBEDDINGS
        ↓
ENCODER
        ↓
SELF-ATTENTION
        ↓
FEED-FORWARD
        ↓
SALIDA
```

---

## 1. Entrada de texto

La persona escribe una pregunta o instrucción.

**Ejemplo:**

```text
“Explícame qué es la fotosíntesis”
```

La IA recibe ese texto para procesarlo.

---

## 2. Tokenización

El texto se divide en piezas pequeñas llamadas **tokens**.

Un token puede ser una palabra completa o una parte de una palabra.

**Ejemplo:**

```text
“Explícame qué es la fotosíntesis”

→ [“Explícame”] [“qué”] [“es”] [“la”] [“fotosíntesis”]
```

---

## 3. Embedding

Cada token se convierte en una lista de números.

A eso se le llama **embedding**.

Sirve para que la IA pueda entender el significado de las palabras.

**Ejemplo:**

```text
“gato”  → [0.21, 0.87, 0.34, ...]
“perro” → [0.19, 0.85, 0.30, ...]
```

Palabras parecidas tienen números parecidos.

También se agrega información sobre la **posición** de cada palabra, porque el orden cambia el significado.

**Ejemplo:**

```text
“El perro mordió al gato”
“El gato mordió al perro”
```

Las palabras son casi las mismas, pero el significado cambia.

---

## 4. Encoder

El **encoder** analiza la frase completa y crea una representación del contexto.

No solo entiende cada palabra por separado, sino cómo se relacionan entre sí.

**Ejemplo:**

```text
“El banco estaba cerca del río”
```

La IA entiende que “banco” probablemente significa un asiento, no una institución financiera.

---

## 5. Self-attention

La **self-attention** o autoatención permite que cada palabra “mire” a las demás.

Así el modelo sabe qué palabras son importantes para entender una frase.

**Ejemplo:**

```text
“Ana le dio su libro a María porque ella lo había pedido”
```

La IA relaciona:

```text
“ella” → “María”
“lo”   → “libro”
```

Esto ayuda a la IA a entender relaciones incluso si las palabras están lejos una de otra.

### Componentes de la self-attention

| Componente | Función |
|---|---|
| Query | Qué información busca una palabra |
| Key | Qué información ofrece cada palabra |
| Value | Qué contenido entrega cada palabra |

La IA compara las *queries* con las *keys* y decide a qué palabras prestar más atención.

---

## 6. Feed-forward

Después de la self-attention, la información pasa por una **red feed-forward**.

Esta parte transforma y refina lo que la IA entendió.

**Idea simple:**

```text
Self-attention → entiende relaciones
Feed-forward   → procesa y mejora esa información
```

Estas operaciones se repiten muchas veces dentro del modelo.

---

## 7. Salida

La salida depende de lo que se pidió al modelo.

| Tipo de modelo | Entrada | Salida |
|---|---|---|
| Encoder | Texto | Clasificación, búsqueda o análisis |
| Decoder | Texto previo | Predicción de la siguiente palabra |
| Encoder-decoder | Texto fuente | Traducción o resumen |

**Ejemplo de salida:**

```text
Pregunta: “¿Qué es la fotosíntesis?”

Respuesta: “Es el proceso por el cual las plantas
usan luz solar, agua y dióxido de carbono
para producir energía y oxígeno.”
```

El modelo genera la respuesta **palabra por palabra** o **token por token**.

---

## Ejemplos de LLM conversacionales

Los **LLM** son modelos de lenguaje grandes.

Muchos usan arquitecturas Transformer para conversar, responder preguntas, escribir textos y analizar información.

| LLM | Empresa | Ejemplo de uso |
|---|---|---|
| **ChatGPT** | OpenAI | “Explícame la fotosíntesis como si tuviera 10 años” |
| **Claude** | Anthropic | “Resume este contrato y dime los riesgos” |
| **Gemini** | Google | “Busca información actual y haz un resumen con fuentes” |
| **Llama** | Meta | “Ayúdame a escribir un correo profesional” |
| **Mistral** | Mistral AI | “Convierte estas notas en un plan de trabajo” |
| **DeepSeek** | DeepSeek | “Explícame este código de Python” |

---

## Clasificación de los mejores LLM

No existe un único “mejor LLM”.

La mejor opción depende de lo que necesites hacer.

| Categoría | Mejores opciones | Para qué sirve |
|---|---|---|
| **Conversación general** | ChatGPT, Claude, Gemini | Preguntas, explicaciones y redacción |
| **Razonamiento complejo** | Claude Opus, GPT, Gemini Pro | Análisis, planeación y problemas difíciles |
| **Programación** | Claude, GPT, DeepSeek | Escribir, revisar y depurar código |
| **Documentos largos** | Gemini, Claude | Resumir libros, reportes y contratos |
| **Multimodal** | Gemini, GPT | Texto, imágenes, audio y documentos |
| **Código abierto** | Llama, Mistral, Qwen, DeepSeek | Privacidad y uso local |
| **Búsqueda con fuentes** | Perplexity, Gemini, ChatGPT | Respuestas actuales con referencias |

---

## Top práctico

- **Para conversar y aprender:** ChatGPT, Claude o Gemini.
- **Para analizar textos largos:** Claude o Gemini.
- **Para programar:** Claude, GPT o DeepSeek.
- **Para trabajar dentro de Google:** Gemini.
- **Para privacidad o uso local:** Llama, Mistral, Qwen o DeepSeek.
- **Para respuestas con fuentes:** Perplexity, Gemini o ChatGPT con búsqueda.

---

## Idea visual para la infografía

```text
TÚ ESCRIBES
     ↓
LA IA DIVIDE EL TEXTO
     ↓
LO CONVIERTE EN NÚMEROS
     ↓
RELACIONA LAS PALABRAS
     ↓
ENTIENDE EL CONTEXTO
     ↓
ELIGE LA MEJOR RESPUESTA
     ↓
TE RESPONDE
```

---

## Frase final para la infografía

> **Los Transformers convierten el texto en números, usan la self-attention para entender las relaciones entre palabras y generan respuestas basadas en el contexto.**
>
> **Ejemplos de LLM conversacionales: ChatGPT, Claude, Gemini, Llama, Mistral y DeepSeek.**