# 📦 Software Delivery

Sistema desenvolvido para gerenciamento de entregas, incluindo cadastro de usuários, pedidos e acompanhamento de status.

---

## 📌 Descrição

Este projeto tem como objetivo simular um sistema de **Software Delivery**, abordando conceitos fundamentais de engenharia de software:

* Requisitos funcionais e não funcionais
* Testes de software
* Documentação e organização de projetos



## 📋 Requisitos Funcionais

* RF01: Cadastro de usuários
* RF02: Login com e-mail e senha
* RF03: Cadastro de pedidos
* RF04: Acompanhamento do status da entrega
* RF05: Atualização de dados do usuário
* RF06: Registro de movimentação de entrega

---

## ⚙️ Requisitos Não Funcionais

* RNF01: Tempo de resposta de até 2 segundos
* RNF02: Segurança dos dados (login protegido)
* RNF03: Disponibilidade 24h
* RNF04: Compatibilidade com navegadores modernos
* RNF05: Suporte a múltiplos usuários simultâneos
* RNF06: Interface simples e intuitiva

---

## 🧪 Testes

### 🔹 Teste de Cadastro de Usuário

**Tipo:** Caixa preta

**Objetivo:**
Verificar se o usuário é cadastrado corretamente

**Passos:**

1. Acessar tela de cadastro
2. Preencher nome, e-mail e senha
3. Clicar em "Cadastrar"

**Resultado esperado:**

* Usuário cadastrado com sucesso
* Mensagem de confirmação exibida

**Cenários alternativos:**

* Campos vazios → exibir erro
* E-mail inválido → bloquear cadastro

---

### 🔹 Teste do Movimento de Entrega

**Tipo:** Integração / E2E

**Objetivo:**
Validar o fluxo completo de entrega

**Passos:**

1. Criar pedido
2. Atualizar status para "Em preparação"
3. Atualizar status para "Saiu para entrega"
4. Atualizar status para "Entregue"

**Resultado esperado:**

* Status atualizado corretamente
* Histórico da entrega registrado

---

## 📄 Documentos e Artefatos de Teste

Além do código, foram criados documentos auxiliares para organização dos testes:

* 📑 **Plano de Teste** → define o que, como e quando testar
* 📝 **Casos de Teste** → descrevem os passos para validar funcionalidades
* 📊 **Relatórios de Teste** → registram os resultados obtidos

---

### 🔹 Exemplo de Caso de Teste (Login)

**Objetivo:**
Validar login com credenciais corretas

**Passos:**

1. Acessar tela de login
2. Inserir usuário válido
3. Inserir senha válida
4. Clicar em "Entrar"

**Resultado esperado:**
Usuário acessa o sistema com sucesso

---

## ▶️ Como Executar

```bash
# Clonar o repositório
git clone https://github.com/RobersonCodes/UC11.git

# Acessar a pasta
cd UC11
```

---

## 👨‍💻 Autor

**Roberson de Oliveira**
Estudante de Desenvolvimento de Software

---

## 📌 Status do Projeto

🚧 Em desenvolvimento
