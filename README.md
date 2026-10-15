<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:0B1220,50:0969DA,100:28C7FA&text=Mohammed%20Islam&fontColor=ffffff&fontSize=48&fontAlignY=39&desc=Cloud%20%7C%20DevOps%20%7C%20Infrastructure%20Automation&descAlignY=61&animation=fadeIn" width="100%" alt="Mohammed Islam — Cloud, DevOps and Infrastructure Automation" />

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=21&duration=2800&pause=850&color=36BCF7&center=true&vCenter=true&repeat=true&width=780&lines=Building+on+AWS+with+Terraform+%26+Docker;Deploying+containerised+apps+on+ECS+Fargate;Automating+deployments+with+GitHub+Actions;Learning+by+building+real+cloud+projects" alt="Animated introduction" /></a>

[![GitHub followers](https://img.shields.io/github/followers/mohammed-972?style=for-the-badge&logo=github&label=Followers&color=238636)](https://github.com/mohammed-972?tab=followers)
[![Profile views](https://komarev.com/ghpvc/?username=mohammed-972&style=for-the-badge&color=0969da)](https://github.com/mohammed-972)
[![Featured project](https://img.shields.io/badge/Featured_Project-ECS_Pomodoro-8250df?style=for-the-badge&logo=terraform&logoColor=white)](https://github.com/mohammed-972/terraform-ecs-pomodoro)

</div>

## About me

I'm developing my skills in **cloud engineering, DevOps and infrastructure automation** through hands-on projects. I enjoy taking an application from a local Docker build through to an automated AWS deployment, and learning how the networking, security and operational pieces fit together.

-  **Latest project:** [Terraform + AWS ECS Fargate Pomodoro deployment](https://github.com/mohammed-972/terraform-ecs-pomodoro)
-  **Currently working with:** AWS, Terraform, Docker, GitHub Actions, Linux and networking
-  **Learning more about:** CI/CD, observability, cloud security and reliability

##  Featured project — Terraform + ECS Pomodoro

<div align="center">

[![Open repository](https://img.shields.io/badge/VIEW_SOURCE_CODE-terraform--ecs--pomodoro-238636?style=for-the-badge&logo=github)](https://github.com/mohammed-972/terraform-ecs-pomodoro)
[![View app](https://img.shields.io/badge/APP_DEMO-Pomodoro_Timer-0969da?style=for-the-badge&logo=googlechrome&logoColor=white)](https://pomodoro.mohammedislam.uk)

</div>

I built and deployed a containerised **Pomodoro timer application** on **Amazon ECS Fargate**. The AWS infrastructure is provisioned with **Terraform**, and **GitHub Actions** automates the image build and infrastructure deployment workflows.

**Architecture at a glance**

```text
              Users
                │
          Route 53 + HTTPS
                │
         Application Load Balancer
                │
       ECS Fargate (private subnets)
                │
        Docker image from ECR

 GitHub Actions ── OIDC ──> AWS
      │                       │
      ├── Build + push to ECR │
      └── Terraform deploy ──┘

 VPC: 2 public + 2 private subnets
      Internet Gateway / NAT Gateway
```

**What I implemented**

- **Infrastructure as Code:** Modular Terraform for the VPC, security groups, ALB, ACM, Route 53, ECR, ECS and IAM.
- **Containerisation:** Nginx-served web app packaged as a Docker image and published to Amazon ECR.
- **Private application workloads:** ECS Fargate tasks in private subnets, reached through an internet-facing Application Load Balancer.
- **HTTPS and DNS:** Custom domain managed through Route 53 with an ACM certificate.
- **CI/CD:** GitHub Actions with AWS OIDC authentication (no long-lived AWS access keys in the workflow), image tagging with the Git commit SHA, plus separate deploy and destroy workflows.
- **Health checks:** A dedicated `/health` endpoint to verify application availability.

> **Interesting challenge:** A fresh environment needs the ECR repository before the application pipeline can push its first image. I documented a bootstrap step for that first deployment.

**Explore the implementation:** [Application](https://github.com/mohammed-972/terraform-ecs-pomodoro/tree/main/app) · [Terraform infrastructure](https://github.com/mohammed-972/terraform-ecs-pomodoro/tree/main/infra) · [GitHub Actions workflows](https://github.com/mohammed-972/terraform-ecs-pomodoro/tree/main/.github/workflows) · [Full project README](https://github.com/mohammed-972/terraform-ecs-pomodoro#readme)

##  Tools & technologies

<div align="center">

<img src="https://skillicons.dev/icons?i=aws,terraform,docker,githubactions,,bash,git,github" alt="AWS, Terraform, Docker, GitHub Actions, Linux, Bash, Git, GitHub, Nginx and VS Code" />

<br/><br/>

![Amazon ECS](https://img.shields.io/badge/Amazon_ECS-FF9900?style=flat-square&logo=amazonecs&logoColor=white)
![AWS Fargate](https://img.shields.io/badge/AWS_Fargate-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Amazon ECR](https://img.shields.io/badge/Amazon_ECR-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Amazon VPC](https://img.shields.io/badge/Amazon_VPC-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF4F8B?style=flat-square&logo=amazoncloudwatch&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

</div>

##  GitHub activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=mohammed-972&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="GitHub statistics" height="165" />
<img src="https://streak-stats.demolab.com?user=mohammed-972&theme=tokyonight&hide_border=true" alt="GitHub contribution streak" height="165" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=mohammed-972&theme=tokyo-night&hide_border=true&area=true" alt="GitHub activity graph" width="98%" />

</div>

##  Contributions in motion

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/mohammed-972/mohammed-972/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/mohammed-972/mohammed-972/output/github-contribution-grid-snake.svg" />
  <img alt="Animated contribution snake" src="https://raw.githubusercontent.com/mohammed-972/mohammed-972/output/github-contribution-grid-snake.svg" />
</picture>

<sub>Generated automatically by GitHub Actions. This animation appears after you add the workflow below and run it.</sub>

</div>

##  Connect & explore

<div align="center">

[![GitHub](https://img.shields.io/badge/Browse_my_repositories-181717?style=for-the-badge&logo=github)](https://github.com/mohammed-972?tab=repositories)
[![Project](https://img.shields.io/badge/See_my_latest_build-0969da?style=for-the-badge&logo=terraform&logoColor=white)](https://github.com/mohammed-972/terraform-ecs-pomodoro)

**Thanks for visiting!** 

<img src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=95&color=0:0B1220,50:0969DA,100:28C7FA" width="100%" alt="Decorative footer" />

</div>
