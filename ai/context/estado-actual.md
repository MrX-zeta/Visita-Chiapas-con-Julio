# Visita Chiapas con Julio — Estado actual

Actualizado: 28 de octubre de 2026 · Grafo v1.0.0

> Este documento resume el estado más reciente del proyecto. El detalle y los valores exactos viven en `ai/context/knowledge-graph.json` (fuente de verdad, DEC-30). `docs/estado del proyecto.md` (agosto) queda como histórico: su flota y su modelo de cobro están desactualizados (INC-05).

---

## 1. Fase actual

| Fase | Estado |
|---|---|
| FASE-0 · Contexto, grafo y handoff | En curso (este documento) |
| FASE-1 · Identidad visual | Siguiente. Bloqueada por PEND-06, 07 y 08 |
| FASE-2 · Sitio de una página | Bloqueada por datos de Julio |
| FASE-3 · Perfil de Empresa en Google | En paralelo; Julio dice que «recién se registró» (PEND-15) |
| FASE-4 · Sistema de reservas | No iniciada; solo si el volumen lo justifica |

## 2. El negocio en una página

- **Qué es:** transporte terrestre privado con operador. Se renta la unidad completa, nunca se comparte con desconocidos (POL-01). Base en San Cristóbal, 16 años operando.
- **Flota:** 4 unidades, 4 operadores. Coche (2–4), van chica (4–7), van mediana (8–11, la tabla de precios dice 14) y van grande (12–20). Modelos sin confirmar (INC-01, INC-02).
- **Servicios:** tours de un día, traslados (aeropuerto de Tuxtla), paquetes de varios días y viajes a la medida.
- **Tours:** Sumidero (6 h, 9:00, el más vendido) · Palenque con Agua Azul y Misol-Ha (2 días, 5:00, el que más deja) · Montebello (14 h, 7:00) · Chamula y Zinacantán (4 h, 10:00) · Arcotete y Rancho Nuevo (4 h, 10:00).
- **Paquetes:** Básico (los 5 tours, una noche en Palenque, penúltimo día libre) y Chiapas Total (más Las Nubes, Las Guacamayas, Yaxchilán y Bonampak, en cabañas). Tarifas por unidad en TAR-01 y TAR-02.
- **Reglas que dan confianza:** recoge y deja en el hospedaje; anticipo del 50% o de palabra; acepta efectivo si el cliente desconfía de transferir; devuelve íntegro el anticipo por fallecimiento o enfermedad; itinerario flexible.
- **Clientes:** sobre todo nacionales, familias y parejas, por recomendación. Unas 2 solicitudes por semana y 7 de cada 8 se cierran. Las que no, suelen ser por presupuesto.
- **Lo que quiere Julio del sitio:** que quien ya lo contactó lo vea formal, seguro y conocido (DEC-22).

## 3. Identidad visual: lo que ya está

- Logo elegido: cordillera azul de trazo continuo y ruta punteada terracota (DEC-13).
- Paleta: `#334351` azul tinta · `#FBF3E6` crema · `#BE6A47` terracota (DEC-14).
- Monocromo como variante obligatoria y favicon solo con la montaña (DEC-15, DEC-16).
- Archivos en la carpeta: `logo/Visita Chiapas con Julio.png` (raster) y `logo/identidad-visual/referencias/` (`logov1.svg`, `simbolo.svg`, `punteada.svg`, calcados del PNG).
- `brief.md` y `reporte.md` de identidad-visual existen pero están vacíos.

### Hallazgos de la revisión
1. El vector está calcado: la montaña tiene grosor irregular y los trazos de la ruta son disparejos. Se propone redibujarlo limpio (DEC-28, depende de PEND-06).
2. La terracota da 3.57:1 sobre crema, así que no sirve para texto normal. Se propone `#A65A3B` para texto y botones (4.6:1 sobre crema, blanco encima 5.06:1) (DEC-27).
3. Faltan paleta extendida, tipografía web, dirección fotográfica, tono de voz y aplicaciones. El vinil de las unidades es urgente porque sirve como prueba para la verificación de Google (DEC-21).
4. Los archivos que el documento de agosto da por entregados (`Logo.tsx`, `logo-completo.svg`, `logo-simbolo.svg`, `comparativa-logo.png`, `logo-monocromatico-azul.png`, prompts y cuestionario) **no están en la carpeta del proyecto** (INC-05).

## 4. Datos que no cuadran (preguntar a Julio)

| Id | Tema |
|---|---|
| INC-01 | «4 vans» frente a coche más 3 vans; «22 y 24» ¿son años-modelo? |
| INC-02 | La van mediana es para 11 pasajeros, pero la tabla de precios llega a 14 |
| INC-03 | ¿Cobra por persona o por viaje? ¿Qué pasa entre el mínimo y el máximo de la tabla? |
| INC-04 | Dice «sin cupo mínimo», pero cada unidad tiene un mínimo |
| INC-06 | Palenque: 5 h de camino frente a 11 h |
| INC-07 | ¿La lancha del Sumidero va incluida en «entradas»? |

## 5. Pendientes que bloquean

**Identidad (FASE-1):** PEND-06 (redibujar el logo) · PEND-07 (tipografía web) · PEND-08 (formato del manual).
**Sitio (FASE-2):** PEND-01 (días por paquete) · PEND-02 (precio base de tours sueltos y traslados) · PEND-03 (WhatsApp y correo definitivos) · PEND-04 (modelos de las unidades) · PEND-05 (constancias de credenciales) · PEND-14 (fotos clave) · PEND-16 (voz en primera persona o «nosotros»).
**Otros:** PEND-09 (costos y mantenimiento, después de la cotización) · PEND-10 (permiso de imagen por escrito) · PEND-11 (hospedaje) · PEND-12 (facturación) · PEND-13 (dominio) · PEND-15 (Perfil de Google) · PEND-17 (plantillas originales del handoff).

## 6. Siguiente paso

1. Resolver PEND-06, 07 y 08 con el responsable.
2. Liberar TAREA-01 en `ai/handoff/siguiente.md` (limpieza vectorial del logo, variantes y tokens).
3. Llevar a Julio la lista de INC y PEND de la sección 4 en la siguiente visita, junto con la petición de fotos.

## 7. Bitácora

| Fecha | Cambio |
|---|---|
| 2026-08-27 | Documento de estado inicial (`docs/estado del proyecto.md`) |
| 2026-10-28 | Entrevista completa integrada. Se crean grafo v1.0.0, estado actual, skill del proyecto y carpeta de handoff |
