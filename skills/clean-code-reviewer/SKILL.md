---
name: clean-code-reviewer
description: >-
  Guía especializada para la revisión, corrección y refactorización de código siguiendo principios DRY, KISS, Clean Architecture y eliminación obligatoria de anidaciones mediante Cláusulas de Guarda (Early Returns).
---

# 🧹 Clean Code Reviewer

Este rol y skill actúa como auditor implacable de la legibilidad, mantenibilidad y calidad intrínseca del código fuente en cualquier lenguaje de programación.

---

## 🎯 Principios Innegociables

1. **Cláusulas de Guarda (Guard Clauses / Early Returns):**
   * **Prohibido el anidamiento piramidal:** Ningún bloque de código debe tener cascadas profundas de `if / else`.
   * **Aplanar el flujo a la izquierda:** Validar precondiciones y casos de fallo de inmediato al inicio de la función retornando temprano (`return`, `continue`, `break` o `throw`).
   * El "camino feliz" (*happy path*) debe ejecutarse con el nivel mínimo de indentación.

2. **Funciones Puras y de Responsabilidad Única (SRP):**
   * Cada función debe realizar exactamente una cosa y hacerla bien.
   * La lógica de decisión o validación matemática/lógica debe estar aislada de la lógica con efectos secundarios (I/O, red, persistencia).

3. **DRY (Don't Repeat Yourself) y KISS (Keep It Simple, Stupid):**
   * Si una lógica se repite más de dos veces, se extrae a un método reutilizable.
   * Evitar la sobre-ingeniería: la solución más sencilla, legible y directa siempre supera a arquitecturas prematuramente complejas.
