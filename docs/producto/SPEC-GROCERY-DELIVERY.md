# SPEC maestro: Grocery Delivery

**Producto transversal y obligatorio del libro** *Ruta Maestra de Aprendizaje de React Native: de fundamentos a arquitecto y desarrollador experto*.

**Estado:** especificación inicial; código de la aplicación aún no implementado. **Alcance:** 56 capítulos, siete proyectos incrementales.

## Objetivo del producto
Construir una aplicación comercial de compra de alimentos y entrega a domicilio, de principio a fin, con diseño móvil fiel al material de referencia suministrado por el autor. La teoría avanza de JavaScript y TypeScript a arquitectura, seguridad, nativo, testing y producción; **cada ejercicio práctico deberá aportar conocimiento o código reutilizable para este producto**.

**Referencia pública:** https://spanish.alibaba.com/product-detail/La-Mejor-Aplicaci%C3%B3n-M%C3%B3vil-para-Entrega-10000042110930.html

## Experiencias y módulos
### Cliente (React Native Android/iOS)
- Inicio, onboarding, dirección y zona de entrega, autenticación.
- Home y catálogo visualmente fieles a la referencia; banners, categorías, búsqueda, filtros y destacados.
- Ficha de producto, disponibilidad, unidades, favoritos y carrito persistente.
- Checkout: dirección, costos calculados en servidor, promociones y pasarela de pagos en entorno apropiado.
- Pedidos, historial, seguimiento, notificaciones y soporte.
- Estados offline, carga, error, permisos y accesibilidad.

### Repartidor
- Identificación y permisos, disponibilidad, asignación de entregas.
- Detalle, ruta, estados válidos de entrega, incidencias y confirmación.
- Políticas de ubicación, privacidad y auditoría.

### Administración/operaciones
- Gestión de catálogo, categorías, fotos, precios y promociones.
- Inventario, reservas y stock transaccional, zonas y tarifas.
- Pedidos, pagos, repartidores y métricas; roles y auditoría.

### Backend de referencia
- API REST, datos transaccionales y contratos tipados.
- Autoridad del servidor en precio, promociones, stock, pago, pedidos y permisos.
- Reintentos e idempotencia en creación de pedidos y webhook de pagos.
- Migraciones, seed de demo identificado, pruebas y documentación OpenAPI.
- Tecnología elegida mediante ADR (.NET o Laravel) y no por suposición.

## Reglas de arquitectura
React Native + TypeScript estricto + Expo; aprendizaje gradual de capacidades nativas. Feature-First y composición. Dominio, aplicación e infraestructura con dependencias invertidas cuando aporten valor, sin capas decorativas. Estado de interfaz separado del servidor, sincronización local/offline cuando corresponda. Seguridad, accesibilidad y testabilidad desde el inicio.

## Diseño
Se persigue máxima fidelidad a la imagen de referencia en las pantallas visibles; diseño original y coherente en pantallas no mostradas. La imagen aportada inicialmente es una composición publicitaria de baja legibilidad, **pero el autor confirma que la ficha de Alibaba contiene otras imágenes del producto**. Antes de suponer que faltan pantallas, debemos examinar la galería original y catalogar sus capturas. Su acceso automatizado fue bloqueado por la página de verificación de Alibaba el 10 de octubre de 2026; no se afirma haberla inspeccionado íntegramente. La paridad visual deberá verificarse con las capturas efectivamente disponibles, sus dimensiones y recursos debidamente autorizados. Ver [referencia visual](../diseno/REFERENCIA-VISUAL.md).

## Definition of Done del producto
1. Cliente navega catálogo real, agrega al carrito, introduce dirección, completa un checkout validado y consulta pedidos.
2. Operación administra existencias, catálogo y pedidos con roles y trazabilidad.
3. Repartidor procesa una entrega con estados válidos y evidencia cuando corresponda.
4. Backend evita inconsistencias de dinero, stock, pagos y concurrencia.
5. Android/iOS tienen manejo de errores, accesibilidad básica, seguridad y tolerancia a conectividad variable.
6. Pruebas unitarias, de integración, E2E y revisión visual; builds reproducibles y documentación operativa.
7. Ningún material de terceros se redistribuye sin los derechos adecuados.

## Gobernanza
- El manuscrito completo y tablero de tareas se mantienen en el Drive privado del autor.
- GitHub público conserva código propio, documentación pública, ejercicios y pruebas.
- Todo avance debe tener evidencia (commit/PR, test, captura o documento).
- No confundir demo con servicio productivo: proveedores de pagos, mapas, push y publicación exigen cuentas, condiciones, costes y aprobaciones externas.
