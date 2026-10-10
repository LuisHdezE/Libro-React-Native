# Catálogo vivo de componentes React Native

Este catálogo forma parte del libro **Ruta Maestra de Aprendizaje de React Native** y crece de forma gradual con sus ejemplos. El proyecto que valida los componentes es **Grocery Delivery**.

**Estado:** inventario y criterios editoriales definidos. **No hay implementaciones React Native ni galería ejecutable creadas todavía.**

## Arquitectura y límites

1. **Tokens semánticos**: colores, tipografía, espaciados, radios, iconografía y temas. Los valores se medirán con las imágenes originales de referencia disponibles, sin inventar paridad visual.
2. **Componentes genéricos**: no importan entidades del negocio, repositorios, navegación de la app ni llamadas HTTP. API de props TypeScript estricta y composición. Reutilizables fuera del supermercado.
3. **Componentes por feature**: `ProductCard`, `CartSummary` y similares residen en las funcionalidades, consumen datos de presentación y callbacks, y componen los anteriores. No determinan precios finales, pagos, existencias o reglas de pedido.

La meta no es hacer Atomic Design por obligación ni construir una gran librería antes de necesitarla: abstraeremos lo que pueda mantenerse y reutilizarse.

## Inventario previsto, no implementado

| Categoría | Componentes iniciales |
|---|---|
| Fundamentos UI (12) | `AppText`, `AppIcon`, `AppButton`, `IconButton`, `AppTextField`, `SearchField`, `AppSurface`, `AppCard`, `AppBadge`, `AppChip`, `SectionHeader`, `AppProductImage` |
| Feedback (6) | `LoadingIndicator`, `Skeleton`, `EmptyState`, `ErrorState`, `InlineMessage`, `ConfirmDialog` |
| Navegación (2) | `AppHeader`, `BottomTabsPresentation` |
| Comercio (10) | `CategoryTile`, `ProductCard`, `PromoBanner`, `QuantityStepper`, `PriceLabel`, `CartItemRow`, `CartSummary`, `DeliveryAddressTile`, `ProductGrid`, `CheckoutSummary` |

Los 30 componentes se ampliarán o consolidarán cuando el proyecto evidencie nuevas necesidades. Componentes de comercio se ubicarán en sus respectivas features; solo se promoverán a componentes compartidos si lo justifica una reutilización real.

## Ficha obligatoria por componente

Cada componente aprobado requiere:

- Identidad, problema resuelto, capítulo de origen y reutilizaciones.
- Contrato de props TypeScript y ejemplos correctos/incorrectos.
- Estados y variantes **pertinentes**: disabled, loading, error, selected, etc.
- Demo visual ejecutable y capturas cuando su apariencia sea crítica.
- Accesibilidad: labels, roles, foco, targets táctiles, texto escalable, contraste.
- Tema, diseño adaptable y particularidades Android/iOS cuando correspondan.
- Pruebas de comportamiento y documentación de decisiones de API.
- Ruta real de código, commit/PR, vínculo con tarea y revisión final.

No declarar un componente terminado por registrar su nombre aquí.

## Galería visual

Se implementará **cuando estudiemos React Native y componentes** (capítulos 9 a 12): galería de desarrollo accesible desde un entorno no productivo. Se evaluará Storybook para React Native frente a galería Expo interna según compatibilidad, esfuerzo y valor didáctico. No se integrará automáticamente una dependencia sin validar.

La galería deberá permitir previsualizar variantes, estados, safe areas, tema y escala de texto. Se documentarán capturas comparativas con referencia y estados disponibles. No distribuir la galería de laboratorio en builds de producción sin aprobación.

## Progresión y control

- **Cap. 1–8**: dominio TypeScript y modelos de datos, sin componentes móviles ficticios.
- **Cap. 9–16**: tokens, primitives, ProductCard, CategoryTile, PromoBanner y Home.
- **Cap. 17–24**: estados remotos, formularios, carrito y checkout.
- **Cap. 25–32**: refactorización arquitectónica y contrato de componentes.
- **Cap. 33–40**: integración, resiliencia y adaptación.
- **Cap. 41–48**: pruebas visuales/E2E, accesibilidad, rendimiento, CI/CD.
- **Cap. 49–56**: consolidación, APIs avanzadas y extracción cuando corresponda.

**Fuente de verdad de tareas:** Google Sheets (pestañas *Tareas*, *Catálogo UI* y *Resumen*).

Especificación editorial privada: [04 · Catálogo maestro de componentes](https://docs.google.com/document/d/1RAoHxeMJMTHgIAzc5LwLiX7Ffj7irXAhomUdmu95Z_s/edit). La documentación técnica, ejemplos y código aprobados sí se publicarán aquí.
