# Sistema de Priorización "Keep It Simple" — Prompts de Onboarding

> **Contexto**: Este es un sistema de 5 sesiones (pueden ser en una sola sentada o repartidas) para que un founder, director de PYME o de ONG configure su propio sistema de priorización diaria con AI.
>
> **Stack**: Claude (Code o Desktop) + Obsidian + Granola
>
> **Filosofía**: La persona usa AI desde el minuto uno. No "aprende sobre AI" primero. Resuelve su problema real y, de paso, ya está usando AI.
>
> **Resultado esperado**: Al terminar, la persona tiene un ritual diario que le genera 3 tareas priorizadas (1 difícil + 2 fáciles) y un sistema mínimo de captura y revisión.

---

## Anatomía del sistema final

El onboarding produce estos componentes (archivos .md en Obsidian):

| Componente | Qué es | Ejemplo |
|---|---|---|
| **Prompt maestro** | El ritual diario/semanal | "Sos mi coach de productividad. Revisá mi inbox y mis reuniones, y dame 3 tareas..." |
| **Memoria** | Contexto personal | Rol, estilo de trabajo, resistencias, ritmos |
| **Principios** | Reglas guía | "1 difícil + 2 fáciles", "mañana = pensar, tarde = hacer" |
| **Inbox** | Brain dump | Archivo donde tirar ideas sueltas |
| **Estructura** | Carpetas mínimas | clientes/, hoy.md, focus.md, inbox.md |

---

## PROMPT 1 — "El espejo" (Diagnóstico de cómo priorizás hoy)

### Instrucción para el coach

> Antes de armar nada, necesitamos entender cómo funciona esta persona HOY. No asumimos nada. Le pedimos que use Claude para generar un auto-diagnóstico. Esto logra dos cosas: (1) rompe la hoja en blanco, (2) la persona ya está usando AI.

### Lo que le decís al founder

"Antes de armar tu sistema, quiero que entiendas cómo priorizás hoy. Abrí Claude y pegá este prompt:"

### El prompt que pega el founder

```
Necesito tu ayuda para hacer un auto-diagnóstico de cómo priorizo mi trabajo.
Te voy a contar cómo es mi día típico y vos me vas a hacer preguntas cortas
para entenderme mejor. Después quiero que me devuelvas un resumen de 300 palabras
con dos secciones:

1. LO QUE ME FUNCIONA — hábitos, herramientas o formas de trabajar que ya tengo y me sirven
2. LO QUE NO ME FUNCIONA — dónde pierdo tiempo, qué postergo, qué me genera ansiedad

Empezá preguntándome: ¿Cómo arrancás un día típico de trabajo? ¿Qué es lo primero que hacés?
```

### Qué esperar

- Claude va a hacer 4-6 preguntas conversacionales
- El founder termina con un resumen de 300 palabras que ya le da claridad
- **Ese resumen es el primer insumo para el sistema**

### Indicación al coach

Pedile que te comparta el resumen. Leelo juntos. Subrayá las frases clave (las vas a usar en el Prompt 3).

---

## PROMPT 2 — "Los principios" (Qué reglas guían tus decisiones)

### Instrucción para el coach

> Ahora buscamos los principios que ya tiene la persona (conscientes o no) y le proponemos algunos que podrían servirle. No es teoría: son reglas operativas para el día a día.

### Lo que le decís al founder

"Ahora vamos a identificar tus reglas de juego. Pegá este prompt en la misma conversación de Claude:"

### El prompt que pega el founder

```
Basándote en lo que te conté, quiero que identifiques:

1. PRINCIPIOS QUE YA TENGO — reglas que ya sigo (aunque no las haya dicho explícitamente).
   Ejemplo: "Priorizo lo urgente sobre lo importante" o "Trabajo mejor solo que en equipo".

2. PRINCIPIOS QUE ME PODRÍAN SERVIR — basándote en mis problemas, sugerí 3 principios
   simples que podría probar. Que sean accionables y concretos.
   Ejemplo: "1 tarea difícil + 2 fáciles por bloque de trabajo" o "Si no cabe en 3 tareas, no es de hoy".

Para cada principio, explicá en una línea por qué creés que me serviría a MÍ específicamente.
```

