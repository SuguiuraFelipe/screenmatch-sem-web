# Screenmatch (sem Web)

Projeto desenvolvido em **Java** com **Spring Boot** e **Maven**, focado no estudo de arquitetura backend, modelagem de domínio e integração entre serviços — sem camada web.

## 🎯 Objetivo do Projeto
Reproduzir a lógica central do Screenmatch usando:
- Modelagem orientada a objetos
- Serviços independentes
- Boas práticas de organização de pacotes
- Regras de negócio desacopladas de interface
- Execução via linha de comando / aplicação standalone

O foco é compreender **como estruturar e conectar as partes internas de uma aplicação**, sem depender de controllers ou endpoints HTTP.

---

## 🧠 Conceitos Praticados

### ✔ Programação Orientada a Objetos
- Criação de entidades e classes de domínio
- Encapsulamento e uso de getters/setters
- Composição entre objetos
- Modelos representando filmes, séries ou avaliações (dependendo da sua estrutura)

### ✔ Arquitetura Backend (sem Web)
- Separação em camadas (model, service, repository / mock)
- Dependências bem definidas entre componentes
- Fluxo interno organizado para consultas e regras de negócio

### ✔ Spring Boot na prática
- Configuração com `SpringApplication.run`
- Beans gerenciados pelo Spring (injeção de dependência)
- Organização modular de pacotes
- Execução estruturada sem precisar de controllers

### ✔ Maven
- Gerenciamento de dependências
- Execução com plugin **spring-boot-maven-plugin**
- Build e empacotamento para `.jar`

---

## ▶️ Como executar

```bash
mvn spring-boot:run
Ou:

bash
Copiar código
mvn clean package
java -jar target/*.jar
📁 Estrutura (simplificada)
css
Copiar código
src/main/java
 ├── model      -> classes de domínio (filmes, dados, ratings…)
 ├── service    -> regras de negócio e operações principais
 ├── config     -> configuração básica Spring Boot
 └── Application.java
📝 Aprendizados do Projeto
Como estruturar uma aplicação backend limpa sem interface gráfica

Como dividir responsabilidades entre serviços e modelos

Como organizar pacotes de forma profissional

Como fazer o Spring Boot trabalhar como motor de execução, mesmo sem endpoints

Como usar Maven de forma prática para build e execução

📄 Sobre
Este projeto é parte de um percurso de estudos em backend Java, servindo como base para futuros módulos, APIs REST e integração com bancos de dados.
