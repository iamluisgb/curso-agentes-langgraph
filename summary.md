# LangGraph


## Fundamentos de LangGraph

### Cómo construir agentes inteligentes con LangGraph

Los agentes de inteligencia artificial están redefiniendo el desarrollo de software con **sistemas robustos que razonan, deciden y ejecutan tareas**. Con LangGraph pasas de manipular un *large language model* potente pero impredecible a **construir un sistema confiable**, con una **arquitectura cognitiva** que te da balance, estructura y control reales.

¿Por qué LangGraph es clave para agentes de inteligencia artificial?

LangGraph no es “otra librería”. Es la base para **conectar un *large language model* con un sistema de grafos** y permitir que el agente **tome decisiones** y **derive patrones avanzados** de forma transparente y controlada.

- Construcción de agentes verdaderamente inteligentes.
- Decisiones guiadas por un sistema de grafos.
- Patrones avanzados sin comportamientos opacos.
- Robustez y confiabilidad sobre simples chats.

¿Qué problemas resuelve frente a respuestas impredecibles?

Un *large language model* puede ser poderoso y a la vez impredecible. LangGraph **aporta estructura al razonamiento y a la toma de decisiones**, reduciendo la variabilidad y dando **consistencia al comportamiento del agente**.

- Respuestas menos erráticas y más útiles.
- Rutas de decisión explícitas y auditables.
- Agentes que ejecutan tareas completas y repetibles.

¿Cómo funciona la arquitectura cognitiva y el control del estado?

En muchos *frameworks*, la derivación del **estado** y la **toma de decisiones** parecen una **caja negra**. Con LangGraph, esa caja se abre. Tienes **balance, estructura y control** sobre cómo el agente **deriva su estado** y **decide qué hacer** en cada paso.

- La arquitectura cognitiva la manipulas tú.
- El *framework* te asiste con utilidades, no decide por ti.
- Transparencia total en el flujo del agente.

¿Qué significa evitar la caja negra en un framework?

Significa que el **cerebro del agente** no está oculto. Puedes **ver, ajustar y dirigir** cómo se forman las decisiones y cómo evoluciona el estado.

- Control explícito del flujo de razonamiento.
- Ajustes finos sin perder trazabilidad.
- Resultados alineados con tus reglas.

¿Qué habilidades desarrollarás para crear y automatizar con agentes?

El reto es **pasar de consumidor a creador** de esta nueva generación de sistemas. Diseñarás agentes que **toman decisiones por sí mismos**, **realizan tareas** y **automatizan procesos completos**, ahorrando **horas de trabajo** con inteligencia artificial.

- Diseño de agentes de inteligencia artificial.
- Modelado de estados y decisiones.
- Uso de un sistema de grafos para control lógico.
- Automatización de procesos de principio a fin.
- Creación de tu primer agente con guía paso a paso.

### Configuración de entorno Python y primer agente con LangGraph

Aprende a montar un entorno Python 3 seguro, instalar LangGraph y LangChain con su integración para OpenAI, y lanzar tu primer agente con el *debugger* de LangGraph. Siguiendo la documentación oficial, el flujo es directo y estable, incluso si usas la versión pre-release: el código no cambia.

¿Cómo preparar el entorno en Python 3 con entorno virtual?

Para evitar conflictos y asegurar compatibilidad, se recomienda **Python 3** (mejor 3.12; también sirven 3.8 o 3.10). La base es crear una carpeta de proyecto y un **entorno virtual**.

- Crear la carpeta: my-course-agent.
- Entrar con cd my-course-agent.
- Verificar versión: Python 3 instalado y activo.
- Crear un entorno virtual con python3 y nombrarlo .env.
- Activar el entorno: source .env/bin/activate.
- Comprobar con which python que apunta al .env y no al global.

Claves y habilidades: - **Entorno virtual**: aísla dependencias del proyecto. - **which python**: valida que el intérprete activo es el del .env.

¿Qué instalar de LangChain y LangGraph para el primer agente?

Desde la documentación en docs.langchain.com, instala los paquetes necesarios. Puede aparecer un aviso de **pre-release**; si está, usa la bandera pre. Si ya salió la versión estable, instala sin esa bandera: el **código no cambia**.

- Paquetes a instalar: **LangGraph**, **LangChain** y **LangChain con OpenAI**.
- Si ves el alert de versión alfa: añade la bandera pre.
- Si no ves el alert: instala sin pre.

¿Qué rol tiene LangGraph y LangChain en el ecosistema?

La arquitectura distingue dos niveles para agentes:

- **LangChain**: un agente individual, el “átomo” operativo.
- **LangGraph**: orquestador de múltiples agentes.

Esta separación te permite crear primero un agente con LangChain y después **orquestarlo** con LangGraph.

¿Cómo crear y ejecutar tu primer agente con OpenAI GPT-4?

El flujo incluye preparar el archivo principal, configurar la **API key** y lanzar el *debugger* con la **CLI** de LangGraph.

¿Cómo definir el agente en main.py con OpenAI?

Parte de un ejemplo de “primer agent” de la sección de LangChain y adáptalo:

- Crear el archivo main.py en tu editor.
- Pegar el ejemplo del “primer agent”.
- Cambiar el proveedor del ejemplo de Anthropic a **OpenAI** con **GPT-4**.

Conceptos clave: - **Agente individual**: corre en LangChain. - **GPT-4**: modelo de OpenAI al que te conectarás.

¿Cómo configurar la API key en un archivo .env?

Para conectarte a modelos como **OpenAI**, **Anthropic** o **Gemini**, necesitas una **API key**.

- Crear un archivo .env en la raíz del proyecto.
- Añadir tu key: la variable para OpenAI debe identificarse como su API key.
- Generar la key en el dashboard del proveedor y pegarla en .env.

Buenas prácticas en contexto: - **Variables de entorno**: no cargues claves en el código. - **.env**: centraliza secretos para usarlos desde herramientas y configuración.

¿Cómo usar el *debugger* de LangGraph con su CLI?

Instala la herramienta de comandos para el entorno de *debugging* y prepara la configuración.

- Instalar “LangGraph CDI” sin la bandera pre.
- Crear un archivo de configuración: langgraph.gist.
- Incluir en la configuración: dependencias (.), carga del archivo .env y definición de los “grafos”.
- Definir un grafo con nombre, por ejemplo “agent”, que apunte al agente en main.py.
- Quitar el bloque que corre el agente directamente: lo arrancarás con el *debugger*.

Ejecución y prueba: - Con el entorno virtual activo, correr: langgraph dev. - Si aparece un error de dependencia, instala lo que falta y repite. - Abre la URL de la **Studio UI** que aparece en la terminal. - Verás tu agente listado con sus *tools*. - Envía un mensaje, por ejemplo: “Hola, ¿cómo estás?”. Debes ver la respuesta del modelo y el trazo del flujo en el *debugger*.

Palabras clave y habilidades en acción: - **CLI de LangGraph**: comando langgraph dev para levantar el entorno de desarrollo. - **Studio UI**: interfaz visual para *debugging* de agentes. - **tools**: capacidades del agente visibles en la interfaz. - **orquestación**: posteriormente LangGraph coordina múltiples agentes basados en LangChain.

### Configuración de uv para escalar agentes de IA en producción

Escalar agentes de IA exige una **arquitectura profesional**, gestión confiable de **dependencias** y una **API** lista para producción. Aquí aprenderás a pasar de varios prototipos a un proyecto robusto: instalación de un gestor moderno llamado uv, separación de dependencias de desarrollo, configuración de **carpetas** y uso de **LangGraph Studio** y *notebooks* para depurar y visualizar grafos.

¿Cómo escalar agentes con una arquitectura profesional?

Adoptar una arquitectura modular evita fricciones al orquestar **múltiples agentes**, moverlos a producción y exponerlos en una **API**. La clave: configurar un gestor de paquetes moderno (uv), ordenar el repositorio y preparar herramientas de desarrollo como *notebooks* y observabilidad.

¿Qué problemas resuelve el gestor de paquetes uv?

- Reemplaza tareas dispersas que antes se hacían con **pip**, pip tools, **Poetry** y **Virtualenv**.
- Gestiona **ambientes** y **dependencias** de forma ligera y profesional.
- Acelera la instalación: uv es aproximadamente diez veces más rápido que pip.
- Centraliza la configuración con un archivo tipo **project.toml** y **.gitignore**.

¿Cómo se instala y verifica uv en el sistema?

- Instálalo según tu sistema operativo: **Mac/Linux** o **Windows** con WSL Ubuntu.
- Verifica la versión instalada:
    
    uv version
    
- Si tienes un *virtualenv* previo, desactívalo y elimínalo para que **uv** gestione el entorno:
    
    Desactivar (ejemplo clásico)
    
    source /bin/deactivate
    
    Eliminar la carpeta del entorno
    
    RMF
    
- Inicializa el proyecto y genera archivos base como **project.toml** y **.gitignore**:
    
    uv init
    

¿Qué buenas prácticas de repositorio se aplican?

- Ignorar carpetas internas no necesarias para el código fuente (ejemplo: la de LangGraph).
- Ignorar variables de entorno para proteger tus keys:
    - .env
- Definir explícitamente la **versión de Python** y separar dependencias de producción y desarrollo en el **project.toml**.

¿Cómo gestionar dependencias y entornos para producción y desarrollo?

Separar lo que necesitas para correr en producción de lo que usas para desarrollar evita empaquetar de más y reduce riesgos.

¿Cómo agregar dependencias con uv add?

- Sustituye pip install por el nuevo comando:
    
    uv add
    
- Reinstala las dependencias del proyecto con uv si eliminaste el entorno anterior.

¿Cómo separar dependencias de desarrollo como LangGraph CLI y Jupyter?

- El **CLI** se usa solo en desarrollo.
- Agrega el *kernel* de **Jupyter** para experimentos con *notebooks*, *tools* y flujos de agentes:
    
    Dependencias de desarrollo (ejemplo)
    
    uv add --dev uv add jupyter --dev
    
- Visualiza en el **project.toml** qué es producción y qué es desarrollo.

¿Cómo ejecutar y verificar con uv run y LangGraph Studio?

- En lugar de activar/desactivar el entorno, ejecuta directo con uv:
    
    uv run
    
- Si usas **LangGraph**, el flujo clásico de desarrollo es:
    
    langgraph dev
    
- Ante errores de puerto ocupado, detén el proceso previo y vuelve a correr. Abre **LangGraph Studio** y crea un **thread** nuevo para probar el agente con un “hola”.

¿Cómo organizar el proyecto para orquestar varios agentes y exponer una API?

Una estructura clara permite añadir agentes, *tools*, conexiones y una **API** sin romper nada. Además, facilita el uso de *notebooks* para visualización y pruebas.

¿Qué estructura de carpetas y módulos usar (CDC, agents, api, notebooks)?

- Crea una carpeta raíz, por ejemplo **CDC**.
- Dentro de CDC, crea:
- **agents**: mueve aquí el archivo principal (por ejemplo, main) y futuros agentes.
- **api**: el paquete para exponer los agentes vía **API**.
- **notebooks**: centraliza todos los *notebooks* de laboratorio.
- Asegúrate de incluir `__init__.py` en cada subcarpeta para que Python los trate como paquetes.

¿Cómo configurar project.toml para descubrir paquetes?

- Añade en el **project.toml** la sección que indica dónde buscar todos los paquetes y módulos del proyecto, sin importar la profundidad. Esto hace que Python “vea” correctamente CDC/agents, CDC/api y otros submódulos.
- Tras mover archivos, actualiza los imports según la nueva ruta de paquete, por ejemplo: `agents.main`.

¿Cómo compilar e integrar notebooks y visualización de grafos?

- Si un *notebook* no encuentra módulos tras reorganizar carpetas, reinicia el *kernel* y “compila/instala” el proyecto localmente:
    
    install
    
- En *notebooks*, puedes importar el agente desde `agents.main` y visualizar su **grafo**. Si la imagen en formato PNG falla por depender de un servidor externo, solicita el **formato** del grafo y pégalo en la página sugerida para renderizarlo.
- Usa **threads** en LangGraph Studio para orquestar conversaciones en paralelo y depurar cómo fluye el grafo.

Habilidades y conceptos reforzados: orquestación de múltiples agentes, creación de una API para consumo externo, gestión de dependencias con **uv**, separación de entornos de producción y desarrollo, configuración de **.gitignore** y **.env**, manipulación de **project.toml**, uso de **Jupyter** y su *kernel*, depuración con **LangGraph Studio**, visualización de grafos, manejo de **WSL Ubuntu**, reinicio de *notebooks* y recompilación local.

## El Núcleo del Agente: Estado y LLMs

### Como funciona el estado compartido el estado compartido en LangGraph

Aprende a crear agentes que recuerdan, consultan información externa y ejecutan acciones con **LangGraph**. La clave está en un **estado como diccionario compartido**, nodos que lo actualizan de forma controlada y una orquestación con **StateGraph**, **start**, **end** y **edges**. Todo con Python, sin complicaciones, y listo para depurar y visualizar en ASCII.

¿Cómo funciona el estado compartido en LangGraph?

El flujo se basa en una **entrada** (mensaje, archivo u otro input), una **salida** y un **grafo de nodos** en medio. Allí viven el **Language Model**, el **retrieval** para enriquecer con datos como un PDF, una **memoria** y las **tools** que dan “manos” al sistema para ejecutar acciones. El **estado** es una memoria compartida entre nodos, modelada como un diccionario de Python que conviene tipar.

- El estado es un diccionario compartido entre nodos y agentes.
- Se recomienda **tiparlo** para claridad y seguridad.
- Accede con **get** para evitar errores cuando una key no existe.
- Usa valores por defecto como **fallback**.
    

```python
from typing import TypedDict

class State(TypedDict, total=False):
    customer_name: str
    my_age: int

state: State = {}

print(state.get("customer_name"))  # None si no existe.

print(state["customer_name"])  # KeyError si no existe.

name = state.get("customer_name", "desconocido")  # fallback.
```


¿Cómo evitar errores con diccionarios en Python?

- Usa get para leer claves opcionales.
- Define valores por defecto para no romper el flujo.
- Añade claves al estado solo cuando tengas datos válidos.

¿Cómo se define un nodo que actualiza el estado?

Un nodo es, en esencia, una **función de Python** que recibe el estado y **devuelve únicamente las partes del estado que actualiza**. Esta es una buena práctica: no devuelvas todo el estado si no lo modificas por completo. Así evitas confusión y sobreescrituras innecesarias.

- Un nodo lee del estado compartido.
- Actualiza solo lo que necesita.
- Devuelve un diccionario con los cambios.
    

```python
def node_one(state: State) -> dict:
    # Si no hay nombre, lo establece.
    if state.get("customer_name") is None:
        return {"customer_name": "John Doe"}
    # Si ya hay nombre, actualiza otra parte del estado.
    return {"my_age": 30}
```


¿Qué devuelve un nodo en LangGraph?

- Solo las keys del estado que modificó.
- Un diccionario vacío si no hay cambios.
- Nada de “devolver todo” salvo que actualices todo.

¿Cómo construir y visualizar el grafo con StateGraph?

La orquestación usa **StateGraph**: defines nodos, conectas **start → nodo → end** con **edges**, y compilas. Para visualizar sin depender de PNG, puedes usar la opción **ASCII** con la dependencia **Granfold**. En el entorno de depuración, seleccionas el grafo, ves el estado y ejecutas hilos de prueba.

- Grafo con start y end para delimitar el flujo.
- Edges para conectar nodos en orden.
- Compilación para obtener el agente ejecutable.
- Visualización en ASCII para avanzar rápido.
    

```python
# Construcción del grafo
from langgraph.graph import StateGraph, START, END  # Referencia: src/agents/simple.py

builder = StateGraph(State)

builder.add_node("node_one", node_one)

builder.add_edge(START, "node_one")
builder.add_edge("node_one", END)

agent = builder.compile()

# Visualización en notebook:
from IPython.display import Image
Image(agent.get_graph().draw_mermaid_png())
```


¿Cómo probar en el debug y extender el estado?

