# Architrechture and Tooling

## Core Infrastructure Stack
The Regenerative DAO system is built on a modular, composable stack that enables contributors to log practices, enrich them with climate context, and participate in networked governance. Each component can operate independently or be combined to match the needs of a cooperative, regional network, or individual steward.

A core design pattern across the system is __two-layer enrichment:__

1. __[Oracled](glossary.md) Climate Data Context__
When a log is submitted, it is first enriched with raw climate data using trusted oracles (e.g., SPI, NDVI, temperature anomalies) based on GPS and timestamp. This overlays objective environmental conditions onto the log — without interpretation.

2. __Agent-Driven Insight__
AI agents then interpret this climate context and generate tags, feedback, or downstream triggers. These may help prioritize logs for funding, highlight resilience actions, or surface patterns across peers.

For example:

>A composting log is enriched with SPI = -1.8 (moderate drought) via a rainfall oracle. 
>An agent detects this context and adds a tag: “_composted during drought_”, along with feedback:
>“_This composting may help retain microbial activity during dry conditions_.”

_A deeper breakdown of this layer is available in the "Enrichment" section below_

<div align="center">
<img src="../diagrams/Data Stack 2025-05-23-1047.png" alt="Data Stack" width="450"/>  

  <em>Figure 4: Datastack </em>

</div>
