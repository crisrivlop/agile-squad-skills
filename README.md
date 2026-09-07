# 👥 Agile Squad Skills

Catálogo universal y modular de **Roles Ágiles y Habilidades (Skills)** para asistentes y agentes de Inteligencia Artificial (Antigravity, Claude Desktop, Cursor, OpenAI Codex).

---

## 🏛️ Arquitectura: El Squad Consume a los Skills

En este ecosistema:
* **El Squad (`squad/`):** Define los **actores/roles** del equipo (PO, Arquitecto, QA, AppSec, DevOps, etc.) con sus responsabilidades e identidades operativas.
* **Los Skills (`skills/`):** Son las **unidades atómicas de procedimiento y conocimiento** (`SKILL.md`) que los roles consultan y ejecutan para garantizar un ciclo de vida de desarrollo de software (SDLC) riguroso.

---

## 🌟 Roles Disponibles en el Squad

| Rol | Slug | Skills que Consume | Responsabilidad Principal |
| :--- | :--- | :--- | :--- |
| **👑 Product Owner** | `product-owner-sentinel` | `product-owner-sentinel` | Refinamiento con Stakeholders, Triángulo de Hierro, User Stories Given/When/Then. |
| **🛡️ Scrum Master** | `scrum-master-sentinel` | `scrum-master-sentinel` | Gobernanza del backlog, control de checklist, aprobación humana innegociable. |
| **🏗️ Senior Architect** | `senior-tech-architect` | `senior-tech-architect`, `clean-code-reviewer` | Volumetría, tráfico, Clean Architecture y Definition of Done (DoD). |
| **🎨 UX/UI Designer** | `ux-ui-design-sentinel` | `ux-ui-design-sentinel` | Ergonomía visual, accesibilidad (WCAG AA) y diseño centrado en el usuario. |
| **🧹 Clean Code Reviewer** | `clean-code-reviewer` | `clean-code-reviewer` | Cláusulas de Guarda (Early Returns), KISS, DRY y aplanado de flujo a la izquierda. |
| **🧪 QA Lead** | `qa-lead-sentinel` | `qa-lead-sentinel` | 100% de cobertura en lógica y verificación real de compilación de UI. |
| **🔒 Security & AppSec** | `security-appsec-sentinel` | `security-appsec-sentinel` | Prevención de fuga de secretos, mitigación de OWASP Top 10 y auditoría de CVEs. |
| **🚀 DevOps & SRE** | `devops-sre-sentinel` | `devops-sre-sentinel` | Pipelines de CI/CD, observabilidad, métricas y despliegues sin caída. |
| **📊 Data & Analytics** | `data-analytics-sentinel` | `data-analytics-sentinel` | Taxonomía de eventos, telemetría y métricas de retención/conversión. |
| **🏷️ Release Guardian** | `version-bump-guardian` | `version-bump-guardian` | SemVer atómico, certificación física en binarios y trazabilidad inmutable. |

---

## 🚀 Compatibilidad

* **Google Antigravity:** Instalable globalmente en `~/.gemini/config/skills/` o a nivel de workspace en `.agents/skills/`.
* **Model Context Protocol (MCP):** Compatible con el servidor MCP `@agile-squad/mcp-server`.