- Ejecuta sin customer_name: el nodo establece "John Doe".
- Ejecuta con un nombre (por ejemplo, "Nicolás Molina"): el nodo actualiza my_age.
- Reto: añade otra variable al estado (por ejemplo, un array) y, según la lógica del nodo, haz un push o cambia valores en función de condiciones.

### **Gestión de historial de mensajes en LangGraph**

Un buen agente conversacional necesita **memoria confiable**. Aquí verás cómo LangGraph integra el historial en el estado, cómo usar los tipos de mensaje de LangChain y cómo evitar errores comunes en Python al concatenar listas. También conocerás el *messages stage* para **agregar mensajes sin sobrescribir** el historial y probarlo en la interfaz de *debug*.

¿Cómo estructurar el historial de mensajes en LangGraph?

Gestionar el contexto es clave para que la IA responda bien. LangChain ofrece una API de mensajes y LangGraph incorpora el historial como parte del estado compartido. Así, cada nodo conoce la conversación y responde según **el rol del mensaje**.

¿Qué tipos de mensajes existen y para qué sirven?

- **AI message**: respuesta de la IA. Importa el rol para que el *language model* entienda quién habla.
- **Human message**: mensaje de la persona usuaria.
- **System message**: instrucciones del *system prompt* para guiar el modelo.
- **Tool message**: intercambio con herramientas externas.
- **Base message** y **any message**: clases base/agnósticas para tipar listas de mensajes.

Ejemplo mínimo en Python:

```python
# Importar clases de mensajes desde LangChain core (según el proyecto).
from langchain_core.messages import AIMessage, HumanMessage, SystemMessage  # nombres referenciales
ai_msg = AIMessage(content="Hola, ¿en qué te ayudo?")
print(ai_msg.text)  # Propiedad mencionada para extraer el texto.
human_msg = HumanMessage(content="Hola, soy Nicolás.")
```

¿Cómo imprimir y depurar el historial con *prettyprint*?

- Cada mensaje expone un formato legible con *prettyprint*.
- Útil para inspeccionar rápido el estado de la conversación.
    

```python
history = [ai_msg, human_msg]
for msg in history:
    msg.prettyprint()  # Muestra rol y contenido de cada mensaje.
```


¿Cómo concatenar listas en Python sin errores?

- Usa el operador **+** entre listas. Siempre listas.
- Evita sumar un elemento suelto. Envuélvelo en una lista.
- Patrón correcto para agregar al historial: lista + [nuevo_mensaje].
    

```python
history = [human_msg]
new_ai = AIMessage(content="Entendido.")

# Correcto: concatenas listas.
history = history + [new_ai]

# Incorrecto: no puedes sumar un solo objeto directamente.
history = history + new_ai  # Esto daría error.
```


¿Cómo gestionar el estado compartido con *messages stage*?

El *messages stage* de LangGraph estandariza la gestión del historial: **concatena** nuevos mensajes sin reemplazar la lista existente. Funciona como memoria compartida entre nodos, con un protocolo de agregado eficiente.

¿Cómo definir el estado con la key messages?

- El estado incluye la clave **messages** con una lista de mensajes.
- Puedes tiparlo con *base message* o *any message*, o usar directamente el *messages stage* para abstraer la lógica de agregado.
- Al retornar, solo envía lo nuevo a concatenar; el *messages stage* lo agrega al final.

```python
# Referencia: src/agents/support/state.py
from langgraph.graph import MessagesState

class State(MessagesState):
    customer_name: str
    phone: str
    my_age: str

from langchain_core.messages import AIMessage

def node_logic(state):
    respuesta = AIMessage(content="Hello")
    # Solo retorna lo nuevo; MessagesState concatena con el historial.
    return {"messages": [respuesta]}
```


¿Cómo reaccionar a entradas y agregar respuestas de la IA?

- Lógica ejemplo: si no hay *customer name*, actualiza esa parte del estado. Si existe, agrega un **AI message** al historial.
- En la interfaz de *debug* puedes inyectar mensajes iniciales: *human message*, *AI message*, *tool*, *function*, *chat*, etc.
- El *messages stage* garantiza que **siempre recibes un array**, así puedes hacer `get("messages")` con confianza.

```python
def simple_node(state):
    customer = state.get("customer_name")

    if not customer:
        # Actualiza solo el nombre del cliente y no toca el historial.
        return {"customer_name": "Nicolás Molina"}
    # Si ya hay customer name, agrega una respuesta de la IA al historial.
    return {"messages": [AIMessage(content="Hola, ¿en qué más te ayudo?")]}
```

- Prueba en *debug*: si envías un *human message* inicial (por ejemplo, "Hola, soy Nicolás"), verás que entra al estado y luego la IA **concatena** su respuesta sin borrar lo anterior.

¿Qué estrategias de contexto y tokens puedes aplicar?

Administrar el historial impacta costos y calidad. Puedes combinar técnicas según el caso.

- Usar un *summary* del historial con un *large language model* para comprimir y ahorrar tokens.
- Enviar todo el historial cuando necesites máximo contexto.
- Tomar el primer o el último mensaje si buscas señales específicas.
- Decidir por nodo o por agente qué porción del historial usar.

### **Integración de modelos OpenAI y Anthropic con LangChain**

Integrar varios modelos en un sistema multiagentes es más simple y potente con una arquitectura agnóstica. Con **LangGraph** como orquestador y **LangChain** como intermediario, puedes cambiar entre OpenAI y Anthropic sin reescribir tu flujo. Aquí verás cómo configurar claves, enviar *history* de chat con *system/human/AI message* y usar la función **init chat model** para mantener una API homogénea.

¿Cómo integrar language models en un sistema multiagentes?

En un entorno de múltiples agentes, cada agente puede usar el **modelo más apropiado** para su tarea. **LangGraph** define la lógica y la coordinación con grafos y un **state graph** que almacena mensajes, mientras que los *language models* son los “cerebros” que razonan y actúan. La ventaja clave: **arquitectura agnóstica o híbrida**.

- **LangGraph**: orquestador de nodos y estado compartido entre agentes.
- **LangChain**: utilidades para conectar modelos de forma agnóstica y uniforme.
- Puedes usar *SDKs* directos de OpenAI, Gemini, Hugging Face o Llama Index en cada nodo.
- **Misma API de invocación**: invocas con *invoke* y cambias el modelo con mínimas modificaciones.

¿Qué pasos necesitas para configurar claves y probar un modelo?

Para trabajar con modelos, primero carga variables de entorno. Evita imprimir tus keys: un *notebook* guarda el historial de ejecuciones y puede exponerlas.

¿Cómo cargar variables de entorno .env sin exponer keys?

```python
import os
from dotenv import load_dotenv
load_dotenv()
# Verifica que la variable exista sin imprimirla
assert os.getenv("OPENAI_API_KEY") is not None
```

- Usa `.env` y `load_dotenv()` para cargar tus claves.
- Evita `print(API_KEY)`. Si lo hiciste, borra la celda para no dejar rastros.

¿Cómo probar ChatOpenAI e interpretar la respuesta?

```python
from langchain_openai import ChatOpenAI
llm = ChatOpenAI(model="gpt-3.5-turbo", temperature=0.7)
response = llm.invoke("Hola, hola, ¿cómo estás?")
print(type(response))  # AIMessage
print(response.text)  # Contenido de la respuesta
```

- Respuesta típica: saludo y oferta de ayuda.
- Ejemplo de latencia: ~1.2 s con un modelo rápido, ~1.3 s en otra llamada.
- Cambiar de modelo es cambiar una línea: `model="gpt-3.5-turbo"` a otro de la misma familia.

¿Cómo manejar historial y cambiar de proveedor sin reescribir código?

El *history* permite que el modelo “recuerde” el contexto. Con **SystemMessage**, **HumanMessage** y **AIMessage** defines instrucciones, entradas y salidas previas. El **state graph** de LangGraph recolecta ese historial para cualquier agente o nodo.

¿Cómo enviar el historial de chat con system, human y AI message?

```python
from langchain_core.messages import SystemMessage, HumanMessage, AIMessage
history = [
    SystemMessage(content="Eres un asistente útil."),
    HumanMessage(content="Me llamo Juan."),
    AIMessage(content="Hola Juan, ¿cómo estás?"),
    HumanMessage(content="¿Cómo me llamo?")
]
response = llm.invoke(history)
print(response.text)  # "Te llamas Juan"
```

- El modelo responde “Te llamas Juan” porque el nombre está en el *history*.
- Con **LangGraph** puedes tener ese *history* disponible en cualquier nodo.

¿Cómo cambiar a Anthropic e instalar la dependencia?

Para usar la familia de Anthropic, agrega su key a tu `.env` e instala el conector.

```bash
pip install -U langchain-anthropic --pre
```

```python
from langchain_anthropic import ChatAnthropic
llm = ChatAnthropic(model="TU_MODELO_ANTHROPIC", temperature=0.7)
response = llm.invoke(history)
print(response.text)  # "Tu nombre es Juan..."
```

- Ejemplo de latencia: ~1.7 s con un modelo de Anthropic.
- El código casi no cambia: solo la declaración del modelo y la dependencia.

¿Para qué usar init chat model en una arquitectura agnóstica?

Cuando los modelos comparten hiperparámetros comunes (como **temperatura** y **nombre del modelo**), **init chat model** compacta la configuración y conserva la misma API de *invoke*.

```python
# Referencia: src/agents/simple.py línea 3
from langchain.chat_models import init_chat_model
llm = init_chat_model(
    model="gpt-4",  # o el que prefieras
    model_provider="openai",  # por ejemplo: "anthropic", "google", "mistral"
    temperature=0.3
)
response = llm.invoke(history)
print(response.text)
```

- Ventaja: **cambiar de proveedor sin reescribir** imports ni lógica.
- Requisito: **instalar la dependencia** del proveedor que uses.
- Internamente, la función hace un gran `if` por *model provider* y verifica el paquete instalado.
- Hiperparámetros: todos comparten **temperatura** y **modelo**. Algunos, como Gemini, permiten además **top-k** y **top-p**.

Habilidades y conceptos prácticos que se aplican:

- **Arquitectura agnóstica** con *frameworks*: cambia de OpenAI a Anthropic manteniendo el mismo flujo.
- **Gestión de variables de entorno**: `.env`, `load_dotenv()` y cuidado con las keys.
- **Estructuración de prompts** con *system/human/AI message* para dar contexto e instrucciones.
- **Historial de chat** y **state graph** para memoria conversacional entre nodos.
- **Hiperparámetros** como temperatura, y según el proveedor, **top-k** y **top-p**.
- **API homogénea** con *invoke* e **init chat model** para rapidez y mantenibilidad.

### **Integración de LLM en grafos para agentes que razonan**

Convierte un flujo de datos en un agente que razona: integra un *large language model* en un grafo con LangGraph y orquesta decisiones de forma autónoma. Este enfoque combina **memoria compartida**, **hilos** y **estado persistente** para que los nodos no solo procesen datos, sino que **piensen y actúen** según el contexto acumulado.

¿Cómo convertir un flujo de datos en un agente que razona con LangGraph y LangChain?

El punto de partida es un flujo de datos sin “cerebro”: start → node1 → end. La clave es **inyectar un *large language model*** en el grafo para que el **agente** decida, ramifique, haga ciclos y retroceda cuando sea necesario. Puedes conectar modelos con **LangChain**, *SDK* nativo o *Llama Index*; lo importante es que **LangGraph** ejecute su motor de grafos y mantenga el **estado**.

- **De proceso a inteligencia**: pasar de transformar datos a razonar y tomar acciones.
- **Nodos con estado**: cada nodo puede leer y escribir en el **estado compartido**.
- **Memoria viva por hilo**: el contexto se conserva mientras mantengas el mismo **ID de hilo**.

¿Qué pasos de código integran el LLM y actualizan el estado compartido?

Se define el modelo, se ajusta la **temperatura** y se reescribe la lógica del nodo para trabajar con un **new_state** que consolida cambios y mensajes antes de devolver el **return**.

¿Cómo configurar el modelo y su temperatura?

Se inicializa el modelo con **temperatura = 1** y se prepara para la **invocación**.

```python
# Referencia: src/agents/simple.py línea 6
llm = init_chat_model("openai:gpt-4o-mini", temperature=1)
```

- **Temperatura 1**: respuestas más creativas y variadas.
- **Invocación**: se llamará al modelo con el historial y el mensaje actual.

¿Cómo cambia la lógica del nodo con new state?

Se crea un **new_state** (diccionario) y se aplica una lógica simple basada en si existe un nombre del usuario.

```python
import random

def node1(state):
    new_state = {}
    # Si no hay nombre, asígnalo; si ya hay, actualiza edad aleatoria.
    if not state.get("customer_name"):
        new_state["customer_name"] = "John Du"  # valor capturado/derivado.
    else:
        new_state["my_age"] = random.randint(18, 80)
    # ...luego se añadirá la parte de mensajes.
    return new_state
```

- **customer_name**: primero se captura y guarda.
- **my_age**: se asigna solo si ya existe un nombre, usando un número aleatorio.

¿Cómo se unen mensajes y se persisten en la memoria?

Se toma el **historial de mensajes** del estado, se agrega la nueva respuesta de la **AI** y se guarda en el **new_state**. Al devolverlo, LangGraph actualizará la **memoria compartida**.

```python
def node1(state):
    new_state = {}
    # Lógica de nombre/edad como antes...
    # ...
    # Historial existente y nueva respuesta de AI.
    history = state.get("messages", [])
    ai_reply = {"role": "ai", "content": "Hola, estoy aquí para ayudarte."}
    # Unir *arrays*: historial + [nueva respuesta].
    new_state["messages"] = history + [ai_reply]
    return new_state
```

- Unión de *arrays*: se usa history + [mensaje_ai].
- Persistencia: el historial crece con cada intercambio.

¿Cómo funcionan los hilos, la memoria compartida y la interfaz de LangGraph Studio?

Al **crear un nuevo hilo**, la memoria arranca en limpio; al **mantener el mismo hilo**, el estado persiste, incluso si recargas la *UI*. En LangGraph Studio es visible el **view state** y puedes **debuggear** el grafo, revisar el **JSON** del estado y chatear desde una **interfaz de chat** cuando el agente es de tipo “mensajes”.

¿Qué es un hilo y cómo persiste el estado?

- Un hilo conserva: **estado**, **historial de mensajes** y valores como customer_name.
- Mientras uses el mismo **ID de hilo**, la **memoria compartida** se mantiene.
- Ejemplo: tras “Hola, ¿cómo estás?” el agente responde “Hola, estoy aquí para ayudarte” y guarda el **customer_name = John Du**; luego, al decir “me llamo Nicolás”, el sistema recuerda y puede asignar **my_age**.

¿Qué viste en el historial de mensajes y *arrays* vacíos?

- Puede aparecer un mensaje “vacío” en el historial: a veces LangGraph/LangChain envían “reacciones” como “estoy pensando” o “escribiendo”.
- Puedes inspeccionar el estado en vista **colapsada** o de **detalle**, e incluso como **JSON** para entender cada paso.

¿Cómo aprovechar el prompt y la memoria compartida?

- Mejora el **system prompt**: inyecta el nombre capturado (por ejemplo, “Nicolás”) para que el modelo **recuerde** y responda con contexto.
- Aplica **prompting** basado en el **estado**: cualquier agente puede leer el estado compartido y continuar el trabajo desde allí.
- Más adelante, podrás montar persistencia propia y exponer una API con *FastAPI*.
- Reto 1: crea dos hilos en LangGraph Studio y verifica que el **historial** y la **memoria compartida** se mantengan por hilo.
- Reto 2: configura un **system prompt** que use datos del estado (por ejemplo, el nombre) para personalizar respuestas.

### RAG con OpenAI file search para consultar pdfs

Implementa un RAG sencillo y funcional con OpenAI para responder preguntas desde tus PDFs. Enfócate en resultados: agrega conocimiento actualizado o privado a tu large language model y mejora la precisión sin montar infraestructura compleja de *embeddings* y bases vectoriales.

¿Qué problema resuelve un RAG con OpenAI file search?

Un large language model se entrena con mucha información pública, pero tiene límites claros. **No sabe datos en tiempo real** y **no incluye tu información privada**. Por eso, si preguntas por el clima de hoy, fallará; y si necesitas que responda sobre tus manuales, productos o bases de datos, tampoco podrá sin que se los cargues.

