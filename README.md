# 💱 Conversor de Moedas: Projeto Desafio ONE (Oracle Next Education)

## 📄 Visão Geral

Este projeto é a solução desenvolvida para o **Challenge ONE: Conversor de Moedas**, parte do programa **Oracle Next Education (ONE)** em parceria com a Alura.

Trata-se de um **aplicativo de linha de comando (CLI)** implementado em Java, desenhado para realizar conversões de moedas em tempo real através de um menu interativo.

O foco técnico principal do projeto foi demonstrar a **integração com APIs externas** (via HTTP) e o **processamento de dados JSON** dentro de um ambiente Java.

---

## ⭐ Recursos Principais e Requisitos Cumpridos

* **Menu de Opções Fixas:** Permite a escolha rápida de pares de moedas populares (ex.: USD/BRL, USD/ARS, USD/COP).
* **Integração HTTP:** Realiza requisições `GET` à **ExchangeRate-API** para obter taxas de câmbio atuais.
* **Histórico de Sessão:** Armazena todas as conversões bem-sucedidas em uma lista (`ArrayList`) e exibe um resumo completo ao sair da aplicação.
* **Tratamento de Exceções:** Implementação robusta de `try-catch` para gerenciar diversos cenários de erro, incluindo:
    * Erros de rede (`IOException`, `InterruptedException`).
    * Erros de parsing JSON da API.
    * Entradas inválidas do usuário (`NumberFormatException`).

---

## 💻 Tecnologias Empregadas

| Categoria | Tecnologia | Detalhes |
| :--- | :--- | :--- |
| **Linguagem Base** | Java 17+ | Utilizada para o desenvolvimento da aplicação CLI. |
| **Cliente HTTP** | `java.net.http.HttpClient` | API nativa do Java para gerenciar as requisições web. |
| **Processamento JSON** | Biblioteca Gson | Responsável por desserializar a resposta JSON da API. |
| **Fonte de Câmbio** | ExchangeRate-API | Serviço externo que fornece as taxas de conversão. |
