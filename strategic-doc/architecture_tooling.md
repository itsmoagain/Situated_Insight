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

### Key layers in the stack described

<details>
  <summary><strong>Practice Logging Tools</strong></summary>
  <p>Land stewards, co-ops, or coordinators record practices using:</p>
  <ul>
    <li>KoboToolbox, Tella, or FieldKit (supports offline use, mobile, local language)</li>
    <li>Paper forms optionally digitized</li>
    <li>Voice or SMS-based input (for low-bandwidth regions)</li>
  </ul>
</details>

<details>
  <summary><strong>Climate Data Oracles</strong></summary>
  <p>Logs include timestamp, GPS, practice code, crop or land type, and optional photos, notes, or metadata.</p>
  <p>Trusted environmental signals (e.g., rainfall, temperature anomalies, NDVI) are pulled based on log location and timing — providing raw context for enrichment without requiring the contributor to interpret climate data themselves.</p>
</details>

<details>
  <summary><strong>Agentic Insights</strong></summary>
  <p>AI agents generate climate-contextualized insights, tags, and metadata from enriched practice logs — turning raw entries into decision-relevant feedback, visualizations, and traceable value.</p>
</details>

<details>
  <summary><strong>Data Storage and Sovereignty</strong></summary>
  <p>Holochain or IPFS Cluster provide edge-based syncing and local-first control, ensuring data remains with the contributor or cooperative unless consented for sharing.</p>
</details>

<details>
  <summary><strong>Governance Models</strong></summary>
  <p>DAOhaus, DisCO, and Coordinape allow each node to design its own validation logic, funding rules, and proposal flows.</p>
</details>

<details>
  <summary><strong>Impact and Credential Layers</strong></summary>
  <p>Practice bundles can be converted into Hypercerts, contributor badges, or ESG-compatible reports — supported by agents that handle formatting and standard mapping.</p>
</details>

<details>
  <summary><strong>Visualization and Feedback</strong></summary>
  <p>Dashboards return enriched insights to contributors — for example, “Your composting during a heatwave likely improved microbial retention” — helping make climate action legible in real time.</p>
</details>