¿Por qué el large language model no tiene info en tiempo real?

- Su “ventana de información” llega hasta la fecha de entrenamiento.
- Es malo respondiendo consultas de tipo real time.
- Para actualizar conocimiento, se usan *tools* como *web search* o un RAG.

¿Qué información privada puedes agregar?

- PDFs: manuales, guías, documentación interna.
- Datos de productos y procedimientos.
- Todo lo que puedas pasar a texto.

En este enfoque se usa la *tool* de OpenAI llamada **file search**: **subes PDFs, se vectorizan y luego consultas**. Es una técnica de RAG sencilla pero potente para prototipos y primeros casos de uso (por ejemplo, customer support).

¿Cómo crear y cargar una base vectorial en OpenAI?

Desde la plataforma de OpenAI, con tu key y proyecto (mejor si creas uno dedicado), ve a Storage > Vector stores. **Crea una base vectorial** (ej.: “My docs”) y **sube tus archivos**. El sistema convierte el texto a *embeddings*, los guarda y te entrega un **ID** para consultarlo desde tu código.

¿Qué bases vectoriales existen y por qué usar la de OpenAI?

- Alternativas: Chroma, Pintcup, Vectorize, PostgreSQL con vectoriales, Mongo con *embeddings*.
- Ventaja aquí: OpenAI ya te da un vector store listo. Cómodo para empezar.
- Nota: no es tan personalizable/automatizable como un RAG avanzado.

¿Qué hace el pipeline de embeddings y búsqueda?

- Vectoriza el PDF en una base de datos vectorial.
- Permite consultas semánticas (queries) sobre ese contenido.
- El modelo usa ese conocimiento para generar respuestas con mayor ajuste al documento cargado.

Habilidades y keywords trabajadas:

- Configurar proyecto y gestionar *vector stores*.
- Subir archivos y “attach” a la base vectorial.
- Copiar y usar el **ID** del vector store.
- Entender *embeddings* e inferencia basada en vectores.

¿Cómo invocar el modelo con la tool de file search?

Debes usar el modelo de OpenAI porque **file search es específica de este proveedor**. Se declara un arreglo con tus IDs de *vector stores*, y se pasa la lista de *tools* al LLM. Al preguntar, el modelo decide si necesita consultar su base vectorial.

- Si la pregunta lo amerita (ej.: “¿Cómo mejorar el rendimiento de un website?”), **hará un query** a la base vectorial y responderá desde el PDF.
- Si es trivial (ej.: “Hola, ¿cómo estás?”), **no llama la tool** y responde directo. Este “switch” lo maneja el propio modelo.
- Puedes comparar tiempos: sin *tools* responde más rápido, pero sin el conocimiento del PDF.

¿Cómo limitar el contexto y manejar el historial?

La *tool* puede fallar si le envías “todo el array de mensajes” (mucho contexto). Solución práctica: **enviar solo el último mensaje** del historial al LLM. Pierdes memoria conversacional (no recordará tu nombre), pero evitas errores. Alternativas: resumir mensajes o, si necesitas historial completo, pasar a un **RAG más avanzado**.

Pseudocódigo ilustrativo:

```python
# IDs de tus vector stores (copiados de OpenAI)
vector_store_ids = ["vs_XXXXXXXX"]
# Declarar tool de file search con tus IDs
tools = [{"type": "file_search", "vector_store_ids": vector_store_ids}]
# Instanciar LLM de OpenAI con tools
llm = LLM(provider="openai", tools=tools)
# Enviar solo el último mensaje del historial
last_message = history[-1].text
response = llm.invoke(user_input=last_message)
print(response)
```

¿Cómo integrarlo en tu app?

- Crea un archivo “rag.py” a partir de tu “simple”.
- Integra la *tool* de **file search** y verifica el **ID** del vector store.
- Sobrescribe el LLM para que use *tools*.
- Envía solo el último mensaje del historial.
- Registra el nuevo agente en “lang-af.json” (ej.: “RAG”).
- Reinicia el servidor con “lang-af.dev” y prueba en la interfaz de chat.

Conceptos y keywords clave incorporados:

- **Large language model**, ventana de información y real time.
- *Tools* de OpenAI: *function coding*, *web search*, *file search*, *Computer Views*.
- **Base de datos vectorial**, *vector stores*, *embeddings*, inferencia.
- Trade-offs entre contexto completo vs. último mensaje.
- Agentes, estado e historial del chat.

## Lógica y Estructura de Nodos

### **Prompt chaining: encadenar agentes en secuencia con LangGraph**

Orquestar varios agentes permite resolver tareas complejas con claridad y control. Aquí verás cómo encadenar nodos con LangGraph, cuándo elegir el enfoque secuencial o en paralelo, y en qué casos conviene delegar el plan a un modelo razonador con *chain of thought* para ahorrar costo y mejorar calidad.

¿Qué es el prompt chaining y cómo orquesta agentes?

El *prompt chaining* conecta varios nodos en una secuencia. Cada nodo usa un *large language model* para una tarea específica y luego pasa el estado al siguiente. En este patrón, el modelo no decide: solo sigue un orden fijo, aunque cada nodo razona localmente.

- **Secuencial:** del nodo uno al dos y al tres, en orden fijo.
- **Paralelo:** ejecuta varios nodos al mismo tiempo, sin decisiones del modelo.
- **Workflows con decisiones:** el modelo puede elegir qué hacer y cuándo.
    - Patrón orquestador con *planning*: planifica y ejecuta solo los nodos necesarios.
    - *Evaluator*: ciclo de revisión hasta que la respuesta sea aceptable.
    - *Routing*: decide por qué nodo continuar.
- Patrón *agent*: integra *tools* y un proceso de reflexión.

En todos los casos, los nodos encapsulan comportamientos distintos y facilitan dividir el problema en pasos comprensibles. La clave: **definir bien qué hace cada nodo** y cómo fluye el estado entre ellos.

¿Cuándo usar chaining y cuándo un modelo razonador con chain of thought?

Un encadenado de pasos puede ser reemplazado por un buen prompt con *chain of thought* en un modelo razonador. La advertencia es clara: si las instrucciones caben bien en un solo prompt, un modelo que razona puede seguir el plan sin necesidad de múltiples nodos.

- **Modelos razonadores mencionados:** Open AI ZeroOne Preview, Gemini 2.5 con Thinking y la familia de Anthropic con razonamiento.
- **Costo:** cada nodo implica una llamada al modelo. Un solo prompt con razonamiento puede ser más económico.
- **Cuándo dividir en nodos:** cuando hay pasos con alta carga cognitiva, prompts muy largos o integración con servicios externos.
- **Cuándo preferir un solo prompt:** en tareas simples donde el modelo puede seguir el plan completo en una pasada.

Ejemplo educativo que ilustra la advertencia: generar una broma, luego mejorarla y añadir un twist. Con modelos actuales, se puede dar toda la secuencia en un prompt y lograr el mismo resultado sin encadenar nodos.

¿Cómo implementar chaining en LangGraph de forma práctica?

El flujo básico: crear nodos, agregarlos al grafo y conectar los edges en secuencia. Así se construye un pipeline del nodo 1 al 2 y al 3, se compila y se visualiza el gráfico.

¿Cómo crear nodos y conexiones en secuencia?

- Definir funciones por nodo y agregarlas al grafo.
- Conectar: del nodo uno al dos, del dos al tres y el tres finaliza.
- Compilar y generar el gráfico para validar la secuencia.
- Alternativa compacta: usar un *builder* con *add sequence* pasando un arreglo de funciones [nodo uno, nodo dos, nodo tres]. El nombre de la función se usa como nombre del nodo.

Advertencia de buenas prácticas: el ejemplo de “generar broma → mejorar broma → añadir twist” funciona, pero puede ser innecesario si un solo prompt en un modelo razonador ya sigue el plan.

¿Cómo llevarlo a un flujo real con extractor y conversation?

- Crear un nodo extractor que prepara o extrae datos del estado.
- Encadenar: iniciar en extractor → pasar a conversation → finalizar.
- El nodo conversation mantiene la interacción y decide si debe analizar un archivo o consultar una base de datos vectorial antes de responder.
- Visualizar en LangGraph Studio para confirmar el patrón de chain.

Incluso si el extractor inicialmente no hace nada, **dejarlo en el flujo hace explícita la arquitectura** y permite evolucionar el pipeline con bifurcaciones futuras.

¿Qué caso práctico ilustra mejor el valor del chain?

- Social media: de un texto largo o PDF, un nodo genera un tuit.
- Luego, otro nodo llama a un modelo de imágenes (por ejemplo, DALL·E de OpenAI) para crear una imagen del tuit.
- Aquí un *chain of thought* no basta, porque **no genera imágenes**. El chain integra modelos diferentes paso a paso.

Si ya estás usando secuencias en tu “rack”, piensa qué pasos conviene dejar en nodos y cuáles condensar en un prompt con razonamiento, equilibrando claridad, costo y rendimiento.

### **Respuestas estructuradas en LLMs para agentes**

Controlar cómo responde un **large language model** es clave para construir agentes que tomen decisiones con seguridad. Pasar de texto libre a **respuestas estructuradas** permite evaluar, guardar y accionar sobre datos concretos como nombre, email, teléfono, tono y sentimiento, reduciendo impredecibilidad y costos.

¿Por qué estructurar respuestas de un large language model?

Estructurar la salida transforma un mensaje impredecible en un **objeto controlado**. En lugar de depender del tono, longitud o adherencia variable al prompt y a la temperatura, se fuerza al modelo a devolver un **JSON** con un **schema** claro para operar en código y en el **lang graph** del agente.

- **Evaluación programática**: extraer nombre, email, teléfono, tono o sentimiento para usarlos como variables.
- **Decisiones de agente**: con datos consistentes, un nodo puede ramificar o reevaluar.
- **Más que chat**: el modelo ya no conversa, actúa como **extractor**.

¿Qué aporta el structured output frente a JSON mode?

La salida estructurada resuelve la necesidad de “responder en JSON” sin depender del antiguo **JSON mode**.

- **Integraciones** en LangChain con múltiples modelos y soporte de salida estructurada.
- Ejemplo citado: “Entropic” con tool chain, tool coding, salida estructurada y multimodal.
- **JSON mode** ya no es central cuando se usa **structured output**.

¿Cómo implementar un extractor con structured output?

El flujo parte de un **schema** y un **system prompt**. Se define una clase Pydantic, se activa el structured output del modelo y se envía el historial para que el LLM devuelva un objeto validado.

- Definir clase contact info con campos como **name**, **email**, **phone**, **tone** e **age**.
- Usar Pydantic en Python para que el **schema** se traduzca a lo que la **API** necesita.
- Indicar en la descripción cómo evaluar variables, por ejemplo **tone** en un rango 0–100 o sentimiento categórico.
- Enviar un **system prompt**: el modelo debe “extraer información de la conversación” siguiendo el schema.
- Enviar mensajes como tuplas tipo system y usuario, con todo el historial cuando se requiera.
- La respuesta llega como objeto Pydantic, listo para hacer acceso directo a campos.

¿Qué errores comunes y cómo mitigarlos?

Al estructurar, emergen fallos típicos que se corrigen con prompt y validación.

- **Alucinación de datos**: puede inventar “age”. Pedir explícitamente “si no encuentras, no inventes”.
- **Validaciones estrictas**: si un campo es entero y no hay dato, se rompe. Ponerlo como string o usar fallback temporal.
- **Sentimiento/tono ambiguo**: aclarar escalas o enums en descripciones.
- **Mensajes genéricos del modelo**: recordar que aquí no se busca chat, sino extracción.

¿Cómo integrar el extractor en un agente con memoria compartida?

Se agrega un **nodo extractor** con structured output y se mantiene el nodo conversacional estándar. El extractor lee el historial, extrae datos clave y los guarda en la memoria para que el siguiente nodo los use en su prompt.

- Instanciar un LLM con **structured output** (se mostró con “Claude”) solo en el nodo extractor.
- Mantener el LLM conversacional normal en el nodo de conversación.
- Lógica de disparo: si customer name es none o si el historial supera **>10 mensajes**, volver a extraer.
- Guardar en estado compartido: **customer name**, **email**, **phone**, **age**.
- Inyectar memoria en el **system prompt** del nodo conversacional de forma dinámica, con fallback si falta información.
- Optimizar costos: evitar llamadas si ya se obtuvo el dato y el historial no cambió.
- Si no hay “información relevante”, instruir al nodo de conversación a seguir el flujo normal, no a consultar la base vectorial.

¿Qué habilidades y keywords se practican?

El ejercicio refuerza técnicas de prompting y diseño de agentes con salida sólida y reusable.

- **Prompting**: buen **system prompt** y reglas de no invención.
- **Técnicas**: *zero shot*, *few shot*, *chain of thought* cuando aplique.
- **Schema design**: Pydantic, tipos, rangos y descripciones claras.
- **Memoria compartida**: actualización de estado y uso en prompts.
- **Control de flujo**: condiciones por tamaño de historial y reextracción.
- **Integraciones**: LangChain, *chat models*, salida estructurada, opciones locales como *Ollama* o *Hugging Face*.
- **Ecosistema**: *JSON Schema*, *API*, *Python*, “Claude”, “OpenAI”, “Cloudflare”.

### **Organización de código en LangGraph para sistemas complejos de AI**

Escalar un sistema con múltiples nodos, prompts, RAGs y tools exige una organización clara. Aquí verás cómo refactorizar hacia una **arquitectura modular en LangGraph** para mejorar mantenimiento, visibilidad de la orquestación y crecimiento controlado, separando agente, estado, nodos, prompts y tools en carpetas consistentes.

¿Por qué reorganizar el código para escalar en LangGraph?

Una sola base de código en un archivo se vuelve frágil cuando crecen los nodos y las dependencias. La propuesta: **convertir cada agente en una carpeta** con subcarpetas por nodo y archivos específicos para estado, grafo, prompts y tools. Así:

- **Mantenibilidad**: localizar y mejorar un nodo es inmediato.
- **Escalabilidad**: añadir nodos no rompe la base existente.
- **Claridad**: cada responsabilidad vive en su lugar: estado, grafo, nodo, prompt, tools.
- **Visibilidad**: entender qué pasa con los nodos y la orquestación es más simple.

Conceptos clave integrados: agente y grafo del flujo, nodos con su propio *large language model* (LLM), *system prompt*, *tools* y manejo del estado del mensaje. Usa LangGraph Studio para depurar y validar el flujo.

¿Cómo estructurar agentes, nodos y prompts para RAG?

La idea central: el agente “Support” deja de ser un archivo y pasa a ser una carpeta. Dentro, se separan el estado, el grafo y los nodos. Cada nodo tiene su propio prompt y, si aplica, sus *tools*.

¿Qué carpetas y archivos crear?

Estructura sugerida para “Support”:

```text
agents/
  support/
    __init__.py
    state.py            # estado del mensaje.
    agent.py            # construcción del grafo del agente.
    nodes/
      extractor/
        __init__.py
        node.py         # lógica del nodo extractor.
        prompt.py       # system prompt del extractor.
      conversation/
        __init__.py
        node.py         # lógica del nodo conversation.
        prompt.py       # system prompt del conversation.
        tools.py        # tools ligadas a este nodo.
```

Puntos clave:

- Cada nodo es una carpeta con su node.py, prompt.py y, si aplica, tools.py.
- Los imports se corrigen para apuntar a paths claros: por ejemplo, al estado desde "agents.support.state".
- Se evita crear carpetas innecesarias como “rutas” si aún no se usan.

¿Cómo separar prompts y tools por nodo?

- Prompt por nodo: se define un archivo prompt.py por nodo con su **system prompt** declarado de forma explícita.
- Tools por nodo: en conversation/tools.py se listan las *tools* y se exportan en un array para inyectarlas al LLM del nodo.

Ejemplo mínimo de prompt y combinación con historial del estado:

