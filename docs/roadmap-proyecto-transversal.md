# Roadmap transversal: una aplicación a través de siete partes

Todo ejercicio del libro debe referirse a **Grocery Delivery** y tener sentido dentro del producto final.

| Parte | Capítulos | Proyecto | Resultado acumulativo |
|---|---|---|---|
| I | 1–8 | Dominio TypeScript | Productos, Money, carrito, precios y pruebas puras |
| II | 9–16 | UI de cliente | Home fiel a referencia, categorías, catálogo, detalle, carrito |
| III | 17–24 | Integración real | Auth, API, direcciones, persistencia, checkout verificado |
| IV | 25–32 | Arquitectura profesional | Feature-First, casos de uso, repositorios y tests |
| V | 33–40 | Comercio y reparto avanzado | Offline-first, seguimiento, repartidores, notificaciones, pagos |
| VI | 41–48 | Calidad y despliegue | E2E, rendimiento, fidelidad visual, observabilidad, builds |
| VII | 49–56 | Producto completo | Cliente, repartidor, administración, backend, auditoría y documentación |

## Plan de crecimiento del repositorio
- Inicio: `ejemplos/`, `ejercicios/`, `proyectos/` y documentación.
- UI inicial: código Expo/React Native cuando llegue el capítulo 9.
- Catálogo incremental de UI: tokens y componentes genéricos primero; composiciones de comercio dentro de sus features. Cada componente debe tener ficha, demo, pruebas y trazabilidad; documentación en [catálogo](design-system/CATALOGO.md).
- Integración: backend y módulos compartidos cuando los contratos lo requieran.
- Final: arquitectura modular reproducible, con apps cliente/repartidor/admin y API **solo si** el diseño aprobado realmente necesita repositorios o paquetes separados.

### Hitos de cada capítulo
1. Investigación y estructura de ocho subapartados.
2. Redacción y explicación.
3. Diagramas y figuras.
4. Ejercicios con implementaciones y pruebas conectados a Grocery Delivery.
5. Revisión final, evidencia y aprobación.

## Ocho mejoras aprobadas de roadmap.sh (índice congelado, 2026-10-10)

Estas son las **únicas ocho incorporaciones** autorizadas antes de redactar el libro. Se aplican al contenido y a las prácticas de **Grocery Delivery**, sin agregar capítulos, partes, tecnologías obligatorias ni proyectos paralelos.

| Ref. | Capítulos | Laboratorio práctico verificable |
|---|---|---|
| P0-01 | 9 y 41 | Ejecutar Grocery Delivery en Android; utilizar menú de desarrollo, Fast Refresh, LogBox y React Native DevTools para diagnosticar un error controlado. |
| P0-02 | 11–12 | Implementar formulario de dirección y checkout con safe areas actuales, teclado y diseño edge-to-edge; verificar que ningún control queda oculto. |
| P0-03 | 11, 15 y 19 | Actualizar listado de productos con RefreshControl, loading, empty y error; comprobar deduplicación y manejo de cancelación. |
| P0-04 | 11–13 y 24 | Resolver una diferencia real Android/iOS con Platform.select y, cuando proceda, .android/.ios/.native; justificar por qué no duplicamos pantallas. |
| P0-05 | 11–15 | Construir preferencia con Switch, elementos de imagen apropiados y listas con estados; documentar sustitutos para APIs deprecadas. |
| P0-06 | 9–10, 50 y 54 | Mantener matriz comprobada de compatibilidad de Expo SDK, React Native, React, Node, Hermes, Metro y dependencias nativas, con versiones fijadas. |
| P0-07 | 11–16 | Crear galería de desarrollo para AppText, AppButton, ProductCard y otros componentes conforme surjan; documentar estados, variantes, accesibilidad y tests. |
| P0-08 | 7–8 y 31–32 | Comparar una ProductCard sobreacoplada con una solución por composición, hooks y casos de uso; documentar separación de responsabilidades y compromisos. |

**Gates:** cada laboratorio debe enlazar capítulo, código real, ejecución, pruebas y evidencia. Se implementarán cuando lleguemos a sus capítulos; aquí solo se planifican.

**Decisión de alcance:** las siete partes, los 56 capítulos y el producto Grocery Delivery quedan congelados. No sumar nuevas propuestas de la auditoría sin aprobación expresa posterior del autor.

**Auditoría de origen:** [05 · Comparación roadmap.sh](https://docs.google.com/document/d/1yZvqgJYXbT4UtUmh_TZm8Lmr5abSYiht7uKFEOVM14g/edit).

## Puertas de salida de cada parte
Cada fase debe producir un estado ejecutable, con criterios de aceptación y pruebas. No marcar «completado» por haber creado carpetas, mockups estáticos, páginas vacías o endpoints que devuelvan datos inventados.
