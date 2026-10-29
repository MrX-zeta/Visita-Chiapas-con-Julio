# Visita Chiapas con Julio — Estado del proyecto
Actualizado: 27 de agosto de 2026

---

## 1. DATOS CONFIRMADOS POR JULIO

| Dato | Valor |
|---|---|
| Nombre comercial | **Visita Chiapas con Julio** (definitivo) |
| Titular | Julio César Hernández Mijangos |
| Años operando | ~16 |
| Base | San Cristóbal de las Casas (lada 967) |
| Equipo | 2 choferes además de él |
| Unidades | 2 camionetas *(el modelo NO lo confirmó; "Urvan" viene de Facebook)* |
| Sitio web previo | Ninguno |
| Dominio | No tiene |
| Reseñas escritas | **Ninguna**, en ningún lado |
| Perfil de Empresa en Google | No tiene |
| Sistema de reservas | Sí le interesa, con el alcance mínimo acordado |
| Quién actualiza precios y fotos | Tú. Julio manda mensaje, tú publicas |
| Logotipo | Elegido (ver sección 3) |

**Contacto público actual** (de su Facebook, falta que lo confirme):
WhatsApp 967 122 7321 · juliomijangos29@hotmail.com

**Presencia digital:** Facebook (362 seguidores, la portada dice "Descubre Chiapas con Julio" y hay que corregirlo), Instagram y WhatsApp ya usan "Visita Chiapas con Julio". El hotmail está ligado a sus redes y **no se toca**.

---

## 2. DECISIONES TOMADAS ENTRE TÚ Y YO

**Producto**
- Fase 1: sitio de una página, en español, sin backend
- El formulario no manda correo: arma un enlace `wa.me` con el mensaje ya redactado
- Bilingüe: se deja la estructura de rutas lista, se traduce después
- Sistema de reservas: fase aparte, solo si el volumen lo justifica
- Sin testimonios hasta que existan reseñas reales
- Módulo de administración de fotos: fuera del MVP

**Alcance del sistema de reservas (cuando toque)**
Solicitud con todos los campos · calendario por unidad *(lo más importante: evitar comprometer la misma camioneta dos veces)* · estados de reserva · registro de pagos en efectivo · funcional desde el celular.
Fuera: pagos en línea, cuentas de cliente, disponibilidad en tiempo real.

**Stack**
Next.js con App Router · Vercel · Supabase (Postgres) · Google OAuth solo para el panel de Julio, nunca para el turista · Mercado Pago a futuro.
**Nest.js descartado:** con Supabase encima sobra, y encaja mal en serverless. Route Handlers de Next.

**Contenido**
- Precios y destinos viven en **un solo archivo de datos**, no regados en el maquetado
- Precios como "desde $X", no exactos, para reducir actualizaciones
- Ventana fija de cambios (ej. los lunes), no disponibilidad permanente
- 10 a 12 fotos, se revisan por temporada. Acordar cuántas entran por revisión
- Proporciones fijas en CSS con `aspect-ratio` y `object-fit: cover`, para que una foto vertical no rompa el diseño
- Fotos: carpeta de Drive para el lote inicial, WhatsApp para lo suelto

**Acuerdos comerciales pendientes de hablar con él**
- Dominio a nombre de Julio, aunque tú lo administres
- Costos recurrentes: dominio anual, hosting y base de datos mensual *(se lo explicas en persona)*
- Mantenimiento: cuántos cambios entran, cada cuándo, y desde cuándo se cobra
- Sugerencia de dominio: `chiapasconjulio.com` (más corto y dictable que el nombre completo)

---

## 3. IDENTIDAD VISUAL

**Logotipo elegido:** base de la propuesta 1 (cordillera de trazo continuo + ruta punteada), con la montaña y el texto en azul y la ruta en terracota.

| Elemento | Valor |
|---|---|
| Tipografía | Garet |
| Azul (tinta) | `#334351` |
| Crema (fondo) | `#FBF3E6` |
| Terracota (acento) | `#BE6A47` |

**Por qué la ruta va en terracota y no en azul:** es el único elemento cálido y es el que marca el recorrido visual. Todo azul se ve más frío y más genérico. La versión monocromática existe como variante obligatoria (sellos, vinil de un tinte, blanco y negro), **no como alternativa a elegir**.

**Favicon:** solo la montaña, sin ruta ni texto. A 16px lo demás desaparece.

**Nota técnica:** el logotipo de Canva es una imagen rasterizada, no vector. No se puede recolorear ni escalar. Ya está vectorizado en `logo-completo.svg`, `logo-simbolo.svg` y el componente `Logo.tsx`. El texto quedó trazado como contornos, así que **no hace falta licenciar Garet para el sitio**. Para los títulos del sitio sí hay que usar una alternativa gratuita: Poppins, Outfit o Jost.

