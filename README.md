<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:F5A623&height=180&section=header&text=Kinza&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Software%20Development%20Engineer&descAlignY=55&descSize=16"/>
  
<h3>AI/ML Engineer · Backend Developer · Computer Vision & LLM Systems</h3>

<p style="font-size:18px"><strong>Rector's List (3x) · Dean's List (2x) 🏆</strong><br/>
I ship production ML and backend systems: from fine-tuned LLM pipelines and computer vision models to FastAPI services with real concurrency and auth concerns.</p>

[![GitHub followers](https://img.shields.io/github/followers/kinza7124?label=Followers&style=for-the-badge&labelColor=161B22&color=F5A623)](https://github.com/kinza7124?tab=followers)&nbsp;[![GitHub User's stars](https://img.shields.io/github/stars/kinza7124?label=Total%20Stars&style=for-the-badge&labelColor=161B22&color=F5A623)](https://github.com/kinza7124)&nbsp;<a href="https://portfolio-kinza-bscs.vercel.app/"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-161B22?style=for-the-badge&logo=vercel&logoColor=F5A623&labelColor=161B22"/></a>&nbsp;<a href="https://linkedin.com/in/kinza-afzal7-"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-161B22?style=for-the-badge&logo=linkedin&logoColor=F5A623&labelColor=161B22"/></a>

</div>
</div>

---

## About Me

```cpp
/*
 * ============================================
 *   SYSTEM BOOT :: kinza_afzal.exe
 *   Compiling with -O3 -Wall -std=c++23
 * ============================================
 */

#include <iostream>
#include <vector>
#include <string>
#include <memory>

using namespace std;

class Engineer {
private:
    // Singleton -- there's only one of me, and I ship.
    static inline unique_ptr<Engineer> instance = nullptr;

    Engineer() = default;

public:
    string name      = "Kinza Afzal";
    string role      = "AI/ML Engineer & Backend Developer";
    string location  = "Karachi, Pakistan";
    string education = "BS CS @ FAST NUCES | Rector's List x3, Dean's List x2";

    vector<string> shipped = {
        "[CV]      PPE-compliance pipeline    -> RF-DETR, 97.8% mAP@50",
        "[LLM/RAG] Medi Query                 -> 92% relevancy, 153 tests passing",
        "[ML]      Network Logs Analyzer      -> 96%+ anomaly detection, 494K+ logs",
        "[DL]      FloodDepth Estimation      -> Attention U-Net + ZoeDepth, MLOps end-to-end",
        "[BACKEND] Invite Flow API            -> Node.js/Express, 12+ RLS policies, OAuth",
        "[SYS]     SLA/Penalty Engine         -> FastAPI + PostgreSQL, concurrency-safe"
    };

    vector<string> stack = {
        "Python", "FastAPI", "PostgreSQL", "LangChain",
        "LangGraph", "PyTorch", "TensorFlow", "Docker",
        "Node.js", "Express", "MongoDB", "REST API"
    };

    vector<string> backend_focus = {
        "System Design    -> scalable service boundaries, API contracts, caching layers",
        "Node.js/Express  -> REST APIs, middleware, auth (JWT/OAuth), rate limiting",
        "MongoDB          -> schema design, aggregation pipelines, indexing strategy",
        "Message Queues   -> async job processing, event-driven pipelines, retries/DLQs",
        "Concurrency      -> row-level locking, SLA/penalty engines, race-condition-safe writes",
        "DevOps           -> Docker/Compose, CI/CD (GitHub Actions), AWS EC2, MLflow, monitoring"
    };

    static Engineer& getInstance() {
        if (!instance) instance = unique_ptr<Engineer>(new Engineer());
        return *instance;
    }

    friend ostream& operator<<(ostream& os, const Engineer& e) {
        os << ">> booting " << e.name << " ...\n";
        os << ">> role     : " << e.role << "\n";
        os << ">> location : " << e.location << "\n";
        os << ">> status   : compiling ideas into production systems\n\n";
        os << ">> git log --oneline --author=\"kinza\"\n";
        for (const auto& log : e.shipped)
            os << "   " << log << "\n";
        os << "\n>> cat backend_focus.txt\n";
        for (const auto& item : e.backend_focus)
            os << "   " << item << "\n";
        return os;
    }

    void ship() const {
        cout << *this;
        cout << "\n>> return 0;  // and ready for the next commit\n";
    }
};

int main() {
    Engineer& me = Engineer::getInstance();
    me.ship();
    return 0;
}

/* ============================================
 *   Process finished with exit code 0
 *   Uptime: since 2023 | Status: still compiling
 * ============================================
 */
```

---

## What I Do

- **AI Product Engineer Intern @ Agento**: building on an enterprise AI operations platform (React 18, TypeScript, Vite); shipping features and fixing bugs across the Skills Engine, Model Router, and Agent Shield (RBAC/ABAC policy engine), and partnering with the compliance team on the Evidence Center's audit-trail and governance flows for launch
- **AI/ML Engineer Intern @ SYSLAB.AI**: computer vision pipelines (OpenCV, Roboflow) for hospital PPE-compliance and anomaly detection; fine-tuned Qwen2.5-3B for automated interview psychometric scoring
- **Software Development Engineer (Research) @ FAST NUCES KHI**: multi-agent AI replanning system (LangGraph, CrewAI, Neo4j) benchmarked against 7 classical optimization algorithms; scalable FastAPI/PostgreSQL backend with concurrency-safe SLA/penalty engines
- **Former AI/ML Trainee @ Shark Stack**: AI voice receptionist (Vapi.ai + n8n) with tool-calling workflows; RAG chatbot (LangChain, Pinecone, Groq) at 88%+ response accuracy, Dockerized CI/CD on AWS
- **Teaching Assistant @ FAST NUCES KHI**: Data Structures & Database Systems; mentored 40+ students, graded 20+ semester projects
- **Specialties**: computer vision, LLM fine-tuning & RAG pipelines, multi-agent systems, backend architecture with row-level security & concurrency control
- **Open to** <strong>AI/ML Engineering, Backend roles, and research collaborations</strong>

---

## Featured Projects

- **[Medi Query: AI Medical Assistant](https://github.com/kinza7124/Medi-Query)**: Medical RAG chatbot (Llama 3.3 70B, hybrid MMR+BM25 retrieval, cross-encoder reranking) with 92% relevancy, 88.7% faithfulness, and 153-test coverage across unit/integration/security/performance, deployed via Dockerized CI/CD on AWS EC2.
- **[Network Logs Analyzer](https://github.com/kinza7124/Network-Log-Analyzer)**: Real-time SOC dashboard powered by a GHF-ART clustering model (96%+ detection accuracy across 494K+ network connections), with live threat visualizations, ChatOps analysis, and automated critical-alert escalation.
- **[FloodDepth Estimation](https://huggingface.co/spaces/Kinzaaa/flood-risk-detection)**: Flood detection & risk assessment system using Attention U-Net segmentation (86.95% Dice/F1, 76.91% IoU) with ZoeDepth metric depth estimation and Grad-CAM explainability, deployed via a full MLOps pipeline (MLflow, FastAPI, Gradio, Hugging Face Spaces).
- **[Invite Flow](https://digital-invite-genie.vercel.app/)**: Supabase Postgres backend with 4 relational tables, 12+ Row-Level Security policies, and security-definer functions; email/password + Google OAuth auth and QR-based invitation/check-in flows, deployed on Vercel with CI-driven multi-environment config.
- **[PixelLang Compiler](https://github.com/kinza7124/PixelLang)**: A retro-inspired domain-specific language for pixel art generation, with a complete compiler pipeline (DFA-based lexer, LL(1) recursive-descent parser, 37-rule semantic analyzer, Pillow-based codegen) and a full Tkinter GUI IDE with syntax highlighting and live preview. Built for CS4031 Compiler Construction.
- **[Gravity Switch](https://github.com/kinza7124/gravity-flip)**: A fast-paced 2D auto-runner mobile game (React Native + Expo, TypeScript, Zustand) where a single tap flips gravity to dodge neon obstacles in a cyberpunk world, with progressive difficulty, particle effects, and haptic feedback, built end-to-end with EAS builds.
- **[Traffic Simulation System](https://github.com/kinza7124/Traffic_Simulation-OS_Project)**: A multi-threaded traffic simulation (C, POSIX pthreads) modeling traffic flow across multiple intersections, with mutex/condition-variable synchronization, priority scheduling for emergency vehicles, `inotify`-based hot-reloading config, and a real-time `ncurses` GUI with live system performance monitoring. Built for an Operating Systems course.

<div align="center">

<a href="https://github.com/kinza7124/Medi-Query">
  <img width="49%" src="https://github-readme-stats-fast.vercel.app/api/pin/?username=kinza7124&repo=Medi-Query&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9&border_color=161B22" alt="Medi Query: AI Medical Assistant"/>
</a>
<a href="https://github.com/kinza7124/Network-Log-Analyzer">
  <img width="49%" src="https://github-readme-stats-fast.vercel.app/api/pin/?username=kinza7124&repo=Network-Log-Analyzer&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9&border_color=161B22" alt="Network Logs Analyzer"/>
</a>

<a href="https://github.com/kinza7124/PixelLang">
  <img width="49%" src="https://github-readme-stats-fast.vercel.app/api/pin/?username=kinza7124&repo=PixelLang&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9&border_color=161B22" alt="PixelLang Compiler"/>
</a>
<a href="https://github.com/kinza7124/gravity-flip">
  <img width="49%" src="https://github-readme-stats-fast.vercel.app/api/pin/?username=kinza7124&repo=gravity-flip&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9&border_color=161B22" alt="Gravity Switch"/>
</a>
<a href="https://github.com/kinza7124/Traffic_Simulation-OS_Project">
  <img width="49%" src="https://github-readme-stats-fast.vercel.app/api/pin/?username=kinza7124&repo=Traffic_Simulation-OS_Project&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9&border_color=161B22" alt="Traffic simulation"/>
</a>

</div>

<div align="center">

<a href="https://huggingface.co/spaces/Kinzaaa/flood-risk-detection"><img alt="Hugging Face Space" src="https://img.shields.io/badge/🤗%20Hugging%20Face-FloodDepth%20Estimation-161B22?style=for-the-badge&labelColor=161B22&color=F5A623"/></a>

</div>

---

## Open-Source

- **[ImportOptimizer](https://www.npmjs.com/package/@kinza7/import-optimizer)**: AST-based npm codemod (TypeScript, Babel scope analysis, magic-string) that detects whole-library imports and safely rewrites them into tree-shakable direct imports, preserving original formatting.

---

## 📄 Publications

- **[Data Security Posture Management (DSPM) in the Era of Generative AI and Agentic AI: Toward an Intelligent Agentic DSPM (IADSPM) Framework](https://www.researchgate.net/publication/413599467_Data_Security_Posture_Management_DSPM_in_the_Era_of_Generative_AI_and_Agentic_AI_Toward_an_Intelligent_Agentic_DSPM_IADSPM_Framework)**: Technical Note, ResearchGate. Proposes an intelligent, agentic approach to Data Security Posture Management (DSPM) for securing data across generative and agentic AI systems.

---

## 🏅 GitHub Achievements

<p align="center">
<strong>Pair Extraordinaire</strong> — @kinza7124 coauthored commits on merged pull requests.
</p>

<p align="center">
<!-- Pull Shark -->
<img src="https://github.githubassets.com/images/modules/profile/achievements/pull-shark-default.png" width="95" alt="Pull Shark" />
<!-- Quickdraw -->
<img src="https://github.githubassets.com/images/modules/profile/achievements/quickdraw-default.png" width="95" alt="Quickdraw" />
<!-- YOLO -->
<img src="https://github.githubassets.com/images/modules/profile/achievements/yolo-default.png" width="95" alt="YOLO" />
</p>

---

## Tech Stack

### Languages
<p>
<img alt="Python" src="https://img.shields.io/badge/Python-161B22?style=for-the-badge&logo=python&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="C++" src="https://img.shields.io/badge/C++-161B22?style=for-the-badge&logo=cplusplus&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="C" src="https://img.shields.io/badge/C-161B22?style=for-the-badge&logo=c&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-161B22?style=for-the-badge&logo=javascript&logoColor=F5A623&labelColor=161B22"/>
</p>

### AI/ML & NLP
<p>
<img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-161B22?style=for-the-badge&logo=pytorch&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-161B22?style=for-the-badge&logo=tensorflow&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="LangChain" src="https://img.shields.io/badge/LangChain-161B22?style=for-the-badge&logo=langchain&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="LangGraph" src="https://img.shields.io/badge/LangGraph-161B22?style=for-the-badge&logo=langgraph&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="LangSmith" src="https://img.shields.io/badge/LangSmith-161B22?style=for-the-badge&logo=langchain&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="CrewAI" src="https://img.shields.io/badge/CrewAI-161B22?style=for-the-badge&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Scikit-learn" src="https://img.shields.io/badge/scikit--learn-161B22?style=for-the-badge&logo=scikitlearn&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-161B22?style=for-the-badge&logo=opencv&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-161B22?style=for-the-badge&logo=huggingface&logoColor=F5A623&labelColor=161B22"/>
</p>

### Backend & System Design
<p>
<img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-161B22?style=for-the-badge&logo=fastapi&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Node.js" src="https://img.shields.io/badge/Node.js-161B22?style=for-the-badge&logo=nodedotjs&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Express" src="https://img.shields.io/badge/Express-161B22?style=for-the-badge&logo=express&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="NestJS" src="https://img.shields.io/badge/NestJS-161B22?style=for-the-badge&logo=nestjs&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Next.js" src="https://img.shields.io/badge/Next.js-161B22?style=for-the-badge&logo=nextdotjs&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Prisma" src="https://img.shields.io/badge/Prisma-161B22?style=for-the-badge&logo=prisma&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="RabbitMQ" src="https://img.shields.io/badge/RabbitMQ-161B22?style=for-the-badge&logo=rabbitmq&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Apache Kafka" src="https://img.shields.io/badge/Kafka-161B22?style=for-the-badge&logo=apachekafka&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Redis" src="https://img.shields.io/badge/Redis-161B22?style=for-the-badge&logo=redis&logoColor=F5A623&labelColor=161B22"/>
</p>

### Databases & Cloud
<p>
<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-161B22?style=for-the-badge&logo=postgresql&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-161B22?style=for-the-badge&logo=mongodb&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="MySQL" src="https://img.shields.io/badge/MySQL-161B22?style=for-the-badge&logo=mysql&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Neo4j" src="https://img.shields.io/badge/Neo4j-161B22?style=for-the-badge&logo=neo4j&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Docker" src="https://img.shields.io/badge/Docker-161B22?style=for-the-badge&logo=docker&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="AWS" src="https://img.shields.io/badge/AWS-161B22?style=for-the-badge&logo=amazonwebservices&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Vercel" src="https://img.shields.io/badge/Vercel-161B22?style=for-the-badge&logo=vercel&logoColor=F5A623&labelColor=161B22"/>
</p>

### DevOps & Tools
<p>
<img alt="Git" src="https://img.shields.io/badge/Git-161B22?style=for-the-badge&logo=git&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub%20Actions-161B22?style=for-the-badge&logo=githubactions&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="MLflow" src="https://img.shields.io/badge/MLflow-161B22?style=for-the-badge&logo=mlflow&logoColor=F5A623&labelColor=161B22"/>&nbsp;<img alt="Postman" src="https://img.shields.io/badge/Postman-161B22?style=for-the-badge&logo=postman&logoColor=F5A623&labelColor=161B22"/>
</p>

---

## Education

| Institute | Program | Result | Years |
|---|---|---|---|
| FAST NUCES | BS Computer Science | CGPA 3.5/4.00: Rector's List (3x), Dean's List (2x) | 2023 - 2027 |
| Highbrow College | A Levels | 3A* 1A | 2021 - 2023 |

---

## GitHub Stats

<div align="center">

<img width="49%" src="https://github-readme-stats-fast.vercel.app/api?username=kinza7124&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&bg_color=0D1117&title_color=F5A623&icon_color=F5A623&text_color=C9D1D9" alt="GitHub Stats"/>
</div>

---

## Connect

<div align="center">

<a href="https://portfolio-kinza-bscs.vercel.app/"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-161B22?style=for-the-badge&logo=vercel&logoColor=F5A623&labelColor=161B22"/></a>&nbsp;<a href="https://linkedin.com/in/kinza-afzal7-"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-161B22?style=for-the-badge&logo=linkedin&logoColor=F5A623&labelColor=161B22"/></a>&nbsp;<a href="mailto:kinzaafzal07122004@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-161B22?style=for-the-badge&logo=gmail&logoColor=F5A623&labelColor=161B22"/></a>

</div>

---

## Contribution Graph

<div align="center">

![Kinza's Contribution Graph](https://ghchart.rshah.org/F5A623/kinza7124)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F5A623,100:0D1117&height=100&section=footer"/>

</div>
