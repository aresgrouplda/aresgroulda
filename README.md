# Sistema de Gerenciamento de Salões

Este projeto é um **sistema de gerenciamento de salões de beleza** dividido em vários microserviços, cada um responsável por uma parte específica da operação do salão. A arquitetura de microserviços permite que o sistema seja escalável, modular e fácil de manter.

### 🧩 **Arquitetura do Sistema**

Abaixo está a lista de microserviços que compõem a aplicação:

- **auth-service**: Gerenciamento de autenticação e autorização de usuários (clientes, funcionários e administradores).
- **salon-service**: Gerenciamento dos salões e suas filiais.
- **employee-service**: Gerenciamento dos funcionários do salão.
- **booking-service**: Gerenciamento de agendamentos de serviços.
- **services-catalog-service**: Gerenciamento de serviços disponíveis (corte de cabelo, manicure, etc.).
- **payment-service**: Processamento de pagamentos.
- **notification-service**: Envio de notificações (lembretes de agendamento, alterações, etc.).
- **feedback-service**: Coleta e gerenciamento de feedbacks dos clientes.
- **report-service**: Geração de relatórios de desempenho do salão.
- **promotion-service**: Gerenciamento de promoções e descontos.
- **inventory-service**: Controle de inventário de produtos utilizados nos serviços.
- **resource-scheduling-service**: Gerenciamento do agendamento de recursos compartilhados (cadeiras, equipamentos, etc.).

### 📝 **Funcionalidades Principais**

#### **1. Auth Service**
- Cadastro de usuários (clientes, funcionários).
- Autenticação e controle de permissões com tokens JWT.
- Gerenciamento de sessões de usuários.

#### **2. Salon Service**
- Cadastro de salões (nome, localização, capacidade).
- Gerenciamento de filiais e serviços oferecidos.
- Configuração de horários de funcionamento e preços.

#### **3. Employee Service**
- Cadastro de funcionários (cabeleireiros, manicures, etc.).
- Controle de horários de trabalho e atribuição de serviços.
- Avaliação de desempenho.

#### **4. Booking Service**
- Agendamento de serviços.
- Verificação de disponibilidade de horários e funcionários.
- Cancelamento e remarcação de agendamentos.
- Notificações de agendamento via SMS e e-mail.

#### **5. Services Catalog Service**
- Cadastro e gerenciamento de serviços oferecidos.
- Definição de duração, preço e descrição de cada serviço.
- Atribuição de serviços a funcionários ou salões.

#### **6. Payment Service**
- Processamento de pagamentos (cartão de crédito, débito, etc.).
- Geração de recibos e faturas.
- Integração com gateways de pagamento como Stripe, PayPal.

#### **7. Notification Service**
- Envio de notificações para clientes e funcionários.
- Lembretes de agendamentos, mudanças de horários, etc.

#### **8. Feedback Service**
- Coleta de avaliações de clientes após o serviço.
- Relatórios de desempenho baseados em feedback.

#### **9. Report Service**
- Relatórios de receita, ocupação de horários, desempenho de funcionários e mais.

#### **10. Promotion Service**
- Criação e gerenciamento de promoções e descontos.
- Geração de códigos promocionais.

#### **11. Inventory Service**
- Controle de estoque de produtos (shampoos, tinturas, etc.).
- Alertas de reposição de estoque.

#### **12. Resource Scheduling Service**
- Agendamento de recursos compartilhados (cadeiras, secadores, etc.).
- Verificação de disponibilidade de recursos durante os agendamentos.

---

### 🔧 **Tecnologias Usadas**

- **Spring Boot**: Framework para construir APIs RESTful para microserviços.
- **Spring Security**: Para autenticação e controle de permissões.
- **Spring Gateway**: Para comunicação assíncrona entre microserviços.
- **GitHub Actions**: Para CI/CD e automação de testes.

---

### 🏗️ **Estrutura do Repositório**

```plaintext
github.com/aresgrouplda/
├── auth-service                  # Gerenciamento de autenticação e autorização
├── salon-service                 # Gerenciamento de salões
├── employee-service              # Gerenciamento de funcionários
├── booking-service               # Agendamento de serviços
├── services-catalog-service      # Catálogo de serviços
├── payment-service               # Processamento de pagamentos
├── notification-service          # Envio de notificações
├── feedback-service              # Coleta de feedbacks de clientes
├── report-service                # Geração de relatórios
├── promotion-service             # Gerenciamento de promoções
├── inventory-service             # Controle de inventário
└── resource-scheduling-service   # Agendamento de recursos compartilhados
```

---

### 🧑‍💻 **Como Contribuir**

1. **Fork o repositório** e crie uma nova branch para sua feature:
   ```bash
   git checkout -b minha-feature
   ```

2. **Faça suas alterações** e escreva testes para garantir que tudo funciona.
3. **Commit suas alterações**:
   ```bash
   git commit -am "Descrição das alterações"
   ```

4. **Envie para o seu fork**:
   ```bash
   git push origin minha-feature
   ```

5. **Crie um Pull Request (PR)** para o branch principal (`main`).

---

### 📜 **Licença**

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo LICENSE para mais informações.

---

### 💬 **Contatos e Suporte**

Se tiver alguma dúvida ou problema, entre em contato com a equipe de desenvolvimento ou abra uma **issue** no GitHub.

---

### 🚀 **Próximos Passos**

- **Escalabilidade**: Planejamos usar Kubernetes para orquestrar os microserviços em produção.
- **Monitoramento**: Implementar soluções de monitoramento (Prometheus, Grafana) para visualizar o desempenho dos microserviços.

---
