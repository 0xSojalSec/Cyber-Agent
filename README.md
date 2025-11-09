<div align="center">
  <img src="public/hackgpt-logo.png" alt="HackGPT Enterprise Logo" width="400" height="auto">
  
  <h1>🚀 HackGPT Enterprise</h1>
  <h3>AI-Powered Penetration Testing Platform</h3>
  
  <p>
    <img src="https://img.shields.io/badge/Python-3.8+-blue.svg" alt="Python 3.8+">
    <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-orange.svg" alt="Multi-Platform">
    <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="MIT License">
    <img src="https://img.shields.io/badge/AI-GPT%20%7C%20Local%20LLM%20%7C%20ML-purple.svg" alt="AI Powered">
  </p>
  <p>
    <img src="https://img.shields.io/badge/Architecture-Microservices-red.svg" alt="Microservices">
    <img src="https://img.shields.io/badge/Cloud-Docker%20%7C%20Kubernetes-lightblue.svg" alt="Cloud Native">
    <img src="https://img.shields.io/badge/Version-2.0.0-success.svg" alt="Version 2.0.0">
    <img src="https://img.shields.io/badge/Status-Production%20Ready-brightgreen.svg" alt="Production Ready">
  </p>
</div>

**HackGPT Enterprise** is a production-ready, cloud-native AI-powered penetration testing platform designed for enterprise security teams. It combines advanced AI, machine learning, microservices architecture, and comprehensive security frameworks to deliver professional-grade cybersecurity assessments.

