<div align="center">
  <a href="https://jeanpaulgiraldo.github.io/">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=FF6B00&center=true&vCenter=true&width=750&lines=Jean+Paul+Giraldo+%7C+Full+Stack+Architect;UI%2FUX+Design+%2B+Software+Engineering;Mobile+(Kotlin)+%7C+Backend+(FastAPI+%2F+C%23);Data+Quality%2C+BI+Pipelines+%26+Cloud" alt="Typing SVG" />
  </a>

  <p>
    <a href="https://jeanpaulgiraldo.github.io/" target="_blank">
      <img src="https://img.shields.io/badge/🌐_Portafolio_Web-111111?style=for-the-badge&logo=githubpages&logoColor=FF6B00" />
    </a>
    <a href="https://www.linkedin.com/in/jean-paul-giraldo-6b59a5275" target="_blank">
      <img src="https://img.shields.io/badge/💼_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
    </a>
  </p>
</div>

---

### 📐 Arquitectura de mi Perfil (Ecosistema End-to-End)

```mermaid
flowchart LR
    subgraph Capa_Visual [🎨 Frontend & Mobile]
        A[UI/UX Design] --> B(React / TypeScript)
        A --> C(Kotlin / Android)
    end

    subgraph Capa_Logica [⚙️ Backend & Automatización]
        B & C <-->|API REST / JSON| D{FastAPI / C#}
        D <--> E[n8n Workflows]
    end

    subgraph Capa_Datos [🗄️ Datos, BI & Cloud]
        C -.->|Offline-First| F[(SQLite)]
        D <--> G[(PostgreSQL)]
        G --> H[ETL & Data Quality]
        D & G -.-> I((Docker / K8s / Cloud))
    end

    style Capa_Visual fill:#161b22,stroke:#FF6B00,stroke-width:2px,color:#fff
    style Capa_Logica fill:#161b22,stroke:#009688,stroke-width:2px,color:#fff
    style Capa_Datos fill:#161b22,stroke:#316192,stroke-width:2px,color:#fff
<!--
**Jeanpaulgiraldo/Jeanpaulgiraldo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
