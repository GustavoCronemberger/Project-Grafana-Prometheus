# 📊 Projeto DevOps: API Fórum com Monitoramento Avançado

Este repositório contém o código-fonte de uma API RESTful para um Fórum, acompanhada de uma infraestrutura completa de conteinerização e monitoramento contínuo.

O objetivo do projeto é demonstrar a implementação de métricas de observabilidade, alertas automatizados e dashboards interativos para acompanhar a saúde e o desempenho da aplicação em tempo real.

## 🚀 Tecnologias e Ferramentas Utilizadas

**Aplicação e Banco de Dados:**
* **Java & Spring Boot:** Desenvolvimento da API REST.
* **MySQL:** Banco de dados relacional para persistência das informações.
* **Redis:** Banco de dados em memória utilizado para cache.
* **Nginx:** Servidor web atuando como proxy reverso.

**Infraestrutura e Observabilidade (DevOps):**
* **Docker & Docker Compose:** Orquestração e conteinerização de todos os serviços.
* **Prometheus:** Coleta e armazenamento de métricas (Time Series Database).
* **Grafana:** Criação de dashboards visuais interativos para análise dos dados.
* **Alertmanager & Slack:** Gerenciamento, roteamento de alertas gerados pelo Prometheus e envio de notificações em tempo real através de Incoming Webhooks.

## ⚙️ Como executar o projeto localmente

**Passo a passo:**
1. Clone este repositório para a sua máquina local:
   ```bash
   git clone [https://github.com/GustavoCronemberger/Project-Grafana-Prometheus.git](https://github.com/GustavoCronemberger/Project-Grafana-Prometheus.git)
   ```
2. Acesse a pasta do projeto via terminal:
   ```bash
   cd conteudo_01
   ```
3. Suba toda a infraestrutura utilizando o Docker Compose:
   ```bash
   docker compose up -d
   ```

## 🌐 Acessando os Serviços

Após os containers subirem, você pode acessar os serviços através dos seguintes endereços no seu navegador:

* **API Fórum:** `http://localhost:8080`
* **Prometheus (Métricas):** `http://localhost:9090`
* **Grafana (Dashboards):** `http://localhost:3000`

*(Nota: O login padrão inicial do Grafana costuma ser `admin` para usuário e `admin` para senha).*

## 📈 O que está sendo monitorado?

* **Métricas da JVM:** Uso de memória (Heap), tempo de Garbage Collection, etc.
* **Métricas HTTP:** Taxa de requisições, tempo de resposta (latência) e códigos de status (Erros 400, 500, etc).
* **Métricas de Sistema:** Consumo de CPU e recursos do servidor.
* **Alertas:** Regras configuradas para avisar quando a API atinge níveis críticos de erro ou de consumo de recursos.

---
*Desenvolvido durante os estudos de práticas DevOps e Monitoramento.*