**Created by [Yashab Alam](https://github.com/0xSojalSec), Founder & CEO of [ZehraSec](https://www.zehrasec.com)**

> 💰 **Support the Project**: [Donate to HackGPT Development](DONATE.md) | Help us build the future of AI-powered penetration testing!

## 🏢 Enterprise Features

### 🤖 Advanced AI Engine
- **Multi-Model Support**: OpenAI GPT-4, Local LLM (Ollama), TensorFlow, PyTorch
- **Machine Learning**: Pattern recognition, anomaly detection, behavioral analysis
- **Zero-Day Detection**: ML-powered vulnerability discovery and correlation
- **Risk Intelligence**: CVSS scoring, impact assessment, exploit prioritization
- **Automated Reporting**: Executive summaries, technical details, compliance mapping

### 🛡️ Enterprise Security & Compliance
- **Authentication**: RBAC + LDAP/Active Directory integration
- **Authorization**: Role-based permissions (Admin, Lead, Senior, Pentester, Analyst)
- **Compliance**: OWASP, NIST, ISO27001, SOC2, PCI-DSS frameworks
- **Audit Logging**: Comprehensive activity tracking and forensics
- **Data Protection**: AES-256-GCM encryption, JWT tokens, secure sessions

### 🏗️ Cloud-Native Architecture
- **Microservices**: Docker containers with Kubernetes orchestration
- **Service Discovery**: Consul-based service registry
- **Load Balancing**: Nginx reverse proxy with auto-scaling
- **Multi-Cloud**: AWS, Azure, GCP deployment support
- **High Availability**: Circuit breakers, health checks, failover

### ⚡ Performance & Scalability
- **Parallel Processing**: Celery-based distributed task execution
- **Multi-Layer Caching**: Redis + memory caching with TTL management
- **Database**: PostgreSQL with connection pooling and replication
- **Real-Time**: WebSocket dashboards with live updates
- **Auto-Scaling**: Worker pools adapt to workload demands

### 📊 Enterprise Reporting & Analytics
- **Dynamic Reports**: HTML, PDF, JSON, XML, CSV export formats
- **Real-Time Dashboards**: Prometheus + Grafana monitoring stack
- **Log Analytics**: ELK stack (Elasticsearch + Kibana) integration
- **Executive Summaries**: AI-generated business impact assessments
- **Compliance Reports**: Framework-specific compliance documentation

## 🚀 Quick Start

### Prerequisites
- **Operating System**: Linux (Ubuntu/Debian/RHEL/CentOS), macOS, or Windows WSL2
- **Python**: 3.8+ with pip and virtual environment support
- **Docker**: For containerized deployment (recommended)
- **Resources**: Minimum 4GB RAM, 20GB disk space

### Enterprise Installation

```bash
# Clone the repository
git clone https://github.com/0xSojalSec/HackGPT.git
cd HackGPT

# Run enterprise installer (sets up all services)
chmod +x install.sh
./install.sh

# Configure environment
cp .env.example .env
# Edit .env with your API keys and settings
nano .env

# Verify installation
python3 test_installation.py
```

### Deployment Options

#### 1. Standalone Enterprise Mode
```bash
# Activate virtual environment
source venv/bin/activate

# Run enterprise application
python3 hackgpt_v2.py
```

#### 2. API Server Mode
```bash
# Start REST API server
python3 hackgpt_v2.py --api

# API available at: http://localhost:8000
# Health check: http://localhost:8000/api/health
```

#### 3. Web Dashboard Mode
```bash
# Start web dashboard
python3 hackgpt_v2.py --web

# Dashboard available at: http://localhost:8080
```

#### 4. Full Enterprise Stack (Recommended)
```bash
# Deploy complete microservices stack
docker-compose up -d

# Services:
# - API Server: http://localhost:8000
# - Web Dashboard: http://localhost:8080  
# - Monitoring: http://localhost:9090 (Prometheus)
# - Analytics: http://localhost:3000 (Grafana)
# - Logs: http://localhost:5601 (Kibana)
```

#### 5. Direct Assessment Mode
```bash
# Run immediate assessment
python3 hackgpt_v2.py \
  --target example.com \
  --scope "Web application and API" \
  --auth-key "ENTERPRISE-2025-AUTH" \
  --assessment-type black-box \
  --compliance OWASP
```

## 🏗️ Enterprise Architecture

### Core Components

```mermaid
graph TD
    A[Load Balancer/Nginx] --> B[HackGPT API Gateway]
    B --> C[Authentication Service]
    B --> D[AI Engine Service] 
    B --> E[Exploitation Service]
    B --> F[Reporting Service]
    
    C --> G[LDAP/AD]
    D --> H[OpenAI API]
    D --> I[Local LLM]
    D --> J[ML Models]
    
    E --> K[Parallel Processor]
    F --> L[Report Generator]
    
    K --> M[Celery Workers]
    M --> N[Redis Queue]
    
    B --> O[PostgreSQL]
    B --> P[Redis Cache]
    
    Q[Prometheus] --> R[Grafana]
    S[Elasticsearch] --> T[Kibana]
```

### Service Stack

| Service | Purpose | Port | Technology |
|---------|---------|------|------------|
| **hackgpt-app** | Main application | 8000, 8080 | Python/Flask |
| **hackgpt-worker** | Background tasks | - | Celery |
| **hackgpt-database** | Data persistence | 5432 | PostgreSQL 15 |
| **hackgpt-redis** | Cache & queues | 6379 | Redis 7 |
| **prometheus** | Metrics collection | 9090 | Prometheus |
| **grafana** | Monitoring dashboard | 3000 | Grafana |
| **elasticsearch** | Log aggregation | 9200 | Elasticsearch |
| **kibana** | Log visualization | 5601 | Kibana |
| **consul** | Service discovery | 8500 | Consul |
| **nginx** | Load balancer | 80, 443 | Nginx |

## 🔧 Configuration

### Enterprise Configuration (`config.ini`)

The configuration file supports 200+ options across multiple categories:

```ini
[app]
debug = false
environment = production
max_sessions = 100

[database]
url = postgresql://hackgpt:hackgpt123@localhost:5432/hackgpt
pool_size = 20
backup_enabled = true

[ai]
openai_api_key = your_key_here
openai_model = gpt-4
enable_local_fallback = true
confidence_threshold = 0.8

[security]
secret_key = your_secret_here
jwt_algorithm = HS256
rate_limit_enabled = true

[ldap]
server = ldaps://your-ldap-server.com:636
bind_dn = cn=admin,dc=example,dc=com

[compliance]
frameworks = OWASP,NIST,ISO27001,SOC2,PCI-DSS
auto_compliance_check = true

[cloud]
docker_host = unix:///var/run/docker.sock
service_registry_backend = consul
```

### Environment Variables (`.env`)

Over 100 environment variables for enterprise deployment:

```bash
# Core Services
DATABASE_URL=postgresql://hackgpt:hackgpt123@localhost:5432/hackgpt
REDIS_URL=redis://localhost:6379/0
OPENAI_API_KEY=your_openai_api_key

# Security
SECRET_KEY=your_secret_key
JWT_SECRET_KEY=your_jwt_secret
LDAP_SERVER=ldaps://your-ldap.com:636

# Cloud Providers
AWS_ACCESS_KEY_ID=your_aws_key
AZURE_SUBSCRIPTION_ID=your_azure_id
GCP_PROJECT_ID=your_gcp_project

# Monitoring
PROMETHEUS_ENDPOINT=http://localhost:9090
GRAFANA_API_KEY=your_grafana_key
ELASTICSEARCH_ENDPOINT=http://localhost:9200
```

## 🎯 Enterprise Penetration Testing

### Enhanced 6-Phase Methodology

#### Phase 1: Intelligence Gathering & Reconnaissance
**Enterprise Features**:
- AI-powered OSINT automation
- Multi-source data aggregation
- Threat intelligence correlation
- Cloud asset discovery (AWS, Azure, GCP)
- **Tools**: theHarvester, Amass, Subfinder, Shodan API

#### Phase 2: Advanced Scanning & Enumeration  
**Enterprise Features**:
- Parallel distributed scanning
- Service fingerprinting with ML classification
- Vulnerability correlation across assets
- Zero-day pattern detection
- **Tools**: Nmap, Masscan, Nuclei, HTTPx, Naabu

#### Phase 3: Vulnerability Assessment
**Enterprise Features**:
- CVSS v3.1 automated scoring
- Business impact analysis
- Exploit availability assessment  
- Compliance framework mapping
- **Tools**: OpenVAS, Nexpose integration, custom scanners

#### Phase 4: Exploitation & Post-Exploitation
**Enterprise Features**:
- Safe-mode exploitation with approval workflows
- Privilege escalation enumeration
- Lateral movement mapping
- Data exfiltration simulation
- **Tools**: Metasploit, CrackMapExec, BloodHound, custom exploits

#### Phase 5: Enterprise Reporting & Analytics
**Enterprise Features**:
- Executive dashboard with KPIs
- Technical vulnerability details
- Compliance gap analysis
- Risk prioritization matrix
- **Outputs**: HTML, PDF, JSON, XML, compliance reports

#### Phase 6: Verification & Retesting
**Enterprise Features**:
- Automated remediation verification
- Regression testing for fixes
- Continuous security monitoring
- Trend analysis and metrics
- **Features**: Scheduled retests, delta reporting

## 📊 Enterprise Interfaces

### 1. Command Line Interface (CLI)
```bash
# Interactive enterprise mode
python3 hackgpt_v2.py

# Available options:
# 1. Full Enterprise Pentest (All 6 Phases)
# 2. Run Specific Phase
# 3. Custom Assessment Workflow
# 4. View Reports & Analytics
# 5. Real-time Dashboard
# 6. User & Permission Management
# 7. System Configuration
# 8. Compliance Management
# 9. Cloud & Container Management
# 10. AI Engine Configuration
```

### 2. REST API Server
```bash
# Start API server
python3 hackgpt_v2.py --api

# Available endpoints:
# GET  /api/health - Health check
# POST /api/pentest/start - Start assessment
# GET  /api/sessions - List sessions
# GET  /api/reports/{id} - Get report
# POST /api/users - User management
# GET  /api/compliance - Compliance status
```

### 3. Web Dashboard
```bash
# Start web dashboard
python3 hackgpt_v2.py --web

# Features:
# - Real-time assessment monitoring
# - Interactive vulnerability management
# - Executive summary dashboard
# - User and role management
# - System configuration
# - Compliance reporting
```

### 4. Voice Commands (Enterprise)
```bash
# Voice command mode
python3 hackgpt_v2.py --voice

# Supported commands:
# "Start enterprise assessment of example.com"
# "Show compliance dashboard"
# "Generate executive report"
# "Scale worker pool to 10"
```

## 🔐 Enterprise Security

### Authentication & Authorization
- **Multi-Factor Authentication**: LDAP/AD + JWT tokens
- **Role-Based Access Control**: Granular permissions matrix
- **Session Management**: Secure session handling with timeout
- **API Security**: Rate limiting, CORS, input validation

### Data Protection
- **Encryption**: AES-256-GCM for data at rest
- **Transport Security**: TLS 1.3 for data in transit  
- **Key Management**: Automated key rotation
- **Audit Logging**: Comprehensive activity tracking

### Compliance Frameworks
| Framework | Coverage | Reports | Automation |
|-----------|----------|---------|------------|
| **OWASP Top 10** | ✅ Full | ✅ Yes | ✅ Automated |
| **NIST Cybersecurity Framework** | ✅ Full | ✅ Yes | ✅ Automated |
| **ISO 27001** | ✅ Partial | ✅ Yes | ✅ Semi-automated |
| **SOC 2** | ✅ Partial | ✅ Yes | ✅ Semi-automated |
| **PCI DSS** | ✅ Partial | ✅ Yes | ✅ Manual |

## 📈 Monitoring & Analytics

### Real-Time Monitoring
- **System Metrics**: CPU, memory, disk, network utilization
- **Application Metrics**: Request rates, response times, error rates
- **Security Metrics**: Vulnerability counts, risk scores, remediation rates
- **Business Metrics**: Assessment coverage, compliance scores

### Alerting
- **Email Alerts**: Critical vulnerabilities, system issues
- **Slack Integration**: Real-time notifications to security teams
- **Webhook Support**: Custom integrations with SIEM systems
- **Dashboard Alerts**: Visual indicators and notifications

### Analytics Dashboard
```bash
# Access Grafana dashboard
http://localhost:3000
# Login: admin / hackgpt123

# Pre-configured dashboards:
# - HackGPT System Overview
# - Assessment Performance Metrics  
# - Vulnerability Trend Analysis
# - User Activity Dashboard
# - Compliance Status Overview
```

## 🛠️ Advanced Usage

### Custom AI Models
```python
# Configure custom AI endpoints
config['ai']['custom_model_endpoint'] = 'http://your-llm:8000'
config['ai']['model_type'] = 'custom'
```

### Custom Compliance Frameworks
```python
# Add custom compliance framework
from security.compliance import ComplianceFrameworkMapper

mapper = ComplianceFrameworkMapper()
mapper.add_framework('CUSTOM', {
    'sql_injection': 'SEC-01',
    'xss': 'SEC-02',
    # ... custom mappings
})
```

### Kubernetes Deployment
```yaml
# Deploy to Kubernetes cluster
kubectl apply -f k8s/
```

### Multi-Cloud Deployment
```bash
# Deploy to AWS
python3 hackgpt_v2.py --deploy aws

# Deploy to Azure  
python3 hackgpt_v2.py --deploy azure

# Deploy to GCP
python3 hackgpt_v2.py --deploy gcp
```

## 🧪 Testing & Development

### Running Tests
```bash
# Unit tests
pytest tests/unit/

# Integration tests  
pytest tests/integration/

# End-to-end tests
pytest tests/e2e/

# Security tests
bandit -r .
safety check
```

### Development Setup
```bash
# Install development dependencies
pip install -r requirements-dev.txt

# Pre-commit hooks
pre-commit install

# Code formatting
black .
flake8 .
mypy .
```

## 📦 Enterprise Deployment

### Docker Swarm
```bash
# Initialize swarm
docker swarm init

# Deploy stack
docker stack deploy -c docker-compose.yml hackgpt
```

### Kubernetes
```bash
# Create namespace
kubectl create namespace hackgpt

# Deploy applications
kubectl apply -f k8s/

# Scale workers
kubectl scale deployment hackgpt-worker --replicas=10
```

### Cloud Platforms

#### AWS Deployment
```bash
# ECS deployment
aws ecs create-cluster --cluster-name hackgpt
aws ecs create-service --service-name hackgpt-api
```

#### Azure Deployment  
```bash
# ACI deployment
az container create --resource-group hackgpt --name hackgpt-api
```

#### GCP Deployment
```bash
# GKE deployment
gcloud container clusters create hackgpt-cluster
kubectl apply -f k8s/
```

## 🔧 Troubleshooting

### Common Enterprise Issues

#### Database Connection Issues
```bash
# Check PostgreSQL status
systemctl status postgresql
docker logs hackgpt-database

# Test connection
python3 -c "from database import get_db_manager; print(get_db_manager().test_connection())"
```

#### Redis Cache Issues
```bash
# Check Redis status
redis-cli ping
docker logs hackgpt-redis

# Clear cache
redis-cli FLUSHALL
```

#### AI Engine Issues
```bash
# Test OpenAI connectivity
python3 -c "import openai; print(openai.Model.list())"

# Check local LLM
ollama list
ollama run llama2:7b
```

#### Worker Pool Issues
```bash
# Check Celery workers
celery -A performance.parallel_processor inspect active

# Restart workers
docker-compose restart hackgpt-worker
```

### Performance Optimization
```bash
# Database optimization
python3 -c "from database import optimize_database; optimize_database()"

# Cache warming
python3 -c "from performance.cache_manager import warm_cache; warm_cache()"

# Worker scaling
docker-compose up --scale hackgpt-worker=10
```



## 📊 Project Statistics

| Metric | Value |
|--------|-------|
| **Total Lines of Code** | 15,000+ |
| **Enterprise Dependencies** | 90+ |
| **Configuration Options** | 200+ |
| **Environment Variables** | 100+ |
| **Docker Services** | 12 |
| **Supported Compliance Frameworks** | 5 |
| **Penetration Testing Tools** | 50+ |
| **API Endpoints** | 25+ |
| **Deployment Platforms** | 6+ |

## 🗺️ Roadmap

### Version 2.1 (Q3 2025)
- [ ] Advanced threat hunting capabilities
- [ ] ML-based false positive reduction
- [ ] Integration with popular SIEM systems
- [ ] Mobile application for executives

### Version 2.2 (Q4 2025) 
- [ ] Automated penetration testing workflows
- [ ] Advanced cloud security assessments
- [ ] Integration with CI/CD pipelines
- [ ] Enhanced compliance reporting

### Version 3.0 (Q1 2026)
- [ ] Fully autonomous security assessments
- [ ] Advanced AI attack simulation
- [ ] Quantum-safe cryptography
- [ ] Next-generation threat detection


### Acknowledgments
- OpenAI for GPT-4 API access
- Ollama team for local LLM support
- Docker & Kubernetes communities
- Security research community
- Open source tool developers


**⚠️ IMPORTANT LEGAL NOTICE**

HackGPT Enterprise is designed for authorized security testing only:

- ✅ **Authorized Use**: Only use against systems you own or have explicit written permission
- ✅ **Compliance**: Follow all applicable laws, regulations, and industry standards
- ✅ **Responsible Disclosure**: Report vulnerabilities through proper channels
- ✅ **Documentation**: Maintain audit trails and documentation
- ❌ **Unauthorized Use**: Never use against systems without permission
- ❌ **Malicious Activity**: Not for criminal or malicious purposes

