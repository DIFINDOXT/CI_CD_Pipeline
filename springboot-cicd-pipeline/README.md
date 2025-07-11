# Spring Boot CI/CD Pipeline Project

This project demonstrates a comprehensive CI/CD pipeline setup using Jenkins, Docker, Maven, SonarQube, and ArgoCD for a Spring Boot application.

## 🚧 Project Status: Paused Due to AWS Billing Constraints

This project was initiated to gain hands-on experience with real-world CI/CD workflows. While significant progress was made, it has been **temporarily paused due to AWS billing concerns (~₹200 on EC2 t2.xlarge)**. The project will resume once I have job stability or access to cloud credits.

---

## ✅ Successfully Completed Components

- ✅ **Jenkins Pipeline Setup**: Full CI pipeline configured with GitHub SCM integration
- ✅ **Docker Integration**: Custom Docker agent image created and pushed to DockerHub
- ✅ **Maven Build Process**: Spring Boot application building successfully through Jenkins
- ✅ **GitHub Integration**: Automatic triggering via SCM polling and webhooks
- ✅ **Credentials Management**: Secure handling of DockerHub, GitHub, and SonarQube credentials
- ✅ **Infrastructure Setup**: EC2 instance configured with Jenkins, Docker, and required tools
- ✅ **Jenkinsfile Configuration**: Multi-stage pipeline with proper error handling

---

## ❌ Components in Progress (Paused)

- ❌ **SonarQube Analysis**: Connection timeout issues due to Java plugin mismatch
- ❌ **ArgoCD Deployment**: Operator installation completed, but UI login authentication failed
- ❌ **Slack Notifications**: Webhook integration planned but not implemented
- ❌ **Production Deployment**: Final Kubernetes deployment pending ArgoCD resolution

---

## 🛠️ Technology Stack

| Component | Technology | Purpose |
|-----------|------------|---------|
| **CI/CD** | Jenkins | Continuous Integration orchestration |
| **SCM** | GitHub | Source code management and triggering |
| **Build Tool** | Maven | Java application building and dependency management |
| **Containerization** | Docker | Application packaging and deployment |
| **Code Quality** | SonarQube | Static code analysis and quality gates |
| **CD** | ArgoCD | Kubernetes-native continuous deployment |
| **Infrastructure** | AWS EC2 | Cloud hosting environment |
| **Orchestration** | Minikube | Local Kubernetes cluster for testing |

---

## 📂 Repository Structure

```
springboot-app-manifests/     	  # Kubernetes deployment files
│   ├── deployment.yml
│   └── service.yml
springboot-cicd-pipeline/
├── src/                          # Spring Boot application source
├── Dockerfile                    # Container definition
├── Jenkinsfile                   # CI/CD pipeline configuration
├── pom.xml                       # Maven build configuration
├── README.md                     # Project documentation
├── challenges_faced.md           # Detailed issue log
└── trainer-assets/               # Screenshots, notes, diagrams```

---

## 🎯 Key Learning Outcomes

### Technical Skills Developed:
- Jenkins pipeline automation and troubleshooting
- Docker containerization and registry management
- Maven build optimization and dependency resolution
- Kubernetes manifest creation and deployment strategies
- AWS EC2 instance management and cost optimization
- Git workflow integration with CI/CD systems

### Problem-Solving Experience:
- Java version compatibility across different tools
- Disk space management in CI environments
- Network connectivity troubleshooting
- Security credential management
- Cost-effective cloud resource utilization

---

## 🔄 Next Steps (Post-Resumption)

1. **Complete SonarQube Integration**: Resolve Java plugin compatibility issues
2. **Fix ArgoCD Authentication**: Debug operator deployment and access credentials
3. **Implement Monitoring**: Add Slack notifications and pipeline metrics
4. **Optimize Infrastructure**: Migrate to cost-effective alternatives (GitHub Actions, GitLab CI)
5. **Add Security Scanning**: Integrate container security scanning tools
6. **Documentation Enhancement**: Add architecture diagrams and detailed setup guides

---

## 💡 Project Architecture

```
GitHub → Jenkins → Maven Build → Docker Build → DockerHub → ArgoCD → Kubernetes
    ↓        ↓                                      ↓
  Webhook  SonarQube                            Slack Notification
```

---

## 🙏 Acknowledgements

- **Trainer**: Abhishek Veeramalla (Youtube)
- **Learning Platform**: Hands-on DevOps project implementation
- **Community Support**: Docker Documentation, Jenkins Documentation,
- **AI Tools Used**: ChatGpt, Cursor.
---

## 📞 Contact & Future Updates

This project demonstrates practical DevOps skills and real-world problem-solving abilities. For detailed technical discussions or project continuation updates, please refer to the challenges_faced.md and interview preparation materials.

**Note**: All configuration files, logs, and detailed setup instructions are preserved for future reference and project continuation.