```python
# src/agents/support/nodes/extractor/prompt.py
from langchain_core.prompts import PromptTemplate

template = """\
You are a helpful assistant that can extract contact information from a given conversation.
"""
prompt_template = PromptTemplate.from_template(template)

# src/agents/support/nodes/extractor/node.py
from agents.support.state import State
from agents.support.nodes.extractor.prompt import prompt_template

def extractor(state: State):
    history = state["messages"]
    customer_name = state.get("customer_name", None)
    new_state: State = {}
    if customer_name is None:
        prompt = prompt_template.format()
        schema = llm.invoke([("system", prompt)] + history)
        new_state["customer_name"] = schema.name
    return new_state
```

Notas prácticas:

- Se usa un *system prompt* claro para guiar el nodo extractor.
- La concatenación del *system prompt* con el history puede requerir ajustarlo a tu API de mensajes: array de uno o tupla, según el formato que uses.

¿Cómo se construye el agente con el grafo?

- agent.py importa el estado y cada nodo ya modularizado.
- Cada nodo declara su propio LLM: por ejemplo, conversation con *OpenAI* para habilitar *tools*.
- Se inyectan prompts y *tools* en el nodo correspondiente, manteniendo la configuración aislada.

Ejemplo mínimo del nodo conversation con *tools*:

```python
# conversation/tools.py
# Define y exporta las tools de este nodo.
tools = [# ...instancias de tools específicas del nodo...]

# conversation/node.py
from .tools import tools
from .prompt import SYSTEM_PROMPT

def configure_conversation_node(llm):
    llm_with_tools = llm.bind_tools(tools)
    # se inyecta el system prompt simple; la dinamización llegará después.
    return {"llm": llm_with_tools, "system_prompt": SYSTEM_PROMPT}
```

¿Qué prácticas aplicar para mantener y crecer el proyecto?

- **Un agente, una carpeta**: facilita navegación y escalabilidad.
- **Estado centralizado**: un state.py con el message state único.
- **Nodo autocontenido**: cada nodo con su node.py, prompt.py y tools.py si aplica.
- **LLM por nodo**: declarar en el nodo el *large language model* que usará.
- **Prompts declarativos**: mantener el *system prompt* por archivo y por nodo.
- **Tools agrupadas**: exportar un array de *tools* por nodo y enlazarlas al LLM.
- **Imports limpios**: rutas explícitas evitan confusiones y errores.
- **Refactor incremental**: trasladar estado, luego nodos, luego prompts y *tools*.
- **Prueba continua**: validar en LangGraph UI y en el debugger que todo sigue funcionando.
- **Preparación para prompts dinámicos**: dejar el *system prompt* simple ahora y planear la inyección de variables después.

### **Prompts dinámicos con LangChain y templates condicionales**

Una buena ingeniería de prompting marca la diferencia. Aunque uses los modelos más potentes y un orquestador de grafos como *LangGraph*, un **prompt mediocre produce resultados mediocres**. Aquí aprenderás a gestionar prompts de forma eficaz, hacerlos dinámicos y limpios con *LangChain*, *PromptTemplate* y un motor de plantillas tipo *Jinja2*, sin depender de técnicas específicas.

¿Por qué el prompting es vital en agentes con LangGraph?

Un *prompt* guía al *language model* hacia el objetivo. No es opcional: es crítico. Técnicas como **zero shot**, **few shot** y **chain of thought** pueden mejorar los resultados según el modelo y la tarea, pero el foco está en **cómo gestionarlos a nivel de ingeniería** para agentes orquestados con *LangGraph*.

- Los ejemplos con una sola línea son prácticos para enseñar orquestación, pero no son buenos prompts.
- Un buen prompt define roles, formato y atributos con claridad.
- **Cada carácter cuenta**: espacios extra y saltos de línea innecesarios añaden tokens y ruido.
- Habilidades clave: ingeniería de *prompt*, orquestación de agentes, manejo de estado, dinamización de variables, control de formato.

¿Cómo impactan las técnicas en los resultados?

- Zero shot: útil cuando no hay ejemplos, pero puede ser inconsistente.
- Few shot: añade ejemplos y guía estilo y formato.
- Chain of thought: favorece la explicación paso a paso; suele funcionar mejor en *XML* que en Markdown.

¿Qué papel cumple el estado en prompts dinámicos?

- Con un gestor de estado como *LangGraph*, puedes derivar tono, contexto o parámetros y **inyectarlos dinámicamente**.
- Si algo es fijo, va en el template; si cambia, se modela como variable.

¿Cómo crear prompts efectivos con PromptTemplate de LangChain?

Usa *PromptTemplate* para declarar variables sin obligarte a resolverlas al definir el string. Evita concatenaciones con f-strings temprano; **inyecta datos al formatear**.

```python
# Ejemplo base de template con primera línea "escapada" para evitar salto inicial
from langchain_core.prompts import PromptTemplate  # Referencia: src/agents/support/nodes/extractor/prompt.py

template = """\
Instrucciones en Markdown:
- Sigue el rol indicado.
- Respeta el formato solicitado.
Fecha actual: {fecha_actual}
Texto del anuncio: {texto_anuncio}
"""

prompt_tmpl = PromptTemplate(template=template)

# Al formatear, envías las variables dinámicas
prompt_final = prompt_tmpl.format(
    fecha_actual="2024-05-01",
    texto_anuncio="Lanza tu producto con 20% de descuento.")
print(prompt_final)
```

- El backslash inicial evita que el primer salto de línea se convierta en tokens.
- Si faltan variables, el template lanza un error: te obliga a completar lo necesario.

¿Cómo evitar errores al inyectar variables?

- Define variables en el template y envíalas en .format cuando estén disponibles.
- Si aún no existen en memoria, no bloquees la definición del template.

¿Cómo usar partial variables por defecto?

Puedes declarar valores por defecto con partial variables para que el template funcione aunque no envíes todo.

```python
from datetime import date

prompt_tmpl = PromptTemplate(
    template=template,
    partial_variables={"fecha_actual": lambda: date.today().isoformat()}
)
# Solo envías lo que cambia en tiempo de ejecución
prompt_final = prompt_tmpl.format(
    texto_anuncio="Actualiza tu sitio con nuevas funcionalidades.")
print(prompt_final)
```

- Útil para campos como "fecha actual" que pueden autocompletarse.
- Mantiene el prompt coherente y reduce errores en orquestación.

¿Cómo condicionar secciones con Jinja2 para prompts limpios?

Cuando necesitas variaciones pequeñas (por ejemplo, saludar por nombre si está disponible), un motor de plantillas tipo *Jinja2* permite **bloques condicionales** en el propio template. Así evitas mantener dos prompts casi iguales.

```python
# Template con condicional y limpieza de espacios
from langchain_core.prompts import PromptTemplate

rag_template = """\
Eres un asistente superútil que responde al mensaje del usuario.
{% if name -%}
El cliente se llama {{ name }}.
{%- endif %}
Mensaje del usuario: {{ user_message }}
"""

prompt_tmpl = PromptTemplate(
    template=rag_template,
    input_variables=["user_message", "name"],
    template_format="jinja2"  # Motor condicional mencionado
)

# Si no hay name, puedes usar partial para neutralizarlo
prompt_tmpl = PromptTemplate(
    template=rag_template,
    input_variables=["user_message"],
    partial_variables={"name": None},
    template_format="jinja2"
)

print(prompt_tmpl.format(user_message="¿Cómo puedo optimizar mi sitio web?"))
```

**Ejemplo real del proyecto** — patrón Jinja2 con condicional en uso:

```python
# src/agents/support/nodes/conversation/prompt.py
from langchain_core.prompts import PromptTemplate

template = """\
Your are a helpful that responds to the user's 

{{% if name %}}
The user's name is {{ name }} and you can call them by that name
{{% endif -%}}
"""
prompt_template = PromptTemplate.from_template(template, template_format="jinja2")
```

```python
# src/agents/support/nodes/booking/prompt.py — partial_variables con fecha dinámica
from langchain_core.prompts import PromptTemplate
from datetime import date

today = date.today().strftime("%Y-%m-%d")
prompt_template = PromptTemplate.from_template(template, partial_variables={"today": today})
```

- El bloque {% if name -%} … {%- endif %} condicionalmente incluye la sección.
- Los guiones “-” en los tags recortan saltos de línea y evitan huecos.
- Ideal para asistentes de *RAG* donde el campo "customer name" podría faltar.

¿Cómo activar el motor de templates condicional?

- Instala la dependencia del motor *Jinja2* y reinicia tu entorno si es necesario.
- Declara template_format="jinja2" al crear el *PromptTemplate*.

¿Cómo limpiar saltos de línea innecesarios?

- Usa guiones en los tags del condicional para **recortar espacios y saltos**.
- Mantén un solo salto cuando separes indicaciones distintas.

## Agentes ReAct

### **Patrón ReAct para agentes que razonan y ejecutan tools**

La arquitectura React para agentes con *tools* permite **razonar, actuar y observar** en ciclos controlados hasta cumplir un objetivo. Con este enfoque, el agente decide si llamar una o varias *tools*, cuándo pedir más datos y en qué momento finalizar, logrando respuestas más precisas y útiles.

¿Qué es el patrón react y por qué potencia agentes con tools?

El patrón React (reason and act) **integra razonamiento y ejecución** en un solo bucle. El agente analiza, actúa con *tools*, observa resultados y decide si continuar o cerrar con una respuesta final. Así se evita separar el “pensar” de la “acción”, y se crea un **ciclo virtuoso** que mejora decisiones.

- Une razonamiento y acciones en un bucle iterativo.
- Controla bucles con un **máximo de iteraciones** para evitar ciclos infinitos.
- No depende del proveedor: puedes definir tus propias *tools*.
- Permite **structured output** usando *tools* para dar salidas formateadas.
- Contrasta con un *chain* secuencial: aquí hay **bifurcaciones** y *routers* en un grafo.

En el ecosistema: **LangChain** ofrece utilidades y un agente que implementa React por defecto con create_agent. **LangGraph** orquesta el flujo en grafo, es agnóstico a librerías y facilita **nodos**, **edges** y **ruteo**. Juntos, simplifican un patrón complejo en “cuatro o cinco líneas”, sin perder flexibilidad para versiones “custom”.

¿Cómo decide un agente cuándo llamar una tool y cuándo responder?

El agente parte de un *prompt* e historial, evalúa si basta con razonar o si debe ejecutar una *tool*. Si no necesita *tool*, responde. Si la requiere, **planifica**, invoca una o varias *tools*, **observa** resultados y decide si repetir o finalizar con la respuesta.

- Decide si usar 1 o varias *tools* antes de responder.
- Pide información faltante al usuario cuando es necesaria.
- Se detiene al cumplir el objetivo o al alcanzar el tope de iteraciones.
- Puede informar “no hay información suficiente” si faltan datos clave.

Ejemplo explicado: un **agendador de citas** pide fecha, nombre del doctor y nombre del paciente para ejecutar *tools* como “crear cita” o “verificar disponibilidad”. El agente **gestiona el diálogo**, recolecta datos mínimos y solo entonces ejecuta las *tools* para resolver la tarea por completo.

Punto clave: aunque proveedores como OpenAI internamente decidan llamar una *tool* (ej.: *file search*), aquí tú **controlas** el patrón. Puedes combinar utilidades de **LangChain** (agente React con create_agent) con la **orquestación** de **LangGraph** para construir flujos con bifurcaciones y ciclos.

¿Qué modelos razonadores convienen para el patrón react?

Este patrón necesita **modelos con razonamiento** para planificar, decidir el orden de *tools* y solicitar datos críticos. Con modelos sin razonamiento, el desempeño puede bajar.

- OpenAI: GPT-4 con buen equilibrio de razonamiento y velocidad. Familia “zero” (01, 03, 01 mini) con razonamiento fuerte; mayor costo y latencia. GPT-4.1 con alta inteligencia, pero no de razonamiento; podría reemplazarse por 01 o 03 según la tarea. Para triage, se menciona 4-0 mini; para tareas complejas, 01. También se cita 01 preview y 03, y opciones más económicas como 04 mini dentro de la serie “zero”.
- Google: **Gemini 2.5 Pro Thinking** con capacidades de *thinking* adecuadas y costo competitivo frente al mercado; 2.5 sin *thinking* y Flashlight sin estas capacidades.
- Anthropic: **Claude Opus 4.1** con razonamiento; alternativas en **Claude Sonnet 4** con razonamiento por defecto.

Habilidades que se practican con este patrón:

- **Planificación** de pasos y selección de *tools*.
- **Evaluación iterativa** de resultados y siguientes acciones.
- **Diseño de *prompts*** que guían decisiones y salidas.
- **Orquestación en grafo** con bifurcaciones y ruteo.
- **Control de iteraciones** para evitar ciclos infinitos.
- **Estructuración de salidas** con *structured output* cuando se requiere formato.

### **Implementación de Tools en ReAct Agents con LangChain Core**

Los grandes modelos de lenguaje pueden pensar, pero para actuar necesitan **tools** bien definidas. Aquí verás, paso a paso, cómo integrar *tools* en un **React Agent**, distinguir qué corre en la **capa de aplicación** y qué puede ejecutar el modelo, y cómo convertir un prompt en acciones reales como consultar una *API* o agendar una cita.

¿Cómo fluyen las tools desde el prompt hasta la capa de aplicación?

La interacción inicia con el request del usuario y pasa por tu aplicación, que actúa como wrapper del **large language model**. Con *tools*, el modelo no ejecuta la acción ni devuelve el resultado directo: primero identifica la herramienta y extrae parámetros, de forma parecida al **structured output**.

¿Qué retorna el modelo con tools y structured output?

- Devuelve un formato con el **function identifier** y los parámetros requeridos.
- Si faltan datos, **pide al usuario** lo que falta hasta estar “listo”.
- Cuando está listo, cambia de respuesta conversacional a **respuesta tool** con el nombre de la función y sus argumentos.

¿Dónde se ejecuta la tool: modelo o capa de aplicación?

- En general, las *tools* declaradas como **funciones** se ejecutan en tu **capa de aplicación**.
- Algunas *tools* son propias del modelo, como *FileSearch* de OpenAI, que corre con su infraestructura.
- Tras ejecutar la función en tu sistema, devuelves el resultado al modelo y este lo **interpreta y responde** al usuario. Ese es el ciclo completo de una *tool*.

¿Cómo definir una tool con LangChain Core y parámetros?

Se construye una función decorada como *tool* en *LangChain Core*. Así, el modelo puede mapear qué hace, cuándo usarla y con qué argumentos.

¿Qué incluir en la descripción y argumentos de la tool?

- Nombre claro, por ejemplo: *GetProducts*.
- Descripción orientada a uso: qué obtiene y para qué sirve.
- Argumentos tipados: por ejemplo, **precio** como entero para filtrar resultados.
- Contexto adicional: explica qué espera cada argumento, como harías en un prompt.

¿Cómo devolver resultados en texto para el modelo?

- Aunque podrías responder con arrays, el modelo entiende mejor **texto formateado**.
- Mapea y **concatena** los elementos (por ejemplo, producto y precio) para ofrecer una lista legible.
- Llama a la *tool* pasando un diccionario con los argumentos; si no hay argumentos, envía un diccionario vacío.

¿Cómo conectar la tool a una API y evitar alucinaciones?

Para información en tiempo real (clima, productos, etc.), no basta el conocimiento del modelo. Necesitas una *tool* que consulte una *API* y te devuelva datos actualizados. Así evitas respuestas vagas o alucinaciones.

¿Qué ejemplo práctico se implementa con GetProducts?

- Se parte de **fake data** para simular productos y luego se sustituye por una **API de productos de Platzi**.
- Se corrige el **endpoint** y se confirman los campos: **title** y **price**.
- La función devuelve los productos en texto con su precio, lista para que el LLM responda con claridad.
- Un ejemplo concreto es el agendador de citas: el modelo identifica la *tool* con parámetros como nombre del paciente, doctor y fecha; tu app llama a la *API* de agendamiento y regresa el resultado al modelo para que lo comunique.

¿Qué modelos convienen para razonar y responder rápido?

- Un modelo de razonamiento: “Claude Opus 4.1”, más lento pero con mejor análisis.
- Alternativa con equilibrio entre rapidez y razonamiento: “Gemini 2.5”.
- Además, se contrasta ampliar conocimiento con un “rack” vectorial frente a usar *tools*: puedes vectorizar productos y hacer retrieval, o conectarte a una *API* según el caso.

