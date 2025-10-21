# Projeto: Funil Inteligente de Recuperação de Pagamentos com N8N

Este repositório contém os workflows de uma automação construída em N8N para recuperar vendas de pagamentos (PIX/Boleto) não concluídos na empresa Weburn.

## 🎯 O Problema

Um número significativo de clientes gerava um meio de pagamento, mas não concluía a transação, resultando em perda de receita e um processo de cobrança manual ineficiente.

## ⚙️ A Solução

Desenvolvi uma régua de comunicação 100% automatizada, com duração de 5 dias, para engajar esses clientes via WhatsApp e recuperar as vendas.

### Destaques da Arquitetura:

* **Orquestração:** N8N para desenhar e executar todo o fluxo lógico.
* **Comunicação:** Integração direta com a WhatsApp Business API para o envio de lembretes personalizados.
* **Integrações:**
    * Iniciado por webhook de um CRM (Clint).
    * Consulta de dados em tempo real em uma plataforma de pagamentos (Guru) via API REST.
* **Lógica Avançada:** O sistema possui um workflow "ouvinte" que detecta respostas do cliente. Se o cliente confirma o pagamento, a régua de comunicação é **interrompida imediatamente**, evitando SPAM e melhorando a experiência do usuário.

### Tecnologias e Ferramentas

* N8N
* WhatsApp Business API
* APIs REST / Webhooks
* Git / GitHub

---

### Visualização do Fluxo Principal

*Insira aqui o print do seu projeto (`image_a709e2.jpg`)*
