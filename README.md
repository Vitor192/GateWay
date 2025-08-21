# 🌐 API Gateway

Este projeto faz parte de uma arquitetura baseada em **Microsserviços**.  
O **Gateway** atua como ponto único de entrada, roteando e filtrando as requisições para os serviços internos, além de expor métricas e informações de saúde via **Spring Boot Actuator**.

---

## 📌 Tecnologias utilizadas
- **Java 17+**
- **Spring Boot**
- **Spring Cloud Gateway**
- **Spring Boot Actuator**
- **Gradle**

---

## ⚙️ Funcionalidades
- Roteamento dinâmico de requisições para os microsserviços.
- Filtros para manipulação de requisições e respostas.
- Monitoramento e métricas com **Spring Boot Actuator**.
- Integração com o **Service Discovery** para resolução de microsserviços.
- Ponto centralizado de entrada para clientes externos.

---

## 🚀 Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Vitor192/Gateway.git