Ideas clave para poner en práctica:

- **React Agent y tools**: la *tool* define la acción, el modelo decide cuándo usarla.
- **function identifier y parámetros**: formato no conversacional que guía la ejecución.
- **Capa de aplicación**: ahí se hacen las llamadas reales a servicios y bases de datos.
- **Respuesta en texto**: formatea la salida para que el modelo continúe la conversación.
- **Evitar alucinaciones**: conecta *APIs* para clima, Wikipedia o tus propios sistemas.

### **Integración de tools con LLM y manejo de respuestas estructuradas**

Conecta tus *tools* a un *large language model* y conviértelas en respuestas claras para el usuario. Aquí verás cómo el modelo detecta funciones como *getProducts* y una *tool* de clima basada en *Geocoding* y *OpenAI OpenMethod*, por qué no las ejecuta, y cómo cerrar el ciclo con resultados formateados en el idioma de la conversación. Además, aprenderás a usar *bind_tools*, orientar con un *system prompt* y apoyarte en el patrón *React* para la iteración.

¿Cómo responde el modelo cuando agregas tools?

Cuando enlazas *tools*, el modelo cambia su comportamiento. **No ejecuta funciones**: identifica cuál llamar y con qué argumentos. Devuelve **texto más un objeto de *tool calls*** que indica la función objetivo y los parámetros extraídos del contexto y del historial.

- **No hay respuesta final** en la primera pasada. El modelo suele decir cosas como “Voy a consultar los productos disponibles de nuestra tienda.”.
- **Tú ejecutas la función** con los argumentos que el modelo sugirió.
- **Le devuelves el resultado** como *string* en la siguiente llamada.
- **El modelo reformatea** y entrega la respuesta al usuario en el tono e idioma del chat.

¿Qué es un tool call y qué información entrega?

Un *tool call* es la instrucción estructurada del modelo: **nombre de la función** a invocar y **argumentos** listos para ejecutar. Llega junto al texto, pero ese texto no es el resultado útil. Sirve como señal para que tu sistema llame a la *tool* correcta.

¿Cómo cerrar el ciclo de ejecución y reformulación?

- Ejecuta la función indicada con los argumentos propuestos.
- Pasa el resultado como *string* en el “botón de la respuesta”.
- El *LLM* usa ese dato para **reformular** y entregar el contenido final al usuario.
- La iteración puede automatizarse con el patrón *React*.

¿Qué pasa si no hay tool que ejecutar?

Si el mensaje no requiere *tools* (por ejemplo, un “hola”), el modelo **responde de forma conversacional**. Los *tool calls* solo aparecen cuando detecta que debe llamar una función.

¿Cómo construir la tool del clima con APIs?

Se crea una *tool* que recibe una ciudad, consulta una API de *Geocoding* para obtener latitud y longitud, y luego llama a *OpenAI OpenMethod* para el clima actual. **El flujo**: ciudad → *Geocoding* (latitud, longitud) → clima (temperatura, velocidad del viento) → salida como *string*.

- La ciudad se envía a *Geocoding*. Se procesa la respuesta como *JSON*.
- Con la latitud y longitud, se llama a *OpenAI OpenMethod* para el clima.
- Se formatea la respuesta en un *string* listo para el *LLM*.
- Ejemplo usado: “Bogotá” devolviendo temperatura y viento.

¿Cómo se agregan las tools al modelo?

Se crea una derivación del *large language model* original y se enlazan las *tools* con *bind_tools*: *getProducts* y *getWeather*. Luego se invoca con los mensajes actuales.

- El modelo detecta cuándo usar cada *tool*.
- Envía el *tool call* con argumentos listos.
- Tu sistema ejecuta y devuelve el resultado para que el *LLM* lo formatee.

```python
# src/agents/support/nodes/conversation/node.py — bind_tools real
from langchain.chat_models import init_chat_model
from agents.support.nodes.conversation.tools import tools

llm = init_chat_model("openai:gpt-4o-mini", temperature=1)
llm = llm.bind_tools(tools)
```


¿Qué incluir en el system prompt para guiar al asistente?

Defínelo como **asistente de ventas** capaz de **encontrar productos** y **dar el clima de una ciudad**. Enumera sus *tools* y la finalidad de cada una.

- Indica qué hace *getProducts*.
- Indica qué hace *getWeather*.
- Mantén el objetivo y el tono deseado.

¿Cómo infiere argumentos desde la conversación?

El modelo puede **inferir argumentos** a partir del historial. Si el usuario menciona “la capital de Colombia”, el modelo puede deducir “Bogotá” y preparar el argumento de “city” para la *tool* del clima. En escenarios como **agendamiento de citas**, puede convertir “mañana” o “en tres días” al **formato exacto** que le pidas para tu API.

¿Cómo definir formatos de entrada para fechas y ciudades?

- Especifica el **formato esperado** en el *prompt* (por ejemplo, estructura de fecha o clave “city”).
- El *LLM* extrae del contexto y **ajusta al formato** antes de sugerir el *tool call*.
- Tú solo ejecutas con parámetros ya listos.

¿Qué habilidades y keywords activan mejores resultados?

- Diseño de *prompts* y uso de *system prompt* claro.
- Definición de *tools*: *getProducts*, *getWeather*.
- Manejo de *tool calls* y argumentos.
- Consumo de APIs: *Geocoding* y *OpenAI OpenMethod* con latitud y longitud.
- Procesamiento de *JSON* y respuesta como *string*.
- Iteración con patrón *React* para cerrar el ciclo.

### **Implementación de agente ReAct para booking de citas médicas**

Un agente React bien diseñado acelera el booking de citas médicas con precisión. Aquí verás cómo estructurar un nodo, definir sus *tools*, preparar un *prompt* con reglas claras y probarlo en *standalone* con *LangGraph Studio*. El enfoque combina razonamiento del *language model* con salidas de *APIs* formateadas en texto plano para una experiencia fluida.

¿Cómo se arma un agente React con tools y prompt?

La base es un nodo tipo React: un agente, sus *tools* y un *system prompt*. Se crea con *create React Agent*, pasando el modelo, el arreglo de *tools* y el *prompt*. El modelo se inyecta directo: no hace falta un init especial. El *prompt* guía pasos, reglas y variables como today para interpretar expresiones temporales relativas.

¿Qué estructura de archivos usa el nodo booking?

Estructura mínima ordenada por responsabilidad: un *node*, su *prompt* y sus *tools*.

```text
booking/
  __init__.py
  node.py
  prompt.py
  tools.py
```

- Un nodo por responsabilidad: extractor, conversation y booking.
- Reutiliza *tools* existentes cuando convenga.
- Mantén ejemplos de React separados para no afectar el booking real.

¿Cómo se carga el prompt con reglas y today?

El *prompt* define el rol: asistente que agenda citas médicas. Incluye today como variable calculada si no se envía. Añade pasos y reglas para reducir errores del agente.

```python
system_prompt = """Eres un asistente que agenda citas médicas.
today: {today}
pasos:
1) obtener información del paciente.
2) obtener fecha y hora deseadas.
3) obtener información del doctor.
4) check de availability.
5) enviar sugerencias.
6) hacer booking.
reglas:
- usa book appointment solo si ya verificaste availability.
- no agendar a más de 30 días.
"""
```

- El *prompt* sigue siendo fundamental, incluso con patrón React.
- Los pasos guían el razonamiento y el orden de llamadas a *tools*.
- Reglas explícitas: primero *check* de *availability*, luego *book appointment*.

¿Cómo se integran tools existentes como getweather y getproducts?

Se importan, se agrupan en un *array* y se pasan al agente. Sirven para validar la arquitectura React antes del booking real.

```python
# src/agents/support/nodes/booking/node.py
from langchain.agents import create_agent
from agents.support.nodes.booking.tools import tools
from agents.support.nodes.booking.prompt import prompt_template

booking_node = create_agent(
    model="openai:gpt-4o-mini",
    tools=tools,
    system_prompt=prompt_template.format(),
)
```

- El agente formatea la salida de las *tools* y genera la respuesta final.
- Ejemplo práctico: listó productos y categorizó por tipo de prenda de forma autónoma.
- También combinó clima con catálogo y sugirió productos acordes a la temperatura.

¿Cómo se prueban el nodo y el agente en standalone?

El nodo booking se puede ejecutar en *standalone*: funciona como mini-nodo de *LangGraph* y como agente individual. Así se valida el flujo antes de integrarlo con extractor y conversation. En *LangGraph Studio* se inspeccionan llamadas a *tools*, *state* y mensajes del chat.

- Respuesta inicial: saluda, confirma nombre del paciente y pide fecha, hora y doctor.
- Entiende expresiones relativas: mañana, tarde, etc., gracias a today.
- Secuencia observada: primero usa get appointment availability, luego hace booking appointment y confirma.

¿Qué habilidades técnicas se aplican en la implementación?

- Diseño de nodos con patrón **React**: agente + *tools* + *prompt*.
- **Prompting** con pasos, reglas y variables como today.
- Reutilización e incorporación de **tools** externas.
- **Mocking** de *APIs* para acelerar pruebas.
- **Control de errores** en *tools*: devolver texto claro al modelo.
- **Formateo en texto plano**: respuestas legibles para el *language model*.
- Pruebas en **standalone** antes de integrar con *routing* y *chain*.

¿Qué herramientas de booking se definieron y qué parámetros aceptan?

Dos *tools* con foco en disponibilidad y reserva. Por ahora hacen *mocking*, listas para conectarse a tu *API* o calendario.

```python
# src/agents/support/nodes/booking/tools.py
from langchain_core.tools import tool

@tool("book_appointment", description="book a medical appointment for a given date, time, doctor and patient")
def book_appointment(date: str, time: str, doctor: str, patient: str) -> str:
    return f"Appointment booked for {date} at {time} with {doctor} for {patient}!"

@tool("get_appointment_availability", description="get the availability of a medical appointment for a given date, time and doctor")
def get_appointment_availability(date: str, time: str, doctor: str) -> str:
    return """
    The availability slots are:
    - Monday: 10:00-15:00
    - Wednesday: 10:00-15:00
    - Thursday: 10:00-15:00
    - Friday: 10:00-12:00
    """

tools = [book_appointment, get_appointment_availability]
```

- booking appointment: requiere fecha, tiempo, doctor y paciente.
- get appointment availability: requiere fecha, tiempo y doctor.
- Devuelven texto plano: fácil de interpretar y reformatear por el agente.

¿Cómo diseñar las tools de booking y el flujo de decisión?

El flujo se guía por el *prompt template*: primero recopilar datos, luego *check* de *availability*, sugerir horarios y finalmente reservar. Añade reglas como no agendar más de treinta días.

- Diseña salidas en texto claro: el modelo debe poder decidir con esa información.
- Si falla una *tool*: devuelve un mensaje de error en texto para que el agente lo comunique.
- Integra después con *routing* para derivar entre extractor, conversation y booking.

## Grafos Avanzados y Colaboración

### **Enrutamiento de agentes con conditional edge en LangGraph**

¿Quieres que tus agentes decidan por sí mismos y deriven la conversación al flujo correcto? Aquí verás cómo aplicar el patrón de **routing** con *conditional edge* para integrar un **booking agent** en una arquitectura con **nodos**, **estado compartido** y un **grafo** modular. Basado en un flujo real con *REACT*, *tools* y *chain*, entenderás qué decide el agente y qué controlas tú.

¿Qué es routing en agentes y por qué importa?

El patrón de **routing** permite que un agente elija el siguiente paso sin seguir un camino rígido. En un soporte con *chain*, extractor y conversation, este enfoque habilita enviar al usuario a un **booking agent** cuando desea “reservar una cita”, o mantenerlo en el agente de conversation (con un rack con OpenAI) cuando no necesita agendamiento. Esa capacidad de bifurcar el flujo, con reglas controladas por ti, hace que el sistema sea flexible y eficiente.

¿Qué diferencia hay entre nodos y edges?

- **Nodos:** actualizan el estado o generan nuevos estados en la memoria compartida.
- **Edges:** solo derivan hacia otros nodos. No actualizan el estado.
- Ambos pueden leer el estado, pero solo el nodo lo persiste.
- Un *edge* de routing devuelve los nodos posibles a los que puede enviar, con su tipado correspondiente.

¿Cómo se decide a dónde ir?

- Por lógica programada y técnicas de *prompt*.
- Por datos en la memoria compartida.
- Por salida del *language model* o uso de *tools*.
- Por azar, usando un umbral de *random* (por ejemplo, -0.5) para elegir entre dos nodos.

¿Cómo implementar un conditional edge en tu grafo?

Primero se replica el patrón de *prompt chain* en un *notebook*: nodo inicial, nodo 1, nodo 2, nodo 3 y nodo final. Luego se introduce una función tipo “route edge” cuyo objetivo es decidir el siguiente nodo y retornar los destinos posibles. Esa función puede leer el estado, pero no lo modifica.

¿Qué pasos componen la integración en el builder?

- Agregar un *conditional edge* en el *builder* como pieza de routing.
- Definir el flujo: *start* → nodo 1 → routing (*conditional edge*) → nodo 2 o nodo 3.
- Quitar conexiones directas innecesarias entre nodos cuando el *edge* ya decide el destino.
- Hacer que nodo 2 y nodo 3 terminen en *end*.
- Al compilar y graficar, el *conditional edge* no se dibuja; verás aristas a los nodos destino, y solo se tomará uno de ellos.

¿Qué reglas clave debes recordar?

- El *edge* puede acceder al estado, pero no lo actualiza.
- El nodo es el único responsable de persistir cambios en la memoria compartida.
- El flujo resultante crea bifurcaciones claras y controladas.

¿Puede el nodo start derivar directamente con routing?

Sí. No siempre necesitas un “nodo 1” antes de derivar. Se puede conectar el nodo *start* directamente a un *conditional edge* y, desde ahí, enviar al nodo 2 o nodo 3 para finalizar. Este patrón es útil cuando el enrutador analiza toda la conversación desde el inicio y decide el mejor camino sin procesamiento intermedio.

¿Qué te permite este patrón desde el inicio?

- Evaluar la intención del usuario al primer paso.
- Enviar de inmediato al **booking agent** si pide “reservar una cita”.
- Mantener al usuario en conversation con un rack con OpenAI si no requiere agendamiento.
- Reducir complejidad cuando un *edge* inicial puede tomar decisiones robustas.

¿Qué reto práctico puedes intentar ahora?

- Derivar a cuatro nodos en lugar de tres.
- Cambiar la lógica del *routing edge*: reemplazar *random* por reglas basadas en memoria.
- Colocar *routing* en otros nodos: por ejemplo, que el nodo 2 derive a más destinos.

### **Routing inteligente con LLM para derivar conversaciones automáticamente**

Construye un agente que decide por sí mismo a qué nodo enviar cada turno. Con el patrón de *routing* en LangGraph y un *structured output* guiado por un *language model*, el flujo se deriva de forma fiable a conversation o booking. Verás cómo integrar un subgrafo *React node*, usar memoria compartida y depurar errores comunes sin añadir complejidad innecesaria.

¿Cómo implementar routing con structured output en LangGraph?

Para que el agente tome decisiones autónomas, se añade un *router* entre el extractor y los nodos finales. El *router* llama al LLM con un *prompt* breve y devuelve un esquema tipado que indica el siguiente paso: conversation o booking. Así, cada mensaje se encamina al nodo correcto.

¿Qué nodos y flujo define el grafo?

- Inicio, extractor y memoria compartida. El extractor guarda datos útiles del historial en el estado común.
- Intent route. Un nodo de enrutamiento que decide el destino con *structured output*.
- Conversation node. Maneja preguntas generales con respuesta directa o con *RAG* cuando aplica.
- Booking node. Agente con patrón *React*, representado como subgrafo con agent, tools y finalizar.
- End. Ambos caminos convergen al cierre del flujo.

¿Cómo se construye el intent route con un LLM?

- Se define un esquema tipado para el paso siguiente con Pydantic: conversation o booking.
- Se pasa al LLM el historial completo más un *system prompt* que explica cuándo ir a cada nodo.
- Se establece un valor por defecto: si no hay decisión clara, ir a conversation.
- Los nombres deben coincidir exactamente con los nodos del grafo: errores de nombre impiden el ruteo correcto.

