Copy everything inside the block below and paste it directly into your GitHub repository's `README.md` editor.

# 🛡️ SOC Command Centre

## 📌 Overview

SOC Command Centre is a full-stack, AI-assisted Security Operations Centre (SOC) platform designed to demonstrate how modern security teams can monitor security events, detect suspicious activities, investigate alerts, correlate threats, manage incidents and coordinate security responses through a unified interface.

The platform combines a FastAPI backend, React and TypeScript frontend, machine-learning-assisted anomaly detection, vector-based similarity search, MITRE ATT&CK mapping and SOAR-style response workflows.

It also includes an Attack Simulation Lab that generates fictional security events to demonstrate the complete security incident lifecycle, from event ingestion and threat detection to investigation, containment workflows and reporting.

The primary objective is to demonstrate how Artificial Intelligence, Machine Learning and security automation can improve SOC operations and support faster, more structured security incident management.

> ⚠️ This is an educational and research prototype. Attack scenarios use simulated data, and containment actions are demonstrated within the application rather than executed against real external systems.

## 🎯 Problem Statement

Modern organizations face increasing cybersecurity threats, including brute-force attacks, phishing, ransomware, credential theft, suspicious logins and data exfiltration.

Security teams often deal with large volumes of security alerts, making investigation, prioritization and incident response challenging.

SOC Command Centre addresses these challenges by demonstrating a centralized platform that supports:

- Centralized security event ingestion.
- Automated threat detection and alert generation.
- Anomaly detection using Machine Learning.
- Threat intelligence and MITRE ATT&CK mapping.
- Alert correlation and incident management.
- AI-assisted security investigation.
- Automated response workflows with approval mechanisms.
- Security reporting and operational monitoring.

## ✨ Key Features

### 🚨 1. Security Monitoring & Detection

- SIEM-style security event ingestion.
- Rule-based threat detection.
- Stateful detection scenarios.
- Machine-learning-assisted anomaly detection.
- Alert severity classification and risk scoring.
- Alert assignment, triage and status management.
- Threat intelligence and IOC enrichment.

### 🧠 2. AI-Powered SOC Copilot

- AI-assisted alert investigation.
- Incident summarization.
- Threat explanation and risk assessment.
- Recommended investigation steps.
- Similar incident retrieval.
- Context-aware security assistance.
- Deterministic fallback behavior when external AI services are unavailable.

### 🗺️ 3. Threat Intelligence & MITRE ATT&CK

- MITRE ATT&CK technique mapping.
- Threat intelligence context.
- IOC management.
- Attack graph visualization.
- Threat hunting workflows.
- Asset and identity inventory.
- Approximate threat-map visualization.

### 🛡️ 4. Incident Response & SOAR

- Incident creation and investigation.
- NIST SP 800-61-inspired incident lifecycle.
- Response playbooks.
- Playbook builder with triggers and conditions.
- Approval-based response actions.
- Simulated IP blocking.
- Simulated host isolation.
- Simulated account disabling.
- Containment verification and response logs.

### 📊 5. SOC Dashboard & Operations

- Real-time security dashboard.
- Authenticated WebSocket communication.
- Alert and incident monitoring.
- SLA countdown and breach monitoring.
- Role-based access control.
- Analyst, Manager and Admin experiences.
- Append-only, hash-chained audit trail.
- Executive and compliance reporting.
- In-app notifications and optional integrations.

### 🧪 6. Attack Simulation Lab

The platform includes seven fictional attack scenarios:

| Scenario            | Description                                       |
| ------------------- | ------------------------------------------------- |
| Brute Force         | Repeated authentication failures                  |
| Phishing to C2      | Phishing followed by command-and-control activity |
| Ransomware          | Simulated ransomware-related activity             |
| Data Exfiltration   | Suspicious outbound data transfer                 |
| Rogue Administrator | Suspicious privileged activity                    |
| Impossible Travel   | Unusual geographical login patterns               |
| Full Kill Chain     | Multi-stage targeted intrusion simulation         |

The full-kill-chain scenario demonstrates a fictional sequence involving phishing, command and control, credential theft, lateral movement, database access and data exfiltration.

## 🏗️ System Architecture

The platform follows a modular full-stack architecture connecting event ingestion, detection, threat enrichment, incident management and response automation.

