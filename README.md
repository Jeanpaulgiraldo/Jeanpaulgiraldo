<!-- BANNER SUPERIOR DINÁMICO -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:161B22,100:FF6B00&height=210&section=header&text=Jean%20Paul%20Giraldo&fontSize=46&fontColor=FFFFFF&fontAlignY=38&desc=Full%20Stack%20Developer%20%E2%80%A2%20UI%2FUX%20Architect%20%E2%80%A2%20Data%20%26%20Cloud&descSize=18&descColor=FF6B00&descAlignY=62&animation=fadeIn" width="100%" />
</div>

<!-- BARRA DE NAVEGACIÓN / ECOSISTEMA -->
<div align="center">
  <a href="https://jeanpaulgiraldo.github.io/" target="_blank">
    <img src="https://img.shields.io/badge/PORTAFOLIO_WEB-0D1117?style=for-the-badge&logo=googlechrome&logoColor=FF6B00" />
  </a>
  <a href="https://www.linkedin.com/in/jean-paul-giraldo-6b59a5275" target="_blank">
    <img src="https://img.shields.io/badge/LINKEDIN-0D1117?style=for-the-badge&logo=linkedin&logoColor=0A66C2" />
  </a>
  <img src="https://img.shields.io/badge/MEDELL%C3%8DN%2C_COLOMBIA-0D1117?style=for-the-badge&logo=googlemaps&logoColor=FF6B00" />
</div>

<br/>

<!-- MATRIZ DE IDENTIDAD Y ARQUITECTURA (2 COLUMNAS SIMÉTRICAS) -->
<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">⚡ Perfil & Enfoque</h3>
      <p align="justify">
        Ingeniero de software en formación y diseñador híbrido especializado en construir <b>productos digitales de extremo a extremo</b>. Combino arquitectura backend robusta, desarrollo móvil nativo, diseño de interfaces centradas en el usuario y pipelines de calidad de datos.
      </p>
      <ul>
        <li>🎨 <b>Diseño + Código:</b> Interfaces funcionales con criterio UI/UX.</li>
        <li>📱 <b>Ecosistema Híbrido:</b> Web reactiva & Android nativo (Offline-First).</li>
        <li>📊 <b>Data & BI:</b> Ingeniería ETL/ELT y gobernanza de datos.</li>
        <li>☁️ <b>Cloud Native:</b> Contenedores, microservicios y automatización.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">🏆 Credenciales & Certificaciones</h3>
      <p align="center">
        <img src="https://img.shields.io/badge/AWS-Cloud_&_GenAI-232F3E?style=flat-square&logo=amazon-aws&logoColor=FF9900" /><br/>
        <img src="https://img.shields.io/badge/Google-Cloud_&_GenAI-1A73E8?style=flat-square&logo=google-cloud&logoColor=white" /><br/>
        <img src="https://img.shields.io/badge/IBM-AI,_LLMs_&_Vision-052FAD?style=flat-square&logo=ibm&logoColor=white" /><br/>
        <img src="https://img.shields.io/badge/BI_&_Data_Quality-SQL_/_ETL-FF6B00?style=flat-square&logo=databricks&logoColor=white" />
      </p>
      <blockquote>
        <i>"Transformando ideas de negocio en sistemas escalables, visualmente impecables y respaldados por datos reales."</i>
      </blockquote>
    </td>
  </tr>
</table>

---

### 🧬 Blueprint de Arquitectura (Cómo conecto las piezas)

```mermaid
graph LR
    subgraph Client ["🖥️ Capa de Experiencia (UI/UX)"]
        direction TB
        WEB["React / TypeScript"]
        MOB["Kotlin / Android"]
        SQLITE[("SQLite Local")]
        MOB <--> SQLITE
    end

    subgraph Core ["⚙️ Núcleo & Orquestación"]
        direction TB
        API{"FastAPI / C# / Java"}
        AUTO["n8n Automation"]
        API <--> AUTO
    end

    subgraph CloudData ["☁️ Persistencia, BI & Cloud"]
        direction TB
        PG[("PostgreSQL")]
        ETL["ETL & Data Quality"]
        K8S(("Docker & Kubernetes"))
        PG --> ETL
    end

    WEB <-->|REST / JSON| API
    MOB <-->|Sync Engine| API
    API <--> PG
    Core -.-> K8S

    style Client fill:#161B22,stroke:#FF6B00,stroke-width:2px,color:#FFFFFF
    style Core fill:#161B22,stroke:#38BDF8,stroke-width:2px,color:#FFFFFF
    style CloudData fill:#161B22,stroke:#10B981,stroke-width:2px,color:#FFFFFF