Ejemplo ilustrativo en Python:

```python
from typing import Literal
from pydantic import BaseModel

class IntentDecision(BaseModel):
    step: Literal["conversation", "booking"] | None = None

SYSTEM_PROMPT = ("Eres un asistente que enruta al paso adecuado: 'conversation' para preguntas generales, "
                 "'booking' si el usuario habla de citas o appointments.")

# src/agents/support/routes/intent/route.py
from pydantic import BaseModel, Field
from typing import Literal
from langchain.chat_models import init_chat_model
from agents.support.state import State

class RouteIntent(BaseModel):
    step: Literal["conversation", "booking"] = Field(
        'conversation', description="The next step in the routing process"
    )

llm = init_chat_model("openai:gpt-4o", temperature=0)
llm = llm.with_structured_output(schema=RouteIntent)

def intent_route(state: State) -> Literal["conversation", "booking"]:
    history = state["messages"]
    schema = llm.invoke([("system", SYSTEM_PROMPT)] + history)
    if schema.step is not None:
        return schema.step
    return 'conversation'
```

¿Cómo organizar el proyecto en nodes y routes?

- Carpeta nodes: define nodos como conversation, extractor y el booking node con patrón *React*.
- Carpeta routes: separa la lógica de enrutamiento. Incluye **init**.py, route.py y prompt.py para mantener el *prompt* del *router* y posibles tools.
- Ventajas: modularidad, claridad y posibilidad de evolucionar el *router* sin tocar los nodos.

¿Qué errores típicos se encontraron y cómo se corrigen?

Durante la integración surgieron fallos útiles para afinar el flujo. Identificarlos rápido evita diagnósticos erróneos del *prompt* o del modelo.

- Nombre del módulo mal escrito. Se intentó importar booking en lugar de booking node. Síntoma: “no puede importar ese módulo”. Solución: corregir el nombre exacto del nodo y evitar “refresh” innecesarios si la configuración de setapp-tools ya descubre módulos automáticamente.
- Condición lógica invertida. El chequeo usaba is none en vez de is not none, forzando el desvío a conversation aunque el LLM devolviera booking. Solución: validar que el esquema no sea nulo y devolver schema.step; si no existe, usar el valor por defecto conversation.
- Ajustes de *prompt* en el *router*. El clasificador debía contemplar variaciones como appointments, no solo “medical appointments”. Solución: afinar el lenguaje del *system prompt* con términos más generales.
- Falta de visibilidad al *debug*. No había impresiones del step devuelto. Solución: imprimir el esquema y usar un sistema de *monitoring* como LangSmith para inspeccionar decisiones y mejorar el *prompt*.

¿Cómo validar el agente con pruebas y buenas prácticas?

Probar con mensajes representativos confirma que el *router* toma decisiones correctas y que la memoria compartida da contexto a todos los nodos.

- Mensaje casual: “Hola, ¿cómo estás?”. Debe ir a conversation y responder con cortesía.
- Petición de cita: “Quiero una cita para mañana a las tres PM con el doctor Pérez”. Debe ir a booking; el extractor aporta nombre, fecha, hora y médico, y el agente *React* pregunta por datos faltantes si aplica.
- Disponibilidad y confirmación: el flujo de booking valida horarios y devuelve alternativas cuando no hay cupo, manteniendo la conversación en el historial compartido.
- Pregunta técnica general: “cómo mejorar el rendimiento de un website”. Debe ir a conversation y activar el *RAG* con la fuente disponible; conviene ajustar el *prompt* para respuestas concisas.

Buenas prácticas observadas:

- Usar el historial completo en el *router* para mayor precisión; si el costo crece, evaluar un resumen previo o basarse solo en el último mensaje.
- Incluir *few-shot* en el *system prompt* del *router* para desambiguar intenciones cercanas.
- Escoger un modelo adecuado: para clasificar, un LLM no razonador puede bastar; para booking con *React*, uno con mejor razonamiento mejora la calidad.
- Mantener consistencia de nombres de nodos y tipados en el *structured output*.

### **Paralelización de nodos en agentes con LangGraph**

Acelera la respuesta de tu agente dividiendo el problema en pasos independientes y ejecutándolos a la vez. Con el patrón de **paralelización**, varios nodos corren en paralelo y un nodo final, el *aggregator*, condensa todo en una única salida confiable. Así evitas esperas innecesarias y resultados duplicados.

¿Qué es el patrón de paralelización y cómo acelera a tu agente?

La **paralelización** permite que un agente envíe tareas a varios *workers* o nodos simultáneamente. A diferencia de *chaining* (secuencial) y *routing* (elige uno u otro), aquí se ejecutan varios caminos a la vez desde un mismo origen.

- Divide un problema en pasos que no dependen entre sí.
- Ejecuta nodos en paralelo en lugar de en secuencia.
- Usa un nodo final *aggregator* para condensar respuestas.

¿En qué se diferencia de *chaining* y *routing*?

- En *chaining*: un nodo tras otro, paso a paso.
- En *routing*: el grafo decide entre un camino u otro, no ambos.
- En paralelización: se ejecutan varios nodos al mismo tiempo y luego se unen los resultados.

¿Cómo definir nodos, *edges* y el rol del *aggregator*?

Para obligar la ejecución en paralelo, se elimina el *edge* que conecta de forma opcional un nodo con otro y se especifica explícitamente que, desde un nodo origen, se debe ir a dos destinos. Por ejemplo: desde el nodo 1 se va al nodo 2 y al nodo 3 a la vez. Ambos son obligatorios.

- Declara que desde el nodo origen se dispara al nodo 2 y al nodo 3 en paralelo.
- Haz que los nodos 2 y 3 apunten al *aggregator*.
- El *aggregator* condensa todo y emite el *end*.

En la visualización del grafo, los caminos obligatorios aparecen con línea sólida, mientras que los condicionales suelen verse como líneas punteadas. Esto señala que el flujo sí o sí pasará por esos nodos paralelos.

¿Por qué es crítico el *aggregator*? Porque, si los nodos en paralelo finalizaran con *end* por su cuenta, el agente podría intentar responder al usuario dos veces a la vez. El *aggregator* espera a que todos los nodos terminen, recopila sus salidas y produce una única respuesta final.

¿Cómo se refleja en el grafo *ASCII* la obligatoriedad?

- Línea sólida: camino obligatorio hacia el siguiente nodo.
- Línea punteada: camino condicional que depende de decisiones previas.
- Paralelización: múltiples líneas sólidas desde un mismo origen a varios nodos.

¿Cuándo iniciar varios nodos desde *start* y qué cuidar?

También es posible enviar varios nodos en paralelo directamente desde *start*. Por ejemplo: *start* dispara el nodo 1, el nodo 2 y el nodo 3 al mismo tiempo. Luego, todos convergen en el *aggregator* y de ahí se pasa al *end*.

- Desde *start* puedes lanzar múltiples nodos a la vez.
- Todos deben converger en un único *aggregator*.
- La salida final debe ser una sola: el *end*.

Para que funcione bien, los nodos paralelos deben ser **independientes**: ninguno debe esperar datos de otro. El *aggregator* resume y decide la respuesta final tras recibir todo.

### **Desarrollo de un agente de code review con análisis paralelo**

Diseña un flujo de revisión de código sólido y rápido con un agente especializado que ejecuta análisis en paralelo. Con un patrón de paralelización, dos revisores independientes detectan vulnerabilidades y problemas de mantenibilidad, y un tercer nodo agrega los hallazgos en un informe final claro. Aquí verás cómo se define el estado tipado, cómo se usan *structured output* y *schema*, y cómo se orquestan los nodos para ganar tiempo sin perder calidad.

¿Cómo funciona el agente de code review con patrón de paralelización?

El objetivo es ejecutar revisiones simultáneas sobre un mismo fragmento de código y consolidarlas en un resultado único. No es conversacional: recibe código, lo analiza y devuelve un reporte.

¿Qué flujo sigue el estado y los nodos?

- Se define un **estado** con el código de entrada y los espacios para los resultados parciales y finales.
- Desde el nodo inicial se lanzan en paralelo: **security review** y **maintainability review**.
- Ambos resultados llegan al nodo **aggregator**, que sintetiza y deja el **informe final** en el estado.
- La interfaz muestra líneas fijas: inicio ejecuta ambos nodos en paralelo, luego el *aggregator* y el final. En otros flujos (por ejemplo, con *React* o *tools*), algunas transiciones son opcionales o exclusivas, pero aquí son simultáneas por diseño.

¿Qué roles cubren security review y mantenibility review?

- Security review: detecta **vulnerabilidades**, inyección, riesgos y sugiere mitigaciones.
- Maintainability review: evalúa **legibilidad**, estructura, buenas prácticas y calidad del código.
- Ambos escriben en el estado usando formatos definidos por *schema* para facilitar el *parsing* y la agregación.

¿Qué hace el aggregator para el informe final?

- Lee los dos *schemas* del estado y produce un **resumen accionable**.
- Puede generar texto libre (sin *structured output*) cuando el objetivo es un reporte legible para el usuario.
- Recomienda acciones claras: sanitización de entradas, restricciones de API, tipado, nombres más expresivos, entre otras.

¿Cómo se definen el estado y el structured output del agente?

El estado es la columna vertebral: organiza entradas, salidas parciales y el reporte final. Usar *structured output* tipa cada nodo y mejora la consistencia del resultado.

¿Qué contiene el estado tipado del proceso?

- code: el fragmento de código a revisar.
- security_review: resultado del revisor de seguridad según su *schema*.
- maintainability_review: salida de mantenibilidad con su *schema*.
- final_review: texto del informe consolidado para el usuario.

¿Cómo se usa structured output y schema en los nodos?

- Security review define un *schema* con: lista de **suggestions** de vulnerabilidades, **risk level** y **suggestions** descriptivas.
- Maintainability review define: **concerns** sobre el código, **code quality** en escala de 1 a 10 y **recomendaciones** de mejora.
- Se menciona el uso de “Pydantic” para tipar los resultados: el *LLM* devuelve datos ya estructurados, listos para inyectarse en el estado sin *post-processing* complejo.

¿Qué modelo LLM y prompts se emplean?

- Modelo: **OpenAI GPT-4-4.1 mini**.
- Mensajería: *system message* y *user message* definidos con **tuplas** para simplicidad.
- Ejemplo de instrucción al usuario: “*review this code*” junto al código fuente.
- Recomendación: ampliar el *prompt* (no de una sola línea) para mejorar calidad, controlar inyección y, si conviene, usar formatos como XML para guiar la salida.

¿Cómo se implementa y prueba el flujo en paralelo?

El desarrollo prioriza agilidad: un archivo único llamado codereview, sin *scaffolding* complejo, útil para prototipado. Para proyectos grandes, conviene dividir prompts y nodos en carpetas.

¿Cómo se invocan los nodos con system message y user message?

- Cada nodo recibe el código desde el estado inicial.
- Se prepara el *system message* con el rol experto: seguridad o calidad.
- Se invoca el *LLM* con *structured output* y su *schema* correspondiente.
- Se guarda solo la parte del estado que cambió para mantener el flujo limpio.

¿Qué verás en LangGraph Studio durante la ejecución?

- Los dos nodos corren en **paralelo** y escriben sus resultados.
- El *aggregator* crea un **reporte final** legible con acciones priorizadas.
- El estado registra: vulnerabilidades medias con su lista, preocupaciones de mantenibilidad, puntuación de calidad y recomendaciones claras.
- Aunque no hay chat como tal, el estado concentra toda la evidencia del proceso.

¿Qué mejoras y reto final se proponen?

- Añadir un tercer revisor: **performance** para evaluar optimizaciones de rendimiento.
- Mejorar *prompts*: versiones extensas, con instrucciones, formato de salida y manejo de riesgos.
- Escalar la arquitectura: separar archivos por nodos y *prompts* cuando el proyecto crezca.

### **Patrón orchestrator para selección dinámica de nodos en paralelo**

Un agente eficaz no sigue un guion fijo: se adapta, decide y ejecuta lo imprescindible para resolver la tarea. Aquí aprenderás cómo el patrón **orchestrator** permite elegir dinámicamente qué nodos correr, cuándo hacerlo en paralelo y cómo sintetizar una única respuesta final con un **aggregator**.

¿Qué es el patrón orchestrator y por qué supera la paralelización y el routing?

El **objetivo** del patrón es claro: **seleccionar de forma dinámica** los nodos a ejecutar según el contexto y correrlos en paralelo solo cuando haga falta. A diferencia de otros patrones:

- En **paralelización**, siempre se ejecutan todos los nodos.
- En *routing*, se ejecuta uno u otro, nunca varios a la vez.
- En *orchestrator*, la selección es dinámica: uno, dos o tres, según la decisión del motor.

Esta decisión puede apoyarse en AI, el historial o reglas. El flujo típico: selección de nodos, ejecución en paralelo de los elegidos y síntesis con un **aggregator**. La estructura de salida y el historial ayudan a que el motor tome decisiones consistentes.

¿Cómo decide qué nodos ejecutar?

La decisión puede estar guiada por un *large language model*, reglas o incluso algo aleatorio para ilustrar el concepto. Lo importante es que el *orchestrator* actualiza el estado con los nodos seleccionados y esos se lanzan en paralelo. El orden de inicio puede variar y el de finalización también, por lo que el **aggregator** debe consolidar solo los resultados presentes y generar un **summary** robusto.

- Usa historial para identificar subtareas y prioridades.
- Emplea *structured output* para marcar qué agentes se requieren.
- Ejecuta en paralelo solo los nodos elegidos.
- Agrega resultados con un *aggregator* en una sola respuesta.

¿En qué ayuda HuggingGPT con el task planning?

Como inspiración, se emplea la idea de *HuggingGPT* para descomponer un *request* y asignar el mejor modelo por paso. Flujo típico:

- *Task planning*: dividir la solicitud en subtareas.
- Selección de modelos por subtarea.
- *Task execution*: correr cada modelo.
- *Aggregator* y *response generation*: integrar respuestas en una única salida.

Ejemplos comentados: describir una imagen y contar objetos, o generar una imagen con la pose de otra y luego describirla con voz. El *orchestrator* replica esta lógica: divide, elige modelos, ejecuta en paralelo y sintetiza.

¿Cómo implementarlo con send y una función asignar nodos?

Se parte de un template que hoy imita paralelización (siempre corre nodo 1, 2 y 3). El ajuste clave es mover la decisión al *orchestrator* para que elija qué nodos ejecutar y luego los dispare en paralelo con el comando *send*.

¿Cómo preparar el estado y actualizar los nodos?

El *orchestrator* decide y guarda en el estado la lista de nodos a ejecutar. Para ilustrar la idea se puede usar un criterio aleatorio; en producción, la decisión puede venir de un LLM con *structured output* y el historial.

```python
import random

def orchestrator(state: dict) -> dict:
    # Ejemplo pedagógico: decisión aleatoria de qué nodos correr
    posibles = [
        ["nodo_1"], ["nodo_2"], ["nodo_3"],
        ["nodo_1", "nodo_2"], ["nodo_2", "nodo_3"], ["nodo_1", "nodo_3"],
        ["nodo_1", "nodo_2", "nodo_3"]
    ]
    elegidos = random.choice(posibles)
    state["nodos"] = elegidos
    return state  # el orquestador actualiza el estado con los nodos elegidos
```

Puntos clave:

- El estado conserva la lista de nodos a ejecutar.
- La lógica de selección es intercambiable.

¿Cómo disparar ejecuciones en paralelo con send?

El *edge* de asignación lee el estado y envía, con *send*, una lista de nodos a ejecutar en paralelo. Cada envío puede llevar su propio estado.

```python
# src/agents/orchestrator.py — Send para dispatch dinámico
from langgraph.types import Send

def assign_nodes(state: State):
    nodes = state['nodes']
    return [Send(n, {}) for n in nodes]

# En el builder:
builder.add_conditional_edges("orchestrator", assign_nodes)
```

De forma explícita, sería equivalente a:

```python
# Equivalente explícito para los tres nodos:
Send("node_1", {})
Send("node_2", {})
Send("node_3", {})
```

Consideraciones prácticas:

- No es *routing* porque pueden ejecutarse varios.
- No es paralelización fija porque la lista es dinámica.
- El **aggregator** debe consolidar solo los resultados disponibles.

¿Cuándo aplicarlo en customer support y tareas multimodales?

En soporte, si el usuario pide dos cosas a la vez, por ejemplo: consejos para optimizar el sitio y agendar una cita con el doctor Pérez, el *orchestrator* podría lanzar en paralelo el agente de conversación y el de reservas, y luego unificar la respuesta. Aun así, se recomienda en soporte guiar a una sola tarea por turno, especialmente si se integra con canales como WhatsApp.

Dónde brilla el patrón:

- Solicitudes largas con múltiples subtareas en un solo mensaje.
- Casos multimodales: imagen, pose, voz y texto en cadena.
- Escenarios donde distintas herramientas o nodos deben coordinarse.

### **Evaluator Optimizer: ciclos de autocrítica para agentes de IA**

Un agente que se autocritica y mejora antes de responder eleva la calidad de salida. Con el patrón **Evaluator Optimizer**, un flujo con ciclo controla cuándo una respuesta está lista: genera, evalúa con criterios claros, recibe **feedback**, reintenta y solo finaliza si pasa la evaluación. Aquí verás cómo se arma en *LangGraph Studio* con *routing edge*, *conditional edge* y *structured output*.

¿Qué es el patrón evaluator optimizer y cómo funciona?

Este patrón crea un **ciclo de autocrítica** entre un *generator node* y un *Evaluator*. El generador produce una respuesta con un *language model*. El Evaluator la juzga según criterios definidos en el *prompt* y devuelve un veredicto. Si es correcta, se envía al final; si no, retorna al generador con **feedback** para mejorar.

- **Generador.** Produce un primer intento con un *large language model*.
- **Evaluator.** Aplica reglas definidas en el *prompt* y escribe su evaluación en el **state**.
- **Loop.** Si falla, el generador reintenta usando el feedback previo. Si aprueba, finaliza.
- **Criterios configurables.** Se definen en el *prompt* del Evaluator: tú decides qué es “bueno”.

Así, un simple *chain* evoluciona a un ciclo controlado donde el Evaluator decide si “va al end” o “regresa al generator”.

¿Cómo configurar el chain con routing edge y conditional edge?

Se parte de un *template* de *chain* con tres nodos: inicial, *generator node* y *Evaluator*. Para cerrar el ciclo, se agrega un **conditional edge** desde el Evaluator hacia un **routing edge**, que decide si se finaliza o se reintenta.

- **Routing edge con random.** Regla base: si el “promedio” es < 0.5, va a end; si no, regresa al generador. Esto permite ver ciclos aleatorios.
- **Flujo visual en LangGraph Studio.** El generador siempre va al Evaluator. El Evaluator puede finalizar o devolver. Se observan uno o varios ciclos según la condición.
- **Estado compartido.** El Evaluator deja su veredicto y feedback en el **state**. El routing edge lee el state y decide.

Ejemplo de la lógica del routing edge:

```python
# src/agents/evaluator.py — conditional edge con Literal real
from typing import Literal
from langgraph.graph import END

def route_edge(state: State) -> Literal[END, "generator_node"]:
    is_funny = state.get("is_funny", True)
    if is_funny:
        return END
    return "generator_node"

builder.add_conditional_edges('evaluator_node', route_edge)
```

¿Cómo integrar un ejemplo con language model para chistes y feedback?

Se implementa un generador de chistes con *structured output* en el Evaluator. El Evaluator devuelve si el chiste fue “gracioso” y, si no, un **feedback** para mejorar. El generador usa ese feedback y reintenta hasta pasar.

- **Structured output.** El Evaluator no responde conversacionalmente, sino con un esquema.

```json
{
    "gracioso": true | false,
    "feedback": "texto con sugerencias para mejorar"
}
```

- **Prompting del generador.** Si hay feedback en el **state**, el *prompt* cambia: “Escribe una broma sobre [topic] considerando el feedback y responde en español”. Si no hay feedback, solo usa el **topic**.
- **Parámetros del LLM.** Generador con temperatura 1 para variedad; Evaluator con temperatura 0 para consistencia. Para forzar el loop, se bajó la temperatura a 0 en ambos y se usaron *prompts* que favorecen chistes más “aburridos”.
- **Reglas explícitas en el Evaluator.** Se añadió un *system prompt* con un criterio: “un chiste gracioso debe tener más de dos párrafos”. Así, chistes cortos fallan, generan feedback y el generador los extiende en la siguiente iteración.

¿Qué criterios define el prompt del evaluator?

- Longitud mínima del chiste en párrafos.
- Calidad percibida: gracioso sí/no como **booleano**.
- Razón del fallo en **feedback** accionable.

¿Qué rol cumplen state, topic y feedback?

- **State.** Guarda el veredicto y el feedback del Evaluator.
- **Topic.** Tema base para generar la broma.
- **Feedback.** Instrucciones específicas para mejorar la siguiente versión.

¿Cómo se ve el ciclo completo con LangGraph Studio?

- Generador crea un chiste sobre el topic.
- Evaluator juzga con *structured output* y escribe en state.
- Routing edge lee el state: si gracioso, end; si no, regresa al generador.
- Generador reescribe aplicando feedback hasta aprobar.

Palabras clave y habilidades que se practican:

- **Evaluator Optimizer.** diseño de ciclos de mejora automática.
- **Routing edge** y **conditional edge.** control de flujo dinámico.
- **Structured output.** evaluación determinística con esquema.
- **Prompt engineering** para criterios y reintentos.
- **Temperatura del LLM** para creatividad vs. consistencia.
- **Gestión de estado** para pasar feedback entre nodos.

### Resumen: cuándo usar cada patrón de grafo

Esta tabla te ayuda a elegir el patrón correcto según tu caso de uso. Todos los scripts de referencia están disponibles en el repositorio del curso.

| Patrón | Referencia en el repo | Cuándo usarlo | Cuándo NO usarlo |
|---|---|---|---|
| **StateGraph simple** | `src/agents/simple.py` | Flujo lineal, un nodo, prototipo inicial | Cuando necesites decisiones o ciclos |
| **Prompt Chaining** | `src/agents/rag.py` | Pasos secuenciales con dependencia de datos entre ellos | Cuando los pasos son independientes entre sí |
| **Routing** | `src/agents/support/routes/intent/route.py` | Derivar el flujo según intención: 2-N destinos excluyentes | Cuando siempre se necesitan todos los nodos |
| **Paralelización** | `src/agents/code_review.py` | Análisis independientes sobre el mismo input | Cuando hay dependencias entre los análisis |
| **Orchestrator con Send** | `src/agents/orchestrator.py` | El número de nodos a ejecutar varía dinámicamente por contexto | Cuando el conjunto de nodos es siempre fijo |
| **Evaluator-Optimizer** | `src/agents/evaluator.py` | Generar → evaluar → reintentar hasta cumplir criterio de calidad | Sin criterio de calidad medible automáticamente |
| **ReAct (create_agent)** | `src/agents/react.py`, `src/agents/main.py` | Agente con tools que razona sobre cuándo y cómo usarlas | Flujo predecible que no requiere razonamiento iterativo |
| **Subgrafo como nodo** | `src/agents/support/nodes/booking/node.py` | `create_agent` embebido como nodo dentro de un grafo mayor | Cuando el subagente no necesita acceder al estado del grafo padre |

> El agente `support` combina tres patrones: Chaining (`extractor` → routing), Routing (conversation vs. booking) y ReAct (el nodo `booking` es un `create_agent` completo). Ver `src/agents/support/agent.py` para la implementación completa.

## Puesta en Producción

### **Exposición de agentes con FastAPI y endpoints REST**

Conecta tu agente inteligente al mundo con **FastAPI** y un **endpoint** claro, escalable y listo para producción. Aquí verás cómo levantar un servidor básico, crear un POST tipado para chat, invocar el agente con *Human message* y habilitar *streaming response* para una mejor UX, todo con pasos prácticos y probados en *Postman*.

¿Cómo exponer tu agente con FastAPI y un endpoint API?

Publicar el agente vía una **recipe API** permite que cualquier app web o móvil se conecte a tu servicio. El flujo es directo: instalar dependencias, crear un servidor básico, validar con un *Hello, world!* y luego añadir el endpoint que conecta con el agente.

¿Qué instala y cómo corre el servidor?

- Instala el paquete y prepara el entorno.
- Crea el archivo main.py dentro de tu carpeta API.
- Corre el servidor en modo desarrollo y verifica la URL.

```bash
uv add fastapi standard
uv run fastapi dev src/api/main.py
```

Ejemplo mínimo con dos *GET* (uno con parámetro):

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def hello():
    return {"message": "hello world"}

@app.get("/hello/{name}")
def hello_name(name: str):
    return {"hello": name}
```

- Verifica el “hello world”.
- Revisa la documentación automática en /docs con tus endpoints.

¿Cómo validar que la API responde?

- Abre la URL que imprime la consola al iniciar el servidor.
- Confirma el JSON esperado en el *GET* raíz.
- Entra a /docs para probar endpoints con la UI interactiva.

¿Cómo crear un endpoint post para chat con tipado?

Para recibir un mensaje y un ID de chat, usa un **POST** con cuerpo tipado. Esto facilita validaciones y escalabilidad.

¿Qué modelo de datos usa message y qué recibe?

- Define una clase que extiende de **BaseModel**.
- Acepta un campo string llamado message.
- El *endpoint* recibe el parámetro de ruta y el cuerpo JSON.

```python
from fastapi import FastAPI
from pydantic import BaseModel  # el transcript menciona extender de BaseModel

app = FastAPI()

class Message(BaseModel):
    message: str

@app.post("/chat/{chat_id}")
def chat(chat_id: int, item: Message):
    return {"chat_id": chat_id, "message": item.message}
```

¿Cómo probarlo con Postman?

- Crea un request tipo POST a /chat/12.
- Envía el JSON: { "message": "hola, ¿cómo estás?" }.
- Verifica que responde el chat_id y el mensaje.

¿Cómo conectar el agente, manejar asincronía y streaming?

La clave es **invocar el agente** con el mensaje del usuario y retornar solo el contenido útil. Puedes cargar variables de entorno al iniciar main.py y elegir entre invocación síncrona o asíncrona, según tu necesidad de rendimiento.

¿Cómo invocar el agent con human message?

- Importa tu agente, por ejemplo, el más completo: support.
- Crea un *Human message* con el contenido recibido.
- Invoca el agente y retorna el último mensaje en texto plano.

```python
from fastapi import FastAPI
from pydantic import BaseModel
# from agents import support as agent  # el transcript sugiere usar el agente "support"
# from langchain_core.messages import HumanMessage  # "Human message" según el transcript

app = FastAPI()

class Message(BaseModel):
    message: str

# Cargar variables de entorno al iniciar main.py (convencional, según el transcript).

@app.post("/chat/{chat_id}")
def chat(chat_id: int, item: Message):
    # response = agent.invoke([HumanMessage(content=item.message)])
    # Retornar solo el último mensaje como texto.
    # return {"text": response.last_message.text}
    return {"text": "Hola, estoy bien. Gracias, ¿en qué puedo ayudarte?"}
```

Notas prácticas:

- **Síncrono vs. asíncrono**: puedes usar agent.invoke o agent.ainvoke si tu flujo es *async*.
- **Estado por defecto**: el agente recibe un estado inicial y el *Human message* en un array.
- **Variables de entorno**: cárgalas antes de invocar al agente para evitar errores de conexión a keys.

¿Cómo mejorar la UX con streaming response?

- Usa el método agent.stream para enviar “pedacitos” a medida que se generan.
- Implementa un *endpoint* adicional, por ejemplo, /chat-stream, y consúmelo en tu UI.
- En web o móvil funciona bien; **WhatsApp no acepta streaming**.

Ejemplo conceptual del uso de stream:

```python
# for chunk in agent.stream([HumanMessage(content=item.message)]):
#     yield chunk  # la interfaz va pintando cada parte
```

Habilidades y conceptos trabajados:

- Exposición del agente mediante **recipe API** y **endpoint** público.
- Creación de servidor básico con *FastAPI* y verificación en /docs.
- Endpoints **GET** y **POST** con parámetros de ruta e input tipado.
- Uso de **BaseModel** para el modelo Message y cuerpo JSON.
- Pruebas con *Postman* para requests POST y validación de respuesta.
- Manejo de **variables de entorno** antes de llamar al agente.
- Invocación con **Human message** y retorno del **last message** en **texto plano**.
- Elección entre **síncrono** y **asíncrono** para rendimiento.
- Habilitación de **streaming response** para mejorar la **UX**.

### **Checkpointers de LangGraph para persistir estado en Postgres**

Evita que tu agente olvide cada interacción: con los **checkpointers de LangGraph** puedes guardar y derivar el estado de la conversación en una base de datos *Postgres* usando *Docker*, y controlar la **concurrencia** con un **thread ID** bien definido. Aquí aprenderás a instalar la librería, levantar *Postgres* y aplicar políticas de *threads* para que tu *endpoint* recuerde a cada usuario.

¿Qué resuelve un checkpointer de LangGraph y por qué importa?

Un agente sin memoria no avanza ni recuerda el nombre del usuario. Durante el *debugging* en *LangGraph Studio* hay memoria temporal, pero en un *endpoint* real el estado no se guarda. Un **checkpointer** crea un **snapshot** o **screenshot** del diálogo, lo asocia a un **thread ID** y lo persiste en una **base de datos** para restaurar: mensajes, memoria compartida y el nodo en el que quedó la ejecución.

- **El agente no recuerda por defecto**: sin estado persistente, cada pregunta empieza de cero.
- **Checkpointer**: guarda snapshots por *thread* para saber hacia dónde continuar o devolver la conversación.
- **Base de datos**: necesaria para recuperar el estado al consultar por *thread ID*.
- **Concurrencia**: cada usuario mantiene su propio estado sin interferir con otros.

¿Cómo funciona el guardado del estado por thread ID?

El **thread ID** define a quién pertenece la conversación y cuál estado cargar. Se pasa en la invocación del agente: “lo vamos a pasar a nivel de *invoke*, entonces siempre lo vamos a pasar aquí”. Cambias de conversación cambiando el ID; retomas un chat reutilizando el mismo ID.

¿Qué bases de datos e integraciones se mencionan?

- Oficialmente mantenidos por el equipo: *Postgres* y uno para *SQL Lite*. Recomendado usar *Postgres* por fiabilidad.
- Integraciones de la comunidad: *Django*, *Dynamo*, *Firestore*, entre otras, no mantenidas directamente por el equipo.

¿Cómo instalar la librería y levantar Postgres con Docker?

Primero instala la librería del checkpointer y prepara una base de datos *Postgres* con *Docker*. Luego conecta la librería a la base de datos para que persista los estados.

- Instalar la librería con *UV*.
- Crear un archivo dockercompose.yaml para *Postgres*.
- Quitar servicios innecesarios del *compose* como el visualizador.
- Levantar contenedores en segundo plano.
- Verificar que *Postgres* está arriba.
- Opcional: revisar en *docker dashboard* qué está corriendo.

¿Qué comandos necesitas?

```bash
# Instalar la librería del checkpointer
uv add langgraph-checkpoint-postgres

# Levantar Postgres con Docker en modo detach
docker compose up -d