**Enlaces de Canva** (el primero es editar, el segundo compartir):
- Tres propuestas + avatares — `jEH0Ot4CAaHhbit` / `qDYvmcx9KbZL6YN`
- Logotipo con frase completa — `jXnvhzLSF14ghzq` / `1kgGUQq7uf0xhot`
- Logotipo final, copia limpia — `pqiiuzkDBHXux9g` / `ozYh6fzSgMtnLVd`
- Favicon 1 — `Fjn29Wg9iC-jkLt` / `vlXjddt-izFZORZ`
- Favicon 2 — `MK__WoAora0-sj3` / `7EfXv3RyHzsSmjW`
- Favicon 3 — `9O8R_bOWygrlu-l` / `7X7HEXQTaSuU3B2`

Van completos como `https://www.canva.com/d/CODIGO`. **A Julio mándale siempre el segundo**, el de compartir.

---

## 4. PLAN DE ACCIÓN: PERFIL DE EMPRESA EN GOOGLE

Esto vale más que el sitio web para traer clientes nuevos, y es gratis. Lo hace **Julio, contigo al lado**: la cuenta debe ser suya y el video lo tiene que grabar quien opera el negocio.

**Antes de empezar, ten listo:** la cuenta de Google del negocio, el nombre exacto, el teléfono que sí contesta, el horario real y la lista de destinos.

**Paso 1 — Crear la ficha.** En `business.google.com`, buscar primero si ya existe una ficha del negocio; si aparece, se reclama en vez de crear otra. Si no, se crea con el nombre **exacto**: "Visita Chiapas con Julio". Nada de meterle palabras clave tipo "transporte barato Palenque" — Google suspende perfiles por eso.

**Paso 2 — Marcarlo como negocio de área de servicio.** Cuando pregunte si los clientes pueden visitarlo en una dirección, la respuesta es **No**. En lugar de dirección se define la zona donde trabaja. Esto hay que dejarlo bien configurado *antes* de pedir la verificación.

**Paso 3 — Categoría.** Es de las decisiones que más pesan para aparecer en el mapa. Principal: servicio de transporte o agencia de viajes, según lo que confirme del modelo de negocio. Se pueden agregar secundarias.

**Paso 4 — La verificación, que es donde se atora la gente.** El método lo asigna Google, no se elige, y hoy casi siempre es por video. Requisitos: grabación única, sin cortes ni ediciones, mínimo 30 segundos, grabada y subida desde el celular dentro del perfil. No se puede grabar antes y subir después.

Para un negocio sin local, el video debe mostrar **prueba de que el negocio existe y de que él lo administra**: la camioneta con el rótulo del negocio, documentos a nombre de la empresa, o el espacio desde donde trabaja.

> **Consecuencia práctica:** el vinil con el logo en la camioneta deja de ser decoración y se vuelve requisito. Y por eso importa la pregunta del RFC: un documento a nombre del negocio sirve como prueba.

**Paso 5 — Llenar el perfil.** Teléfono que de verdad contesta, horario real, descripción, servicios por destino, y fotos. Aquí se reusan las mismas fotos del sitio.

**Paso 6 — Reseñas.** Una vez verificado, sale el enlace directo para pedirlas. Que empiece **al bajar a la gente del carro**, no después por mensaje. Una sola vez, sin insistir.

Cuenta con que la revisión puede tardar días. Empezar hoy es lo que hace que para el lanzamiento del sitio ya haya reseñas.

---

## 5. LO QUE BLOQUEA EL DISEÑO

- [ ] **Modelo de negocio:** ¿unidad privada completa o lugares compartidos? ¿Cobra por viaje o por persona?
- [ ] Capacidad y modelo de las camionetas
- [ ] Lista de destinos con duración, punto de salida y precio
- [ ] WhatsApp y correo definitivos, verificados con un mensaje de prueba
- [ ] Mínimo 10 fotos, incluyendo las 5 que no tiene: él, la camioneta por fuera, el interior, gente disfrutando, y un paisaje horizontal
- [ ] Permiso de uso de imagen por escrito
- [ ] Cuenta de Google del negocio creada
- [ ] Costos y mantenimiento hablados

---

## 6. ARCHIVOS ENTREGADOS

`Logo.tsx` · `logo-completo.svg` · `logo-simbolo.svg` · `comparativa-logo.png` · `logo-monocromatico-azul.png` · `glosario-vibecoding.md` · `plantilla-prompt-sitios-web.md` · `prompt-fase1-julio.md` · `cuestionario-julio-v2.md`

**Nota sobre el prompt de la Fase 1:** se escribió cuando creíamos que el servicio era un sedán con chofer. Hay que actualizarlo con lo que salga del Bloque 2 — capacidad en las tarjetas, precio por viaje en vez de por persona, y probablemente una sección para grupos grandes.