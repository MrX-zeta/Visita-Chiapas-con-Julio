---
name: visita-chiapas-con-julio
description: Contexto, reglas de negocio y protocolo de trabajo del proyecto Visita Chiapas con Julio (identidad visual, sitio web y reservas). Úsala antes de escribir código, textos, precios o diseño de este proyecto, y al ejecutar una tarea de ai/handoff.
---

# Visita Chiapas con Julio

Negocio de transporte terrestre privado con operador en San Cristóbal de las Casas, Chiapas. Se renta la **unidad completa** con operador; nunca se comparte. El proyecto incluye identidad visual, un sitio de una página y, más adelante, un sistema de reservas.

## Antes de empezar

1. Lee `ai/context/estado-actual.md` (dónde va el proyecto).
2. Busca en `ai/context/knowledge-graph.json` los nodos que toca tu tarea **con Grep por id**, sin leer el archivo completo:
   - Reglas duras: `INV-01` a `INV-15` (léelas siempre).
   - Negocio `NEG-*`, flota `UNI-*`, servicios `SRV-*`, destinos `DST-*`, paquetes `PAQ-*`, tarifas `TAR-*`, políticas `POL-*`.
   - Marca `MRC-*`, decisiones `DEC-*`, datos contradictorios `INC-*`, pendientes `PEND-*`, fuera de alcance `FDA-*`.
3. Si vienes por una tarea, sigue `ai/handoff/README.md`.

## Reglas que más se rompen

- Se dice **«operador»**, nunca «chofer». Los vehículos son **«unidades»**.
- El nombre es exactamente **«Visita Chiapas con Julio»**.
- Nada de tours colectivos ni de precio «por asiento».
- No inventes reseñas, testimonios, cifras ni credenciales. Solo se publica lo que Julio puede comprobar.
- Precios, destinos y unidades se leen del **archivo de datos único**. No se escriben a mano en componentes.
- Los colores salen de los tokens. La terracota `#BE6A47` no se usa en texto de tamaño normal.
- Todo el texto va en español.
- Si un nodo está en `propuesto`, `pendiente`, `preliminar` o tiene un `INC-*` encima, **no lo resuelvas tú**: anótalo en el reporte.

## Marca en breve

- Paleta: azul tinta `#334351`, crema `#FBF3E6`, terracota `#BE6A47` (para texto se propone `#A65A3B`).
- Logo: cordillera de trazo continuo y ruta punteada terracota. El favicon es solo la montaña. El monocromo es variante obligatoria.
- Personalidad: confiable, cálido, formal sin ser corporativo, cercano, local. **No es** lujo frío, aventura extrema, turismo masivo ni agencia genérica.
- Garet solo vive en el logo, trazada. La tipografía web está pendiente (PEND-07).

## Stack (cuando toque código)

Next.js App Router en Vercel. La fase 1 no tiene backend: el contacto es un enlace `wa.me` con el mensaje prellenado. Supabase y Google OAuth (solo para el panel de Julio) llegan en la fase de reservas. NestJS está descartado.

## Lo que no se hace

Claude Code no edita `knowledge-graph.json`, `estado-actual.md`, `siguiente.md` ni `revisiones-pendientes.md`. Propone los cambios en `ai/handoff/reporte.md` y el consultor decide.

> Copia de trabajo. Para que Claude Code la cargue sola, cópiala a `.claude/skills/visita-chiapas-con-julio/SKILL.md`.