\#chatgpt-mermaid-\_r_10p\_{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;fill:rgb(237, 237, 237);}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#chatgpt-mermaid-\_r_10p\_ .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-\_r_10p\_ .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-\_r_10p\_ .error-icon{fill:rgb(48, 48, 48);}#chatgpt-mermaid-\_r_10p\_ .error-text{fill:rgb(237, 237, 237);stroke:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .edge-thickness-normal{stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .edge-thickness-thick{stroke-width:3.5px;}#chatgpt-mermaid-\_r_10p\_ .edge-pattern-solid{stroke-dasharray:0;}#chatgpt-mermaid-\_r_10p\_ .edge-thickness-invisible{stroke-width:0;fill:none;}#chatgpt-mermaid-\_r_10p\_ .edge-pattern-dashed{stroke-dasharray:3;}#chatgpt-mermaid-\_r_10p\_ .edge-pattern-dotted{stroke-dasharray:2;}#chatgpt-mermaid-\_r_10p\_ .marker{fill:rgb(175, 175, 175);stroke:rgb(175, 175, 175);}#chatgpt-mermaid-\_r_10p\_ .marker.cross{stroke:rgb(175, 175, 175);}#chatgpt-mermaid-\_r_10p\_ svg{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;}#chatgpt-mermaid-\_r_10p\_ p{margin:0;}#chatgpt-mermaid-\_r_10p\_ .label{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";color:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .cluster-label text{fill:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .cluster-label span{color:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .cluster-label span p{background-color:transparent;}#chatgpt-mermaid-\_r_10p\_ .label text,#chatgpt-mermaid-\_r_10p\_ span{fill:rgb(237, 237, 237);color:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .node rect,#chatgpt-mermaid-\_r_10p\_ .node circle,#chatgpt-mermaid-\_r_10p\_ .node ellipse,#chatgpt-mermaid-\_r_10p\_ .node polygon,#chatgpt-mermaid-\_r_10p\_ .node path{fill:rgb(9, 23, 44);stroke:rgb(31, 78, 148);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .rough-node .label text,#chatgpt-mermaid-\_r_10p\_ .node .label text,#chatgpt-mermaid-\_r_10p\_ .image-shape .label,#chatgpt-mermaid-\_r_10p\_ .icon-shape .label{text-anchor:middle;}#chatgpt-mermaid-\_r_10p\_ .node .katex path{fill:#000;stroke:#000;stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .rough-node .label,#chatgpt-mermaid-\_r_10p\_ .node .label,#chatgpt-mermaid-\_r_10p\_ .image-shape .label,#chatgpt-mermaid-\_r_10p\_ .icon-shape .label{text-align:center;}#chatgpt-mermaid-\_r_10p\_ .node.clickable{cursor:pointer;}#chatgpt-mermaid-\_r_10p\_ .root .anchor path{fill:rgb(175, 175, 175)!important;stroke-width:0;stroke:rgb(175, 175, 175);}#chatgpt-mermaid-\_r_10p\_ .arrowheadPath{fill:rgb(175, 175, 175);}#chatgpt-mermaid-\_r_10p\_ .edgePath .path{stroke:rgb(175, 175, 175);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .flowchart-link{stroke:rgb(175, 175, 175);fill:none;}#chatgpt-mermaid-\_r_10p\_ .edgeLabel{background-color:rgb(0, 0, 0);text-align:center;}#chatgpt-mermaid-\_r_10p\_ .edgeLabel p{background-color:rgb(0, 0, 0);}#chatgpt-mermaid-\_r_10p\_ .edgeLabel rect{opacity:0.5;background-color:rgb(0, 0, 0);fill:rgb(0, 0, 0);}#chatgpt-mermaid-\_r_10p\_ .labelBkg{background-color:rgba(0, 0, 0, 0.5);}#chatgpt-mermaid-\_r_10p\_ .cluster rect{fill:rgb(48, 48, 48);stroke:rgba(255, 255, 255, 0.15);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .cluster text{fill:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ .cluster span{color:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:12px;background:rgb(48, 48, 48);border:1px solid rgba(255, 255, 255, 0.15);border-radius:2px;pointer-events:none;z-index:100;}#chatgpt-mermaid-\_r_10p\_ .flowchartTitleText{text-anchor:middle;font-size:18px;fill:rgb(237, 237, 237);}#chatgpt-mermaid-\_r_10p\_ rect.text{fill:none;stroke-width:0;}#chatgpt-mermaid-\_r_10p\_ .icon-shape,#chatgpt-mermaid-\_r_10p\_ .image-shape{background-color:rgb(0, 0, 0);text-align:center;}#chatgpt-mermaid-\_r_10p\_ .icon-shape p,#chatgpt-mermaid-\_r_10p\_ .image-shape p{background-color:rgb(0, 0, 0);padding:2px;}#chatgpt-mermaid-\_r_10p\_ .icon-shape .label rect,#chatgpt-mermaid-\_r_10p\_ .image-shape .label rect{opacity:0.5;background-color:rgb(0, 0, 0);fill:rgb(0, 0, 0);}#chatgpt-mermaid-\_r_10p\_ .label-icon{display:inline-block;height:1em;overflow:visible;vertical-align:-0.125em;}#chatgpt-mermaid-\_r_10p\_ .node .label-icon path{fill:currentColor;stroke:revert;stroke-width:revert;}#chatgpt-mermaid-\_r_10p\_ .node .neo-node{stroke:rgb(31, 78, 148);}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node rect,#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].cluster rect,#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node polygon{stroke:url(#chatgpt-mermaid-\_r_10p\_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].swimlane.cluster rect{filter:none;}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node path{stroke:url(#chatgpt-mermaid-\_r_10p\_-gradient);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node .outer-path{filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node .neo-line path{stroke:rgb(31, 78, 148);filter:none;}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node circle{stroke:url(#chatgpt-mermaid-\_r_10p\_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].node circle .state-start{fill:#000000;}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].icon-shape .icon{fill:url(#chatgpt-mermaid-\_r_10p\_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-\_r_10p\_ [data-look="neo"].icon-shape .icon-neo path{stroke:url(#chatgpt-mermaid-\_r_10p\_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-\_r_10p\_ .node text{font-size:14px;font-weight:600;letter-spacing:normal;fill:rgb(153, 206, 255);}#chatgpt-mermaid-\_r_10p\_ .edgeLabels text{font-size:13px;font-weight:600;letter-spacing:-0.08px;fill:rgb(153, 206, 255);}#chatgpt-mermaid-\_r_10p\_ .node tspan[font-weight="normal"],#chatgpt-mermaid-\_r_10p\_ .edgeLabels tspan[font-weight="normal"]{font-weight:600;}#chatgpt-mermaid-\_r_10p\_ .edgeLabel .label rect{opacity:1;rx:13px;ry:13px;fill:rgb(0, 14, 26);stroke:rgb(26, 62, 95);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .node rect,#chatgpt-mermaid-\_r_10p\_ .node circle,#chatgpt-mermaid-\_r_10p\_ .node ellipse,#chatgpt-mermaid-\_r_10p\_ .node polygon,#chatgpt-mermaid-\_r_10p\_ .node path{fill:rgb(0, 40, 77);stroke:rgba(255, 255, 255, 0.1);stroke-width:1px;}#chatgpt-mermaid-\_r_10p\_ .node rect{rx:16px;ry:16px;}#chatgpt-mermaid-\_r_10p\_ .mermaid-decision .label-container{fill:rgb(0, 14, 26);stroke:rgb(26, 62, 95);stroke-dasharray:2,2;}#chatgpt-mermaid-\_r_10p\_ .edgePaths .flowchart-link{stroke:rgb(175, 175, 175);stroke-width:1px;stroke-linecap:round;stroke-linejoin:round;}#chatgpt-mermaid-\_r_10p\_ .marker{fill:rgb(175, 175, 175);stroke:rgb(175, 175, 175);}#chatgpt-mermaid-\_r_10p\_ :root{--mermaid-font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";}Security Event Sources /Attack SimulatorEvent Ingestion APIEvent Validation &ProcessingDetection EngineRule-Based DetectionML Anomaly DetectionAlert EnrichmentMITRE ATT&CK MappingAlert CorrelationIncident ManagementSOC Analyst InvestigationAI SOC CopilotSOAR PlaybooksApproval WorkflowSandboxed Response ActionsAudit Trail & SLA MonitoringSOC DashboardReact FrontendSQL DatabaseQdrant Vector Database