# Verificar servicios activos
docker compose ps
```

¿Cómo pasar el thread ID al agente?

Configura el agente para recibir el **thread ID** en cada *invoke*. Es el identificador que decide qué estado cargar, de quién es la conversación y dónde retomar. Cambia el ID para empezar un hilo nuevo o reutilízalo para continuar el mismo.

¿Qué políticas de thread ID mejoran memoria y concurrencia?

Definir políticas de *threads* es clave para equilibrar recuerdo, rendimiento y costos. Elige la lógica que mejor se adapte a tu caso de uso.

- Relación uno a uno: usuario → un solo thread. Recuerda conversaciones aunque pase mucho tiempo. Puede degradar el contexto si el historial crece demasiado.
- Caducidad por tiempo: si el hilo supera 24 h, 48 h o una semana, se crea un **nuevo thread**. Mantiene al usuario enlazado, pero reinicia historial y estado de memoria compartida.
- Finalización por objetivo: cuando se resuelve la solicitud del usuario, se marca como finalizado y el siguiente mensaje abre un hilo desde cero, como en un call center.
- Concurrencia por usuario: el **thread ID** permite que “Juanito”, “Pepito” y “Fulanito” mantengan estados separados, cada uno con sus propios checkpoints.

### **Configuración de checkpointer dinámico con FastAPI y Postgres**

Conecta tu agente a una base de datos y preserva el historial sin dolores de cabeza. Aquí verás cómo construir un grafo con *checkpointer* dinámico, inicializarlo con *FastAPI* y *Postgres*, inyectar dependencias, y evitar que el contexto se corrompa al guardar solo lo esencial. Además, se señalan errores reales y cómo depurarlos con LangGraph Studio.

¿Cómo crear un checkpointer dinámico con FastAPI y Postgres?

Para que el agente recuerde y comparta estado, la configuración debe ser dinámica. La clave es recibir el *checkpointer* desde la app web y no “quemarlo” en el *build* del agente.

¿Cómo definir la función makegraph con configuración dinámica?

- Define una función que construya el grafo y reciba un *config* con el *checkpointer*.
- Envía el *checkpointer* al construir el agente.

```python
# makegraph.py
from typing import TypedDict, Optional

class GraphConfig(TypedDict, total=False):
    checkpointer: object  # instancia del checkpointer

def makegraph(config: GraphConfig):
    checkpointer = config.get("checkpointer", None)
    # construir el agente/grafo usando el checkpointer dinámico
    agent = build_agent(checkpointer=checkpointer)  # función de construcción existente
    return agent
```

- Ventaja: permite seguir usando LangGraph Studio para *debug* (si no pasas *checkpointer*, usarán uno propio) y, a la vez, integrarlo bien con *FastAPI*.

¿Cómo inicializar la conexión en el lifespan de FastAPI?

- Crea una instancia global para el *checkpointer* de *Postgres*.
- Inicializa antes de levantar la app con *lifespan* y ejecuta el *setup* para las tablas del estado.
- Evita credenciales “quemadas”; usa variables de ambiente. Si las “quemas”, es inseguro.

```python
# db.py
from contextlib import asynccontextmanager
from fastapi import FastAPI

checkpointer_global = None  # instancia global

@asynccontextmanager
async def lifespan(app: FastAPI):
    global checkpointer_global
    # ejemplo: lee de env en la práctica (aquí simplificado)
    dsn = "postgresql+psycopg://user:password@localhost:5432/db"
    checkpointer_global = PostgresCheckpointer(dsn)
    await checkpointer_global.setup()  # crea tablas para estado del grafo
    yield  # opcional: cerrar conexiones

def get_checkpointer():
    if not checkpointer_global:
        raise RuntimeError("checkpointer no inicializado")
    return checkpointer_global
```

¿Cómo invocar el grafo desde el endpoint con dependencia?

- Inyecta el *checkpointer* como dependencia.
- Construye el grafo con `makegraph` y pásale la instancia.

```python
# api.py
from fastapi import FastAPI, Depends
from db import lifespan, get_checkpointer
from makegraph import makegraph

app = FastAPI(lifespan=lifespan)

@app.post("/chat")
async def chat_endpoint(payload: dict, checkpointer=Depends(get_checkpointer)):
    agent = makegraph({"checkpointer": checkpointer})
    state = {"messages": [payload.get("message")]}  # además de otros campos de estado
    result = await agent.invoke(state)
    return result
```

- Tip: si usas el *endpoint* de *stream*, inyecta también la dependencia del *checkpointer*.

¿Cómo mantener limpio el estado y el historial del grafo?

El estado es memoria compartida. Si guardas metadatos “ruidosos”, el *prompt* y el *routing* se degradan. La solución: persistir solo el texto útil.

¿Qué guardar del AI message para no corromper el contexto?

- Problema observado: guardar la respuesta con metadata y *response* completos ensucia el historial.
- Solución: parsear el *AI message* y almacenar solo el texto cuando trabajes con texto plano.

```python
# al producir la respuesta en el nodo de conversation
raw_ai_message = await conversation_node(...)  # respuesta del modelo
clean_text = raw_ai_message.content if hasattr(raw_ai_message, "content") else str(raw_ai_message)

# guardar solo clean_text en historial/DB
save_message({
    "role": "ai",
    "content": clean_text,
})
```

- Beneficio: el *language model* recibe contexto claro. Evitas errores en *system history* y *routing*.

¿Cómo usar thread ID, CRUD y memoria compartida de forma segura?

- Cada conversación usa un *thread ID*. Si cambias el *thread ID*, inicias otra memoria desde cero.
- Guarda entrada y salida: `add_message` del usuario y también de la AI con su *chat ID*.
- Puedes reconstruir el estado desde la base: cargas historial y lo inyectas como `state` junto a campos como `customer_name`.
- Si un *thread* quedó “sucio”, crea uno nuevo y continúa con historial limpio.
- Buenas prácticas.
    - Persistir mensajes con *CRUD* simple..
    - Asociar por *chat ID*..
    - Evitar metadata innecesaria en el historial..

¿Cómo depurar errores frecuentes con LangGraph Studio y el API?

La depuración combina impresión rápida, revisión del historial y ajuste del *routing*. Estos fueron fallos típicos y su enfoque.

¿Qué hacer ante internal server error e invalid request?

- Verifica que ya no invocas al agente directo: usa `makegraph` con *checkpointer* en el *endpoint*.
- Imprime el último *message* para validar formato de entrada. Aunque no es lo ideal, un `print` veloz ayuda a aislar el problema.
- Revisa si el error proviene del *extractor* y no del nodo de conversación. Ajusta esa etapa primero.

¿Cómo revisar system history y routing con LangGraph Studio?

- Usa LangGraph Studio para ejecutar la función constructora del grafo y ver el *system history*.
- Imprime el historial y valida que no contenga metadatos no deseados.
- Si el primer *thread* se creó sin *checkpointer*, puede haber historial viejo. Crea un *thread* nuevo y prueba.

¿Cómo optimizar el flujo con booking e intent route?

- El *booking* (creative rig agent) comparte estado completo y suele manejar mejor el historial limpio.
- Si el *rack* de *OpenAI* solo toma el último mensaje, ajusta el *prompt* o define un *custom rack* según el caso.
- Guía con *intent route* hacia el agente correcto cuando el usuario pida acciones como citas médicas.
- Señales de mejora.
    - Evitar búsquedas a *file search* para preguntas simples..
    - Inyectar *prompt* con datos del usuario si corresponde..
    - Limpiar también la salida del agente de *booking* si añade metadata..

### **Patrones avanzados de LangGraph para agentes complejos**

Crear agentes avanzados exige una combinación de habilidades claras y patrones comprobados. Aquí encontrarás una guía práctica para entender el rol emergente de **ingeniero de contexto**, explorar **patrones LangGraph** listos para probar y afianzar las **skills** necesarias para construir sistemas con control, memoria y potencia.

¿Qué es el ingeniero de contexto y por qué será clave?

El ingeniero de contexto —también llamado *agent engineer*— integra los **skills** que permiten crear agentes robustos y seguros. La responsabilidad central es **diseñar y gestionar el contexto** que consumirá la *language model*: estado, historial, memoria y formatos de salida.

- **Técnicas de Rack.** Conjunto de prácticas para enriquecer y organizar el contexto que recibe el modelo. Ayudan a mejorar precisión y relevancia.
- **Manejo del estado e historial.** Evita que el historial se corrompa, decide qué conservar y qué descartar, y define cómo resumir. Es parte crítica del contexto que verá la *language model*.
- **Memoria.** Estrategias para persistir información útil entre turnos y sesiones sin perder control.
- **Prompt engineer.** Sigue siendo fundamental para alinear instrucciones, delimitadores, roles y ejemplos.
- **Structural outputs.** Diseña salidas estructuradas (por ejemplo, JSON) que facilitan orquestación y validación.

En conjunto, estas capacidades permiten agentes con un **equilibrio entre autocontrol y supervisión humana**, listos para tareas reales.

¿Qué patrones de LangGraph puedes probar hoy?

LangGraph ofrece patrones prácticos para coordinar múltiples agentes y *tools* con transparencia en cada paso. Dos repositorios experimentales destacan por su propuesta de arquitectura:

¿Cómo funciona el patrón supervisor en LangGraph?

- **LangGraph Supervisor.** Implementa el patrón supervisor: en lugar de decidir qué *tool* llamar, **decide qué agente invocar**. Creas varios agentes (por ejemplo, varios *Rake Agent*) y un supervisor que los **gestiona**.
- Beneficio clave: orquesta decisiones de alto nivel con control explícito sobre el flujo.
- Nota importante: es experimental y puede migrar a otra librería. Conviene revisarlo antes de integrarlo en producción.

¿Qué aporta el patrón swarm para una granja de agentes?

- **Swarm.** Similar a Supervisor, pero opera como **granja de agentes**. Administra sin supervisar: elige el agente adecuado **según el contexto y el historial**.
- Flujo típico: crear varios *Rake Agent*, configurar el *check pointer* y activar el modo *Swarm* para delegar la elección.
- Ventaja: simplifica la selección del agente correcto con menos reglas manuales.

¿Cómo publicar tu agente con FastAPI de forma práctica?

- **FastAPI LangGraph.** Un template de servidor *FastAPI* para exponer tu agente con funcionalidades ya resueltas: **historial persistente**, **streaming** y **endpoints** listos para consultar y administrar la conversación.
- Úsalo para clonar y montar tu agente o para **tomar ideas del código** y adaptarlo a tu servidor.

Ten presente que estos repositorios están en exploración. LangGraph podría incorporarlos a su librería principal o moverlos a espacios externos. Aun así, con lo ya aprendido, es posible **probarlos** y evaluar su encaje en tus flujos.

¿Qué aprendiste para crear agentes potentes con LangGraph?

A lo largo del aprendizaje, el foco fue combinar control explícito con flexibilidad. Con LangGraph puedes construir patrones como *routing*, *orchestrator*, *evaluator* y *optimizer*, y decidir cómo pasan las acciones dentro del grafo.

- **Control del estado.** Define variables de conversación, resultados intermedios y banderas de control.
- **Gestión del historial.** Evita corrupción, resume y recorta con criterio.
- **Conexión de nodos con la *language model*.** Diseña nodos y transiciones claras para cada decisión.
- **Structural outputs.** Emite formatos validados para consumir en otras partes del sistema.
- **Llamar agentes y usar *tools*.** Implementa uno de los patrones más comunes: **los Rake Agents** con *tools*, y aprende a **orquestarlos** y **optimizar** su comportamiento.
- **Balance y poder.** El framework permite agentes con **autocontrol** y, al mismo tiempo, **tu control** sobre reglas, memoria y decisiones.
- **Escenarios reales.** Desde responder tickets y clasificar, hasta investigar y resolver problemas complejos en una compañía, gracias a contextos bien diseñados y patrones consistentes.

La *language model* seguirá mejorando y ampliando ventanas de contexto, pero la **ventaja competitiva** está en cómo la controlas: **contexto bien diseñado, estado estable, historial curado y salidas estructuradas**. Así se construyen sistemas confiables y escalables.
---

### Consideraciones adicionales para producción

#### Observabilidad con LangSmith

LangSmith permite inspeccionar cada ejecución del grafo: qué nodos se activaron, qué tokens consumió cada LLM y dónde falló. El proyecto ya tiene las variables configuradas en `.env`:

```bash
LANGCHAIN_TRACING_V2=true
LANGSMITH_API_KEY=tu_langsmith_key
LANGSMITH_ENDPOINT=https://api.smith.langchain.com
```

Con estas variables activas, todos los grafos compilados emiten trazas automáticamente sin cambios en el código. Accede a las trazas en [smith.langchain.com](https://smith.langchain.com).

#### Variables de entorno seguras

El archivo `src/api/db.py` tiene `DB_URI` hardcodeado. Para producción usa siempre variables de entorno:

```python
# src/api/db.py — patrón correcto
import os
DB_URI = os.getenv("DB_URI")
if not DB_URI:
    raise RuntimeError("DB_URI no configurada en variables de entorno")
```

#### Gestión del historial en producción

Sin límite, el historial crece en cada turno y encarece cada llamada al modelo. Estrategias:

- **Enviar solo el último mensaje**: adecuado para el RAG (ya implementado en `src/agents/rag.py`).
- **Recortar por tokens**: usar `trim_messages` de LangChain para mantener un máximo de tokens.
- **Nodo de resumen periódico**: cada N mensajes, un nodo comprime el historial con un LLM.
- **Por nodo**: el extractor puede necesitar el historial completo; el nodo de conversación puede trabajar solo con los últimos 5 mensajes.

#### Compatibilidad de streaming por canal

```python
# src/api/main.py — endpoint de streaming SSE
@app.post("/chat/{chat_id}/stream")
async def stream_chat(chat_id: str, message: Message, checkpointer: CheckpointerDep):
    async def generate_response():
        agent = make_graph(config={"checkpointer": checkpointer})
        for message_chunk, metadata in agent.stream(
            {"messages": [HumanMessage(content=message.message)]},
            stream_mode="messages"
        ):
            if message_chunk.content:
                yield f"data: {message_chunk.content}\n\n"
    return StreamingResponse(generate_response(), media_type="text/event-stream")
```

| Canal | Soporta streaming | Endpoint recomendado |
|---|---|---|
| Web / SPA | Sí | `/chat/{id}/stream` con SSE |
| WhatsApp (Twilio, 360dialog) | No | `/chat/{id}` síncrono |
| Mobile iOS/Android | Depende de la librería HTTP | `/chat/{id}/stream` con manejo de chunks |
| Slack | No nativo | `/chat/{id}` síncrono |

---

### Errores comunes y cómo resolverlos

#### Errores de imports

| Síntoma | Solución |
|---|---|
| `ModuleNotFoundError: No module named 'langgraph.state'` | `from langgraph.graph import MessagesState` |
| `ModuleNotFoundError: No module named 'langchain.schema'` | `from langchain_core.messages import HumanMessage, AIMessage, SystemMessage` |
| `ModuleNotFoundError: No module named 'langchain.prompts'` | `from langchain_core.prompts import PromptTemplate` |
| Error al usar `template_format="ninja_two"` | Usar `template_format="jinja2"` e instalar con `uv add jinja2` |
| `ImportError: cannot import name 'init_chat_model' from 'langchain'` | `from langchain.chat_models import init_chat_model` |

#### Errores de estado

| Síntoma | Solución |
|---|---|
| `KeyError` al acceder a una clave del estado | Usar `state.get("key", default)` en lugar de `state["key"]` |
| El historial se sobreescribe en lugar de concatenarse | Con `MessagesState`, retornar `{"messages": [new_message]}` — el reducer concatena automáticamente |
| El estado no se actualiza entre nodos | Siempre retornar un dict con las claves modificadas: `return {"customer_name": value}` |

#### Errores de routing

| Síntoma | Solución |
|---|---|
| El agente siempre va al mismo nodo | Condición invertida: verificar `if schema.step is not None: return schema.step` |
| `ValueError: Node 'X' not found` | Los nombres deben coincidir exactamente: `builder.add_node("conversation", ...)` y `return "conversation"` |
| El router no detecta la intención correcta | Ampliar los términos del system prompt: cubrir variantes como "appointments", "cita", "agenda" |
| Ciclo infinito en el Evaluator-Optimizer | Añadir contador al estado y condición de salida: `if state.get("attempts", 0) >= 3: return END` |

#### Errores en producción (FastAPI + Postgres)

| Síntoma | Solución |
|---|---|
| `RuntimeError: Checkpointer not initialized` | Verificar `app = FastAPI(lifespan=lifespan)` y que el endpoint use `CheckpointerDep` como dependencia |
| El agente no recuerda el contexto entre requests | Usar el mismo `chat_id` como `thread_id` en el config de forma consistente |
| `OSError: [Errno 48] Address already in use` | `lsof -ti :8000 \| xargs kill -9` |
| Error de conexión a Postgres al arrancar | `docker-compose up -d` y verificar con `docker ps` |
| `psycopg ImportError: no pq wrapper available` | `pip install "psycopg[binary]"` |
