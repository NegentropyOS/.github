<a href="https://discord.gg/g8nqB3NtXt"><img align="right" src="https://img.shields.io/badge/NEGENTROPY-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="NEGENTROPY on Discord"></a>
<a href="https://opensource.org/licenses/Apache-2.0"><img align="right" src="https://img.shields.io/badge/Apache_2.0-181717?style=for-the-badge&logoColor=white" alt="Apache 2.0"></a>
<div align="left"><a href="./README.md">English</a> | Español</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="org-negentropy.gif">
  <img src="org-negentropy-light.gif" alt="Logotipo de NEGENTROPY animándose hasta su posición" width="960">
</picture>

<p align="center"><strong>Orden desde el caos para la era de los agentes de IA.</strong></p>

<p align="center"><em>Infraestructura determinista y memoria persistente para sistemas autónomos en los que se puede confiar.</em></p>

---

## Qué es NegentropyOS

NegentropyOS construye **infraestructura verificable y determinista para agentes de IA**.

Los modelos de lenguaje grandes aportan inteligencia estadística cruda, pero los entornos operativos corporativos demandan estados predecibles, memoria reproducible y soberanía estricta de datos. NegentropyOS provee la capa de ingeniería que transforma la inferencia no determinista en ejecuciones confiables y auditables.

Nuestra tesis técnica es directa: **la infraestructura debe sobrevivir a la realidad operativa**. Separamos la salida probabilística de los modelos del almacenamiento transaccional con garantías ACID y sustratos de ejecución verificables.

---

## Sustrato Activo: VantaDB

Nuestro componente central en producción activa es **VantaDB** — un motor embebido de recuperación híbrida y memoria persistente escrito en **Rust**.

| Propiedad | Detalle |
|---|---|
| **Repositorio** | [`ness-e/Vantadb`](https://github.com/ness-e/Vantadb) |
| **Versión Actual** | `v0.7.0` (Librería en producción en PyPI y crates.io) |
| **Arquitectura del Motor** | Embebido, local-first, zero-copy, acelerado por SIMD |
| **Mecánica de Recuperación** | Vectorial denso (HNSW) + Léxico texto completo (BM25) con fusión RRF (*Reciprocal Rank Fusion*) |
| **Persistencia y Garantías** | Transaccionalidad ACID, WAL (*Write-Ahead Logging*), aislamiento MVCC |
| **Ecosistema y Conectores** | Bindings en Python (`vantadb-py`), LangChain (`vantadb-langchain`), Mem0 (`vantadb-mem0`) |

VantaDB provee a los agentes autónomos memoria episódica y semántica de latencia submilisegundo sin la sobrecarga operativa ni la latencia de red de clústeres externos.

---

## Estructura de Repositorios

Mantenemos una arquitectura limpia y sin sobrecarga de repositorios vacíos:

| Repositorio | Ámbito | Descripción |
|---|---|---|
| [`VantaDB`](https://github.com/ness-e/Vantadb) | **Sustrato Central** | Motor embebido de memoria y recuperación híbrida en Rust. |
| [`NEGENTROPY`](https://github.com/NegentropyOS/NEGENTROPY) | **Especificaciones y RFCs** | Diseños arquitectónicos, especificaciones de investigación y runtime de agentes. |
| [`.github`](https://github.com/NegentropyOS/.github) | **Organización y Gobernanza** | Perfil institucional, manifiesto técnico y estándares de contribución. |

---

## Hoja de Ruta e Investigación Técnica

En lugar de dispersar el esfuerzo en repositorios vacíos, nuestras capacidades futuras se gestionan como especificaciones rigurosas dentro de [`NegentropyOS/NEGENTROPY`](https://github.com/NegentropyOS/NEGENTROPY):

```
+-------------------------------------------------------------+
¦                    RUNTIME DEL AGENTE                       ¦
+-------------------------------------------------------------+
                               ?
+-------------------------------------------------------------+
¦  Fase 3: Verificación y Metacognición (RFC Meta)            ¦
¦  - Atestación de ejecución, auditoría y control de alucinación¦
+-------------------------------------------------------------+
                               ?
+-------------------------------------------------------------+
¦  Fase 2: Contexto y Anclaje Episódico (RFC Cardinal)        ¦
¦  - Estado bitemporal, presupuesto de tokens y grafos de memoria¦
+-------------------------------------------------------------+
                               ?
+-------------------------------------------------------------+
¦  Fase 1: Sustrato de Memoria Persistente (VantaDB - Activo) ¦
¦  - Núcleo en Rust, HNSW + BM25, persistencia local ACID     ¦
+-----------------------------+
```

1. **Sustrato (Activo):** Memoria persistente de alto rendimiento y bajo consumo mediante **VantaDB**.
2. **Anclaje de Contexto (RFC Cardinal):** Memoria de trabajo bitemporal que registra qué supo el agente, cuándo lo supo y el linaje de las fuentes.
3. **Auditabilidad y Confianza (RFC Meta):** Atestación criptográfica y registro inmutable de auditoría para ejecuciones de herramientas.

---

## Principios de Ingeniería

1. **Infraestructura, no aplicaciones finales:** Construimos los cimientos sobre los cuales operan los agentes.
2. **Local-First y Soberano:** Minimizamos el acoplamiento a servicios en la nube externos; priorizamos ejecución local y gobernanza en premisa.
3. **Estado Determinista sobre Garantías Estadísticas:** Aislar el razonamiento probabilístico de esquemas rígidos y almacenamiento transaccional.
4. **Transparencia Radical:** Métricas reales, benchmarks reproducibles y análisis explícito de modos de falla.

?? **Manifiesto Completo**: [MANIFESTO_ES.md](https://github.com/NegentropyOS/.github/blob/main/MANIFESTO_ES.md)

---

## Comunidad y Contribución

- **?? Reporte de Errores**: Issues técnicos y benchmarks en los repositorios correspondientes.
- **?? Comunidad**: Conversaciones y desarrollo en [Discord](https://discord.gg/g8nqB3NtXt).
- **?? Contacto**: [NegentropyOS.ia@gmail.com](mailto:NegentropyOS.ia@gmail.com)
- **?? Guía de Contribución**: Ver [CONTRIBUTING_ES.md](https://github.com/NegentropyOS/.github/blob/main/CONTRIBUTING_ES.md)

---

## Licencia

Código distribuido bajo [Licencia Apache 2.0](https://github.com/NegentropyOS/.github/blob/main/LICENSE).

**NegentropyOS** — Orden desde el caos.

