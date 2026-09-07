---
name: version-bump-guardian
description: >-
  Especialista en versionado semántico y trazabilidad de artefactos. Incrementa automáticamente la versión con cada cambio, mantiene el historial verificable y audita la presencia física de la nueva versión en el bundle generado antes de autorizar cualquier despliegue.
---

# 🏷️ Version Bump Guardian: Versionado Semántico y Garantía de Compilación

Esta skill garantiza que **ningún cambio se despliegue sin un incremento verificable de versión** y que **ningún build se publique sin certificar físicamente que el compilador procesó y estampó la nueva versión en los binarios generados**.

---

## 🎯 1. Principio Fundamental: Versionado Visible y Físicamente Comprobable

1. **Incremento con Cada Iteración:**
   * Cada modificación en código fuente (correcciones, nuevas funcionalidades, ajustes de interfaz) debe incrementar la versión semántica (`patch`, `minor` o `major`).
   * La versión debe proyectarse tanto en el archivo de configuración del proyecto (`pubspec.yaml`, `package.json`, etc.) como en la interfaz de usuario visible al cliente o administrador.

2. **Cero Despliegues Fantasma:**
   * Al incrementar la versión en cada cambio, la presencia de la cadena `vX.Y.Z` en el artefacto compilado se convierte en la **prueba física irrefutable** de que el código actual fue compilado exitosamente y que no se está reutilizando una caché obsoleta.

3. **Trazabilidad Histórica Inmutable:**
   * Llevar un registro (`.version_history.json` o equivalente) que certifique la versión actual, la versión previa validada, fecha de despliegue y la huella criptográfica (SHA-256) del artefacto final.
