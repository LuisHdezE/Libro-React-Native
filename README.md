# Ruta Maestra de Aprendizaje de React Native
### De fundamentos a arquitecto y desarrollador experto

Este repositorio público recopilará **todos los ejemplos, ejercicios, pruebas y proyectos** del libro. Su columna vertebral será **Grocery Delivery**, una aplicación de supermercado y entregas que evolucionará desde los primeros ejemplos de TypeScript hasta un producto móvil de extremo a extremo.

> **Estado actual:** planificación, diseño objetivo y estructura de documentación definidos. La aplicación y sus ejemplos aún deben implementarse capítulo a capítulo.

## Referencia de diseño

El autor ha elegido como objetivo visual el póster de la aplicación de supermercado: https://spanish.alibaba.com/product-detail/La-Mejor-Aplicaci%C3%B3n-M%C3%B3vil-para-Entrega-10000042110930.html

Se reproducirán mediante **código propio** la jerarquía, composición, colores, componentes y pantallas mostradas, con aprobación visual progresiva. Las pantallas no mostradas se diseñarán coherentemente. No se redistribuirán fotografías, logotipos, creatividades ni código comercial de terceros sin derechos de uso.

## Siete entregas acumulativas

1. Dominio TypeScript: catálogo, precios, carrito, validaciones y tests.
2. App React Native: Home fiel a referencia, categorías, catálogo, fichas y carrito.
3. Backend real: API, auth, direcciones, stock, checkout y pedidos.
4. Arquitectura: Feature-First, dominio, casos de uso, adaptadores y pruebas.
5. Operación avanzada: offline-first, reparto, seguimiento, pagos y notificaciones.
6. Calidad: E2E, análisis de rendimiento, fidelidad visual, CI/CD y builds.
7. Producto completo: cliente, repartidor, administración, backend y documentación.

## Estructura vigente

| Carpeta | Contenido |
|---|---|
| [ejemplos/](ejemplos/) | Ejercicios de código por capítulo, todos enfocados en Grocery Delivery |
| [ejercicios/](ejercicios/) | Enunciados y soluciones |
| [proyectos/](proyectos/) | Implementaciones de las siete fases |
| [docs/producto/](docs/producto/) | Alcance, actores, reglas y criterios de aceptación |
| [docs/diseno/](docs/diseno/) | Objetivos de fidelidad con la referencia |
| [docs/arquitectura/](docs/arquitectura/) | Decisiones de arquitectura |
| [docs/design-system/CATALOGO.md](docs/design-system/CATALOGO.md) | Catálogo vivo de componentes, convenciones y criterios de aceptación |
| [docs/roadmap-proyecto-transversal.md](docs/roadmap-proyecto-transversal.md) | Correspondencia entre capítulos y fases |

La estructura final de aplicaciones y servicios aparecerá gradualmente, cuando exista código que la justifique.

## Principios de ingeniería

- React Native y TypeScript estrictos; comenzar con Expo.
- Composición, hooks y módulos Feature-First; Clean Architecture **cuando esté justificada**, no por plantilla.
- Separación entre lógica de dominio, integración de APIs, UI, persistencia y permisos.
- Backend como autoridad de precios, existencias, pagos y estados de pedidos.
- Pruebas, accesibilidad, seguridad, rendimiento y CI/CD.
- Publicación solo de código reproducible, con dependencias explícitas y sin credenciales.

**Nota:** un repositorio público no otorga automáticamente licencia para copiar recursos o código ajenos. La licencia de reutilización del código de este repositorio se establecerá antes de abrir contribuciones o distribución derivada.
