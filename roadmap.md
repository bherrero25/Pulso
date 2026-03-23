# 🧭 Pulso — Roadmap de Producto

## Visión
App de finanzas personales para mujeres de 45-55 años que gestionan la economía familiar.
Sin acceso al banco, sin publicidad, sin vender datos. Suscripción ~6€/mes.

---

## Versión actual — v1 (en uso)
Estado: ✅ En producción y uso diario
URL: bherrero25.github.io/Pulso
Stack: HTML single-file · GitHub Pages · Supabase

### Lo que tiene
- Transacciones con categorías, cuentas y filtros
- Importación CSV (Airtable + Bankinter XLSX/XLS)
- Inversiones con semáforos de rentabilidad y TIR
- Tesorería con flujos de caja
- Ahorro y gastos extraordinarios con cuotas mensuales
- Patrimonio (activos y pasivos)
- Seguros con alertas a 75 días y semáforos 🔴🟢
- Agenda con eventos, pagos, citas y hora
- Análisis con calculadora de fondos corregida
- Resumen PDF mensual con todas las transacciones
- Backup/restauración JSON completo
- Tooltips CSS en botones de cabecera
- Bloqueo con PIN
- Multi-tema (Clásico, Noche, Turquesa, Pastel, Grafito)
- PWA instalable

### Limitaciones conocidas (v1)
- Hardcodeada para un único usuario (betsabe en Supabase)
- Algunas pestañas muy personalizadas (Bonus, hijos por universidad)
- Entrada de datos manual o via CSV — no voz

---

## Versión 2 — v2 (próxima)
Estado: 🗓 Planificada
Objetivo: validar que el nuevo sistema de entrada de datos da los mismos resultados que v1

### Nuevas funcionalidades
- **Importación CSV del banco** — subir extracto directamente, sin pasar por Airtable
- **Gastos en efectivo por voz** — botón 🎤, el navegador transcribe, reglas simples extraen importe y descripción
- **Multi-usuario** — construir desde el principio con Supabase Auth (registro + login)

### Plan de validación
- Mantener v1 (Airtable + manual) en paralelo durante varios meses
- Comparar que los números cuadran entre v1 y v2
- Cuando cuadren durante 2-3 meses seguidos → migración definitiva a v2

---

## Versión comercial — vPRO
Estado: 💡 En definición
Objetivo: producto vendible a otras usuarias

### Diferencias respecto a v1 personal
- ❌ Pestaña Bonus anual → reemplazar por "Ingresos extraordinarios" configurable
- ❌ Hijos hardcodeados → "Personas a cargo" que cada usuaria define
- ❌ Categorías fijas → lista estándar editable por la usuaria
- ✅ Todo el motor financiero (cálculos, gráficos, importación) se reutiliza

### Lo que necesita además
- **Landing page** — explica qué es, para quién, precio y botón "Probar demo"
- **App de demo** — datos ficticios realistas (mujer 48 años, 2 hijos, hipoteca, fondos, seguros...)
  - Usuario fijo: demo@pulso.app / demo1234
  - Reset automático de datos cada noche
- **Onboarding** — que una usuaria nueva entienda cómo funciona sola
- **Stripe** — pagos y gestión de suscripciones
- **Versión móvil pulida** — ya es PWA, revisar experiencia en iPhone
- **Soporte** — canal de contacto (email o chat)

### Plan de lanzamiento
1. Terminar y estabilizar v2
2. Probar con 3-5 personas del perfil objetivo (sin cobrar)
3. Recoger feedback y ajustar
4. Con 10-20 usuarias satisfechas → abrir suscripción de pago
5. No se necesita inversión ni equipo — stack actual es suficiente

---

## Decisiones de producto tomadas
- Precio objetivo: ~6€/mes
- Sin acceso al banco (diferenciador clave frente a competencia)
- Sin publicidad, sin venta de datos
- Entrada por voz: empezar con reglas simples (gratis), añadir IA si hace falta
- La v2 se construye ya con multi-usuario desde el principio

---

## Notas técnicas
- Stack actual: HTML single-file · Supabase (thzurasttoyqphepvhlc) · GitHub Pages
- Para vPRO migrar a Lovable + Supabase Auth + Stripe
- Demo con datos ficticios: generar 12 meses de transacciones realistas

---

*Última actualización: marzo 2026*

---

## Línea de producto — Pulso Joven
Estado: 💡 En definición
Objetivo: app de finanzas para jóvenes de 18-28 años, simple y visual

### Perfil de usuaria/o
- 20-25 años, estudiante o primer empleo
- Pregunta clave: "¿llego a fin de mes?" y "¿cuándo puedo irme de viaje?"
- Usa el móvil para todo, espera diseño moderno y rápido
- Puede tener primeras inversiones (fondos indexados)

### Pestañas previstas
- **Inicio** — semáforo del mes, saldo actual, próxima meta de ahorro
- **Gastos e ingresos** — categorías visuales con emoji, simple
- **Presupuesto** — límite por categoría (ocio, comida, transporte...)
- **Viajes** — meta de ahorro con cuenta atrás y barra de progreso
- **Metas** — ahorro para coche, piso, gadget, experiencias...
- **Inversiones** — opcional, para quienes empiezan con fondos indexados

### Lo que NO tendría
- Seguros, leasing, bonus anual, hipoteca, hijos, patrimonio complejo

### Diferencias de producto
- Diseño diferente al Pulso adulto — más colorido, mobile-first, moderno
- Precio menor o freemium — 3€/mes o gratis con límite de transacciones
- Posiblemente marca diferente (no necesariamente "Pulso Juvenil")

### Pendiente de definir
- Nombre de marca
- Pestañas definitivas — darle una vuelta en profundidad
- Si comparte base de código con Pulso adulto o es independiente
- Modelo de precio exacto

