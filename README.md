# Software Delivery

## Requisitos Funcionais

- RF01: O sistema deve permitir o cadastro de usuários  
- RF02: O sistema deve permitir login com e-mail e senha  
- RF03: O sistema deve permitir cadastro de pedidos  
- RF04: O sistema deve permitir acompanhar o status da entrega  
- RF05: O sistema deve permitir atualizar dados do usuário  
- RF06: O sistema deve permitir registro de movimentação de entrega (saída, em rota, entregue)  

---

## Requisitos Não Funcionais

- RNF01: O sistema deve responder em até 2 segundos  
- RNF02: O sistema deve garantir segurança dos dados (login protegido)  
- RNF03: O sistema deve estar disponível 24 horas por dia  
- RNF04: O sistema deve ser compatível com navegadores modernos  
- RNF05: O sistema deve suportar múltiplos usuários simultâneos  
- RNF06: O sistema deve possuir interface simples e intuitiva  

---

## Teste de Cadastro de Usuário

**Tipo de teste:**  
- Caixa preta  
- Pode ser automatizado com Selenium  

**Cenário de teste:**  

**Objetivo:**  
Verificar se o usuário é cadastrado corretamente  

**Passos:**  
1. Acessar tela de cadastro  
2. Preencher nome, e-mail e senha  
3. Clicar em "Cadastrar"  

**Resultado esperado:**  
- Usuário cadastrado com sucesso  
- Mensagem de confirmação exibida  

**Teste alternativo:**  
- Campos vazios → deve exibir erro  
- E-mail inválido → deve bloquear cadastro  

---

## Teste do Movimento de Entrega

**Tipo de teste:**  
- Integração / E2E  

**Cenário de teste:**  

**Objetivo:**  
Verificar o fluxo de entrega  

**Passos:**  
1. Criar pedido  
2. Alterar status para "Em preparação"  
3. Alterar status para "Saiu para entrega"  
4. Alterar status para "Entregue"  

**Resultado esperado:**  
- Status atualizado corretamente em cada etapa  
- Sistema registra o histórico da entrega  
