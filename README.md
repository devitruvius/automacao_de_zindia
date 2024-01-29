# Automação de Zindia

### Etapa 1: Rastreamento das Coordenadas

1. **Ação Inicial:** Enviar as `coordenadas` do posto por-email para o setor de rastreamento.
2. **Responsabilidade do Setor de Rastreamento:** Validar as coordenadas recebidas.

### Etapa 2: Anexar Documentos e Informações no SAP

1. **Ação:** Após a validação das coordenadas, encaminhar um e-mail contendo `contrato social`, `CNPJ` e `coordenadas` para o setor de Crédito.
2. **Responsabilidade do Setor de Crédito:**
   - Anexar os documentos no SAP.
   - Informar a latitude e longitude.
   - Criar um código de identificação para o cliente.
  
### Etapa 3: Lançamento dos Pedidos

1. **Ação:** Durante o lançamento de pedidos, é inserido o `código do cliente`.
2. **Informações Adicionadas no Pedido:**
   - Tipo de frete (`FOB` ou `CIF`).
   - Prazo de entrega, se aplicável.
  
### Etapa 4: Condição FOB

1. **Se FOB:**
   - Opção de `carga assegurada`.
   - Adição de R$ 0,008 ao valor de cada produto.

### Etapa 5: Adicional no Prazo

1. **Adicional no Prazo:** Se houver prazo aprovado pelo setor de Crédito, adiciona `valor extra` de acordo com os dias aprovados.

### Etapa 6: Condição CIF

1. **Se CIF:**
   - Sistema soma o `valor dos produtos` com o `valor do frete`.
   - Opção de prazo, com adicional no `valor total` conforme o prazo aprovado.
  
### Etapa 7: Acesso à Ficha de Crédito

1. **Acesso à Ficha de Crédito:**
   - Acesso parcial à ficha de crédito.
   - Acompanhamento dos lançamentos, incluindo PIX, TED e boletos para clientes com prazo.
  
  ### Etapa 8: Pagamento de Boletos

  1. **Quando o Cliente Paga Boletos:**
     - Cliente repassa comprovante em PDF.
     - Anexação do comprovante na ficha do cliente.
     - Análise e baixa realizadas pelo setor financeiro.