### Qué esperar

- Claude identifica 2-3 principios implícitos y sugiere 2-3 nuevos
- El founder elige cuáles le resuenan
- **Esos principios van a ser la base del prompt maestro**

### Indicación al coach

Discutí con la persona cuáles principios elige. Proponele que pruebe al menos uno nuevo durante 2 semanas ("como dejar el azúcar — probá y después decidís"). El principio recomendado por defecto es: **1 difícil + 2 fáciles**.

---

## PROMPT 3 — "El mapa" (Contexto, herramientas y estructura)

### Instrucción para el coach

> Necesitamos saber dónde vive la información de esta persona: clientes, proyectos, notas, reuniones. Esto define la estructura mínima del vault de Obsidian.

### Lo que le decís al founder

"Ahora necesito entender dónde tenés tu información hoy. Pegá esto:"

### El prompt que pega el founder

```
Ayudame a hacer un inventario rápido de mi sistema actual de información.
Haceme preguntas cortas sobre:

1. ¿Dónde anoto mis tareas hoy? (app, papel, cabeza, nada)
2. ¿Tengo una lista de clientes/proyectos activos en algún lado?
3. ¿Uso alguna herramienta para reuniones/notas? (Granola, Notion, Google Docs, nada)
4. ¿Tengo algún lugar donde hago "brain dump" de ideas sueltas?
5. ¿Reviso alguna vez lo que hice la semana pasada?

Después de mis respuestas, armá:
- MAPA ACTUAL: dónde está mi información hoy (en una tabla simple)
- ESTRUCTURA MÍNIMA PROPUESTA: qué archivos/carpetas necesitaría en Obsidian
  para tener un sistema básico de priorización. Máximo 5 archivos. Menos es más.
```

### Qué esperar

- Un mapa de dónde vive la información actual
- Una propuesta de estructura mínima (ej: `inbox.md`, `hoy.md`, `focus.md`, `clientes/`)
- **Esto define la arquitectura del vault**

### Indicación al coach

Si la persona no usa Obsidian todavía, ayudala a instalarlo y crear el vault con la estructura propuesta. Si ya lo usa, adaptá la propuesta a lo que ya tiene. La clave es **no crear más de 5 archivos**.

---

## PROMPT 4 — "El ritual" (Generación del prompt maestro diario)

### Instrucción para el coach

> Este es el momento cumbre. Con el diagnóstico (Prompt 1), los principios (Prompt 2) y la estructura (Prompt 3), ahora Claude genera el prompt maestro personalizado. Este prompt es lo que la persona va a correr cada mañana.

### Lo que le decís al founder

"Ahora vamos a crear tu ritual diario. Este es el prompt que vas a usar cada mañana para que Claude te ayude a priorizar. Pegá esto:"

### El prompt que pega el founder

```
Con todo lo que sabés de mí hasta ahora, necesito que me generes un PROMPT MAESTRO
que voy a usar como ritual diario en Claude Code (dentro de mi vault de Obsidian).

El prompt tiene que:

1. DESCRIBIR MI CONTEXTO — quién soy, qué hago, cómo trabajo mejor
2. DEFINIR EL ROL DE CLAUDE — sos mi coach de productividad, no un asistente genérico
3. INCLUIR MIS PRINCIPIOS — las reglas que elegí para priorizar
4. DESCRIBIR EL RITUAL — qué tiene que hacer Claude cada vez que lo corro:
   - Revisar mi archivo inbox.md (brain dump)
   - Revisar mis notas de reuniones recientes (si las hay)
   - Proponerme 3 tareas: 1 difícil + 2 fáciles (o los principios que elegí)
   - Lo que no entra hoy, dejarlo en el inbox para después
5. SER BREVE — máximo 40 líneas. Si es más largo, no lo voy a usar.

Formato: generá el archivo como un bloque de código markdown que pueda copiar y pegar
directo en mi vault de Obsidian como archivo .md en la carpeta .claude/commands/
```

