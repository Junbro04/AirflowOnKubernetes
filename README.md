# Airflow on Kubernetes를 통한 AWS 클라우드 인프라 이상 탐지 시스템 구축

## 1. 기본 인프라 및 도구

### 1.1 Kubernetes (K8s)
- **Kubernetes 기초**: K8s의 기본 개념 (Pod, Node, Deployment, Service 등)
- **Kubernetes 클러스터 설정**: EKS (Elastic Kubernetes Service)에서 K8s 클러스터를 설정하는 방법
- **Kubernetes 관리 도구**: `kubectl` 사용법 및 Helm Charts
- **등**

### 1.2 Terraform
- **Terraform 기본**: Terraform의 기본 문법 및 구성 요소 (Provider, Resource, Module 등)
- **AWS Provider**: AWS 인프라를 설정하기 위한 Terraform AWS Provider 사용법
- **Infrastructure as Code (IaC)**: 코드로 인프라를 관리하고 배포하는 방법
- **등**

### 1.3 AWS 인프라
- **EKS (Elastic Kubernetes Service)**: Kubernetes 클러스터를 AWS에서 운영하기 위한 서비스
- **VPC (Virtual Private Cloud)**: VPC 설정 및 관리 (서브넷, 라우팅 테이블, 게이트웨이 등)
- **IAM (Identity and Access Management)**: 접근 권한 및 정책 설정
- **S3 (Simple Storage Service)**: 데이터 저장소로 사용
- **RDS (Relational Database Service)**: 데이터베이스 설정 및 관리
- **등**

## 2. Airflow

- **Airflow 기초**: Airflow의 기본 개념 (DAG, Operator, Task 등)
- **Airflow 설치 및 구성**: Kubernetes 환경에서 Airflow를 설치하고 구성하는 방법
- **Airflow Operator**: 다양한 AWS 서비스와 통합하기 위한 Airflow Operator (S3, RDS 등)
- **Airflow 관리 및 모니터링**: Airflow 웹 UI를 통한 관리 및 모니터링
- **등**

## 3. 데이터 파이프라인 및 처리

### 3.1 데이터 수집 및 전처리
- **데이터 수집**: AWS 서비스에서 데이터를 수집하는 방법 (CloudWatch, S3 등)
- **데이터 전처리**: 수집된 데이터를 정제하고 변환하는 방법
- **등**

### 3.2 이상 탐지 알고리즘
- **이상 탐지 개념**: 이상 탐지의 기본 개념 및 다양한 알고리즘 (예: 시계열 분석, 머신러닝)
- **모델 훈련**: 이상 탐지 모델을 훈련시키는 방법
- **모델 배포 및 운영**: 훈련된 모델을 배포하고 운영하는 방법
- **등**

## 4. 모니터링 및 로깅

- **Prometheus & Grafana**: 모니터링 도구 설정 및 대시보드 구성
- **ELK Stack**: Elasticsearch, Logstash, Kibana를 이용한 로깅 및 로그 분석
- **AWS CloudWatch**: AWS 서비스의 모니터링 및 로깅
- **등**

## 5. 보안 및 권한 관리

- **네트워크 보안**: VPC 보안 그룹 및 네트워크 ACL 설정
- **IAM**: 세분화된 IAM 역할 및 정책 설정
- **Kubernetes RBAC**: Kubernetes 내의 역할 기반 접근 제어 설정
- **등**

## 6. DevOps 및 CI/CD

- **CI/CD 파이프라인**: 코드 변경사항을 자동으로 배포하기 위한 파이프라인 구축 (Jenkins, GitLab CI/CD 등)
- **도커**: Docker를 이용한 애플리케이션 컨테이너화
- **Helm**: Helm 차트를 이용한 Kubernetes 애플리케이션 배포 및 관리
- **등**

## 7. 예제 시나리오

- **데이터 수집 DAG**: AWS CloudWatch에서 로그 데이터를 수집하여 S3에 저장하는 DAG
- **데이터 전처리 DAG**: S3에 저장된 데이터를 전처리하여 분석용 데이터로 변환하는 DAG
- **이상 탐지 DAG**: 전처리된 데이터를 이상 탐지 알고리즘에 적용하고 결과를 저장하는 DAG
- **등**