## 🔄 How the System Works

1. Event Ingestion: Security events are received through backend APIs or the attack simulation module.
2. Event Processing: Incoming events are validated and processed.
3. Threat Detection: Detection rules and anomaly analysis identify suspicious activity.
4. Alert Generation: Detected events are converted into security alerts.
5. Threat Enrichment: Alerts receive contextual information, including MITRE ATT&CK mappings.
6. Alert Correlation: Related alerts are retrieved and correlated to support incident investigation.
7. Incident Investigation: SOC analysts investigate alerts and review associated evidence.
8. AI Assistance: SOC Copilot provides summaries, explanations and suggested next steps.
9. Incident Response: SOAR-style playbooks demonstrate response actions and approval workflows.
10. Monitoring & Reporting: Audit logs, SLA tracking and reports support operational visibility.

## 🧰 Technical Stack

| Category                | Technology             | Purpose                             |
| ----------------------- | ---------------------- | ----------------------------------- |
| Programming Language    | Python 3.12+           | Backend development                 |
| Backend Framework       | FastAPI                | REST APIs and application services  |
| Frontend Framework      | React 19               | User interface                      |
| Frontend Language       | TypeScript             | Type-safe development               |
| Build Tool              | Vite                   | Frontend development and bundling   |
| Styling                 | Tailwind CSS           | Responsive UI                       |
| Database                | SQLite / PostgreSQL    | Persistent application data         |
| ORM                     | SQLAlchemy 2           | Database operations                 |
| Migrations              | Alembic                | Database schema management          |
| Machine Learning        | Scikit-learn           | Anomaly detection                   |
| Numerical Computing     | NumPy                  | Numerical operations                |
| Vector Database         | Qdrant                 | Similarity search and retrieval     |
| Authentication          | JWT, bcrypt            | Authentication and password hashing |
| Real-Time Communication | WebSockets             | Live dashboard updates              |
| Data Visualization      | Recharts               | Charts and analytics                |
| Mapping                 | Leaflet, TopoJSON      | Threat-map visualization            |
| Testing                 | Pytest, HTTPX          | Backend testing                     |
| Containerization        | Docker, Docker Compose | Service deployment                  |

