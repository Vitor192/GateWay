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

   🛠️ Exemplo de Configuração

No arquivo application.yml, podemos configurar o Gateway com rotas para outros microsserviços:

yml 

server:
  port: 8080

spring:
  application:
    name: gateway

  cloud:
    gateway:
      routes:
        - id: product-catalog
          uri: http://localhost:8081
          predicates:
            - Path=/products/**
        - id: shopping-cart
          uri: http://localhost:8082
          predicates:
            - Path=/cart/**

management:
  endpoints:
    web:
      exposure:
        include: "*"

📚 Próximos Passos

Adicionar autenticação e autorização no Gateway.

Implementar log centralizado de requisições.

Integrar com Circuit Breaker e resiliência via Spring Cloud.



