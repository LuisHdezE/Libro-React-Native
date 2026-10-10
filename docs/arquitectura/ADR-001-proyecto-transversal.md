# ADR-001 · Grocery Delivery como producto transversal

**Fecha:** 2026-10-10
**Estado:** Aceptado para el enfoque pedagógico; decisiones tecnológicas específicas aún pendientes.

## Contexto
La primera versión editorial del libro contemplaba proyectos independientes (tareas, inventario, etc.). El autor ha definido una aplicación de supermercado/entregas de referencia como producto final que deberá quedar completo y público en GitHub.

## Decisión
Mantener los 56 capítulos y sus fundamentos, pero orientar todos los ejercicios hacia piezas reutilizables del producto Grocery Delivery. Reorganizar los siete proyectos como entregas acumulativas del mismo producto, para obtener Android/iOS, backend, operaciones, repartidor, pruebas, documentación y release.

El objetivo de diseño es reproducir con fidelidad la UI de cliente mostrada; las pantallas no disponibles son diseñadas de forma coherente y validada.

## Consecuencias
- Mayor continuidad didáctica, contratos y regresión acumulativa.
- Incrementa el alcance final frente a una app de demostración sencilla.
- Requiere distinguir entregables realmente operativos de pantallas y mocks.
- El backend y el panel administrativo requieren documentación y QA adicionales.
- Se aplicarán etapas, quality gates y arquitectura proporcional para no sobreingenierizar capítulos tempranos.
- La selección de backend (.NET o Laravel), despliegue y módulos móviles nativos se decidirá con ADR posteriores.
- La reproducción «tal cual» queda condicionada a disponer de material legible y derechos para activos visuales de terceros.