## 🧠 Machine Learning & AI Components

The project integrates machine-learning and AI-assisted capabilities into SOC workflows.

### Anomaly Detection

Uses Scikit-learn-based anomaly analysis to identify unusual login behavior and suspicious activity.

### Vector Similarity Search

Qdrant supports retrieval of similar alerts and historical cases based on vector similarity.

### SOC Copilot

Provides AI-assisted investigation, incident summaries, risk explanations and recommended next steps.

### Threat Mapping

Uses MITRE ATT&CK context to help analysts understand possible adversary techniques and attack behavior.

### Risk Scoring

Combines security context and detection information to support alert prioritization.

## 🧩 Core Application Modules

| Module              | Responsibility                            |
| ------------------- | ----------------------------------------- |
| Authentication      | Login, authentication and access control  |
| Event Ingestion     | Receiving and validating security events  |
| Detection Engine    | Rule-based detection and anomaly analysis |
| Alert Management    | Alert creation, assignment and triage     |
| Threat Intelligence | IOC enrichment and threat context         |
| MITRE Mapper        | ATT&CK technique mapping                  |
| Correlation Engine  | Identifying related security events       |
| Vector Store        | Similarity-based case retrieval           |
| SOC Copilot         | AI-assisted investigation                 |
| Incident Management | Investigation and incident lifecycle      |
| SOAR Engine         | Playbooks and response automation         |
| Response Centre     | Approval and containment workflows        |
| Audit Service       | Audit logging and integrity verification  |
| SLA Service         | SLA tracking and breach monitoring        |
| WebSocket Service   | Real-time communication                   |
| Reporting           | Executive and compliance reporting        |

## 📁 Project Structure

```
soc-command-centre/
│
├── backend/
│   ├── app/
│   │   ├── api/                 # FastAPI API routes
│   │   ├── core/                # Configuration and security
│   │   ├── db/                  # Database configuration
│   │   ├── models/              # Database models
│   │   ├── schemas/             # Pydantic schemas
│   │   ├── services/            # Business logic and security services
│   │   ├── websocket/           # Real-time communication
│   │   └── main.py              # Backend entry point
│   │
│   ├── data/                    # Reference data
│   ├── migrations/              # Database migrations
│   ├── scripts/                 # Simulation scripts
│   ├── tests/                   # Automated tests
│   ├── requirements.txt
│   ├── seed.py
│   └── .env.example
│
├── frontend/
│   ├── src/
│   │   ├── components/          # Reusable UI components
│   │   ├── hooks/               # React hooks
│   │   ├── lib/                 # API clients and utilities
│   │   ├── pages/               # Application pages
│   │   ├── App.tsx
│   │   └── main.tsx
│   │
│   ├── package.json
│   └── .env.example
│
├── docs/                        # Project documentation
├── docker-compose.yml
├── setup_mac.sh
├── start_mac.sh
└── README.md
```

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.12+
- Node.js 20+
- npm
- Git
- VS Code or another code editor

Optional:

- Docker Desktop
- Qdrant server
- PostgreSQL
- External LLM API credentials

### 1. Clone the Repository

```
git clone https://github.com/YOUR_USERNAME/soc-command-centre.git

cd soc-command-centre
```

### 2. Backend Setup

