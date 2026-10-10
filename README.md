<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,50:1f6feb,100:58a6ff&height=200&section=header&text=Binita%20Dutta&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=I%20debug%20systems%20for%20fun%20and%20build%20them%20to%20last&descAlignY=60&descSize=18" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&color=58A6FF&center=true&vCenter=true&width=760&lines=%24+whoami+%E2%86%92+Software+Engineer+%7C+3.5%2B+yrs;%24+focus+%E2%86%92+real-time+%2B+data-intensive+backends;%24+tail+-f+production+%E2%86%92+industrial+SCADA+%40+HART;%24+status+%E2%86%92+open+to+new+opportunities)](https://git.io/typing-svg)

![Status](https://img.shields.io/badge/status-open_to_work-2ea043?style=for-the-badge) ![Roles](https://img.shields.io/badge/looking_for-Backend_%7C_Full--Stack-1f6feb?style=for-the-badge) ![Base](https://img.shields.io/badge/based_in-Kolkata,_India-orange?style=for-the-badge)

<a href="https://www.linkedin.com/in/binita-dutta"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
<a href="mailto:binitadutta777@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
<a href="https://leetcode.com/u/BinitaDutta_03/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=black" /></a>

</div>

---

## 🧭 The Short Version

Most engineers enjoy shipping features. I enjoy the moment *after*: when a report takes too long, a dashboard lags, or a database starts sweating, and someone has to work out **why**.

For 3.5+ years I've been doing exactly that at **Hamilton Research & Technology (HART)**, building software for **industrial SCADA systems**, where downtime is not an option and "it works on my machine" doesn't count.

```text
┌──────────────────────────────────────────────────────────────┐
│  🧠 Thinks in    →  bottlenecks, hot paths, data flow         │
│  🛠️ Builds with  →  Node.js · TypeScript · Kafka · Redis      │
│  📍 Lives in     →  real-time + high-volume data systems      │
│  🌱 Learning     →  LLMs · RAG · agentic AI                   │
│  🎓 Trained at   →  Asansol Engineering College (CGPA 9.01)   │
└──────────────────────────────────────────────────────────────┘
```

---

## 🩺 Bugs, Bottlenecks & Fixes

A few real problems I've diagnosed at work, and what changed afterwards.

| 🔍 The Problem | 🔧 What I Did | 📈 The Result |
|---|---|---|
| Slow report generation in a monolithic SCADA app | Split it into domain-specific **microservices** with Node.js/Express REST APIs | Report generation time **↓ 90%** |
| Frequent hot reads hammering the database | Introduced **Redis caching** on the hot path | Retrieval latency **↓ ~80%**, DB load **↓ 60%** |
| Operators polling APIs for live process data | Moved the pipeline to **Socket.IO event streaming** | Continuous updates, far fewer redundant requests |
| Operators acting on stale configs across tabs and machines | Built an **SSE-based sync mechanism** that flags stale data | Fewer conflicting or outdated configurations |
| High-volume real-time data eating disk space | Engineered **automated archival + retention cleanup** | Disk utilization **↓ ~30–40%** |
| Fragmented, line-by-line data access | Centralized retrieval for **500+ controllers** across **100+ operator endpoints** into one server | Historical data accessibility **↑ ~40–50%** |

---

## 🗺️ The Kind of System I Work On

A simplified, conceptual view of the architecture behind the table above:

```mermaid
flowchart LR
    C["500+ Controllers"] --> S["Centralized Data Server"]
    S <--> R[("Redis Cache")]
    S <--> D[("Database")]
    D -. "archive and purge" .-> A[("Archive")]
    S -- "Socket.IO live stream" --> O["Operator Interfaces (100+)"]
    S -- "SSE: config changed" --> O
```

---

## 🍔 Side Quest: Dinezo

A real-time food delivery platform I built to practice event-driven microservices end to end.

```mermaid
flowchart LR
    U["React Client"] --> SV["Node.js Services"]
    SV -- "async events via RabbitMQ" --> SV
    SV --> M[("MongoDB")]
    SV -- "Socket.IO" --> U
```

- 📨 **RabbitMQ** keeps services decoupled through asynchronous communication
- 📍 **Socket.IO** pushes live order status and rider location to the client
- 🐳 Containerized with **Docker**

[![Source](https://img.shields.io/badge/View_Source-24292e?style=for-the-badge&logo=github)](https://github.com/BinitaDuttaDec03/dinezo)

---

## 🧰 Toolbox

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white) ![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white) ![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

<details>
<summary><b>See the full list</b></summary>

<br>

| Area | Tools |
|---|---|
| **Languages** | TypeScript, JavaScript (ES6+), Python |
| **Backend** | Node.js, Express.js, REST APIs, JWT, OAuth2.0 |
| **Distributed & Real-Time** | Apache Kafka, RabbitMQ, Redis, Socket.IO, Server-Sent Events, Event-Driven Architecture |
| **Databases** | MongoDB, PostgreSQL, Mongoose, Prisma |
| **Frontend** | React.js, Next.js, Redux, Zustand, Tailwind CSS |
| **Architecture & Tools** | Microservices, System Design, Git, Docker, Postman, Swagger/OpenAPI |

</details>

---

## 🌱 Currently Exploring

- 🤖 **LLMs, RAG, and agentic AI**, and how to fit them into practical, scalable software instead of demos
- 🏗️ Deeper **system design** and **distributed systems** patterns
- ⚙️ **Performance engineering** for real-time, data-intensive workloads

---

## 🏅 Recognition

🌟 **Star Performer of the Month** at HART, for end-to-end project ownership, client management, and delivering maintainable solutions from requirements through production.

---

## 📊 Activity

<div align="center">

<img src="https://streak-stats.demolab.com?user=BinitaDuttaDec03&theme=tokyonight&hide_border=true" />

</div>

---

## 🤝 Let's Talk

If you're building something **real-time, data-heavy, or just painfully slow**, I'd love to hear about it.

I'm looking for **Backend and Full-Stack Software Engineer** roles with teams working on system design, performance, and distributed systems.

📫 [binitadutta777@gmail.com](mailto:binitadutta777@gmail.com) &nbsp;·&nbsp; 💼 [LinkedIn](https://www.linkedin.com/in/binita-dutta) &nbsp;·&nbsp; 🧩 [LeetCode](https://leetcode.com/u/BinitaDutta_03/)

<div align="center">

[![Footer Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&pause=1200&color=58A6FF&center=true&vCenter=true&width=640&lines=%24+echo+%22Thanks+for+stopping+by!+%F0%9F%91%8B%22;%24+git+commit+-m+%22Let%27s+build+something+that+scales%22;%24+exit+0)](https://git.io/typing-svg)

</div>