### Qué esperar

- Un prompt maestro personalizado, listo para copiar
- Que refleje el estilo, ritmos y principios de la persona
- **Este archivo es el corazón del sistema**

### Indicación al coach

Revisalo junto con la persona. Preguntá: "¿Esto te suena a vos o suena genérico?" Si suena genérico, iterá. El prompt tiene que sonar como un coach que LA conoce.

---

## PROMPT 5 — "La prueba" (Primera corrida del sistema)

### Instrucción para el coach

> No hay mejor forma de validar que corriéndolo. Ahora mismo. En vivo. Si funciona, la persona se va con el sistema andando. Si no, iteramos.

### Lo que le decís al founder

"Vamos a probarlo ahora. Abrí Claude Code en tu vault de Obsidian. Antes de correr el ritual, hacé dos cosas:"

### Paso 1 — Cargar el inbox

"Abrí `inbox.md` y tirá ahí 5-10 cosas que tenés en la cabeza ahora mismo. No importa el formato, no importa si son importantes o no. Brain dump de 2 minutos."

### Paso 2 — Correr el ritual

"Ahora corré el comando del ritual (el prompt maestro que acabamos de crear)."

### Paso 3 — Evaluar juntos

Después de que Claude genere las 3 tareas, preguntale a la persona:

1. **"¿La difícil es realmente la difícil?"** — Si no, el prompt necesita ajuste en cómo detecta resistencia
2. **"¿Las fáciles son alcanzables hoy?"** — Si no, el prompt está siendo ambicioso
3. **"¿Sentís que te sacó algo de la cabeza?"** — Si sí, el sistema ya está funcionando

### Indicación al coach

Si la persona dice "sí, me sirve", el onboarding terminó. Dejalo así. **No agregues más**. La evolución viene después, orgánicamente, cuando la persona diga "quiero más". Ahí sí podés ofrecer: ritual semanal, eco-cycle de iniciativas, dashboard, etc.

---

## Secuencia resumida

| # | Nombre | Duración | Output |
|---|--------|----------|--------|
| 1 | El espejo | 10 min | Diagnóstico de 300 palabras |
| 2 | Los principios | 10 min | 3-4 principios elegidos |
| 3 | El mapa | 10 min | Estructura de 5 archivos max |
| 4 | El ritual | 15 min | Prompt maestro personalizado |
| 5 | La prueba | 10 min | Primera corrida real del sistema |
| **Total** | | **~55 min** | **Sistema funcionando** |

---

## Camino de evolución (NO incluir en el onboarding)

Una vez que la persona usa el sistema diario por 2+ semanas, podés ofrecer:

1. **Ritual semanal** — Revisión de qué logró, qué postergó, qué patrones ve
2. **Integración Granola** — Que el ritual lea transcripts de reuniones y extraiga pendientes automáticamente
3. **Focus semanal** — Un archivo con los 3 focos de la semana (arriba de las tareas diarias)
4. **Dashboard estratégico** — Eco-cycle de iniciativas, matriz de impacto (el FlightOS simplificado)

Cada paso se agrega SOLO cuando la persona lo pide o demuestra que ya domina el anterior.

---

## Notas de diseño

- **Por qué 5 prompts y no 1 mega-prompt**: Cada prompt genera una conversación. La persona reflexiona, Claude aprende. Un mega-prompt saltea la reflexión.
- **Por qué la persona pega los prompts (en vez de que lo haga el coach)**: Porque queremos que la persona sepa hacer esto sola después. El coach es un facilitador, no una dependencia.
- **Por qué máximo 40 líneas en el prompt maestro**: Si es más largo, no lo va a leer, no lo va a entender, no lo va a mantener. Keep it simple.
- **Por qué 1 difícil + 2 fáciles**: Es el principio de Gaspar, validado en la práctica. La difícil ataca la procrastinación, las fáciles dan sensación de progreso.