```
cd backend

python3.12 -m venv venv

source venv/bin/activate

python -m pip install --upgrade pip

pip install -r requirements.txt
```

Create the environment configuration:

```
cp .env.example .env
```

### 3. Initialize the Database

```
python seed.py
```

This initializes the database and creates demonstration records and accounts.

### 4. Start the Backend Server

```
uvicorn app.main:app --reload --port 8000
```

Backend API:

```
http://localhost:8000
```

Swagger API documentation:

```
http://localhost:8000/docs
```

Health check:

```
http://localhost:8000/api/health
```

### 5. Frontend Setup

Open a new terminal:

```
cd frontend

cp .env.example .env

npm install

npm run dev
```

Open the application:

```
http://localhost:5173
```

### 6. macOS Quick Setup

The repository also includes setup scripts:

```
bash setup_mac.sh

bash start_mac.sh
```

Use these scripts as an alternative to the manual setup after reviewing their configuration.

## 🐳 Docker Deployment

Start PostgreSQL and Qdrant:

```
docker compose up -d postgres qdrant
```

Start the full application:

```
docker compose --profile full up --build
```

Stop the services:

```
docker compose --profile full down
```

## 🔑 Demo Login Credentials

The seeded demonstration environment provides three access levels.

Demo Password: `Demo@1234`

| Role            | Email                    | Permissions                         |
| --------------- | ------------------------ | ----------------------------------- |
| Analyst         | analyst\@socplatform.io  | Alert triage and investigation      |
| On-Call Analyst | analyst2\@socplatform.io | Analyst workflows                   |
| Manager         | manager\@socplatform.io  | Operational oversight and approvals |
| Admin           | admin\@socplatform.io    | User and platform administration    |

> ⚠️ These credentials are for local demonstration only. Never use default demo credentials in production.

## 🔌 Event Ingestion API

The backend provides a security event ingestion endpoint:

```
POST /api/events/ingest
```

Example request:

```
curl -X POST http://localhost:8000/api/events/ingest \
-H "Content-Type: application/json" \
-H "X-Ingest-Key: YOUR_INGEST_API_KEY" \
-d '{
  "event_type": "authentication_failure",
  "source": "demo-forwarder"
}'
```

Refer to the Swagger documentation for the exact request schema and supported fields.

## 📈 Testing

Run backend tests:

```
cd backend

source venv/bin/activate

pytest -q
```

Run frontend linting:

```
cd frontend

npm run lint
```

Build the frontend:

```
npm run build
```

## 🔐 Security Considerations

- Attack scenarios use fictional and simulated security events.
- Response actions are sandboxed application-level demonstrations.
- Threat-map locations are approximate and should not be treated as precise attribution.
- AI-generated recommendations require analyst verification.
- External integrations require secure configuration.
- Production deployment requires additional security testing and hardening.
- Never commit API keys, credentials, private logs or sensitive information.

## 🚀 Future Enhancements

- Integration with additional SIEM platforms.
- Advanced threat-intelligence integrations.
- Improved ML model validation and anomaly detection.
- More advanced threat correlation and attack graph analysis.
- Extended SOAR integrations with explicit approval controls.
- Enhanced real-time monitoring and alert prioritization.
- More automated security testing.
- Improved deployment, monitoring and observability.
- Production-grade secrets management and access auditing.

## 🎓 Learning Outcomes

This project demonstrates practical implementation and understanding of:

- Security Operations Centre architecture.
- SIEM and SOAR concepts.
- Security event ingestion and detection engineering.
- Machine Learning for cybersecurity.
- Anomaly detection and threat analysis.
- MITRE ATT&CK framework.
- NIST incident response concepts.
- Vector databases and similarity search.
- REST API and WebSocket development.
- Role-Based Access Control (RBAC).
- Database management and migrations.
- Full-stack application development.

## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork this repository.
2. Create a feature branch.
3. Commit your changes.
4. Push your branch.
5. Submit a Pull Request.

Please include appropriate testing and documentation with contributions.

## 📜 License

This project is currently intended for educational and research purposes. Add an appropriate open-source license if you wish to permit public reuse and redistribution.

## 👨‍💻 Author

YOUR NAME

B.Tech | Cybersecurity

- GitHub: [YOUR_USERNAME](https://github.com/YOUR_USERNAME?utm_source=chatgpt.com)
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/YOUR_PROFILE/?utm_source=chatgpt.com)

Before publishing: Replace `YOUR_USERNAME`, `YOUR NAME`, and LinkedIn placeholders. Verify the demo credentials, scripts, API fields and Docker services against your actual repository configuration.
