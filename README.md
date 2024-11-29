# Sistema de Controle de Ordens de Serviço - Oficina Mecânica

## Objetivo
Desenvolver o esquema conceitual para o gerenciamento de ordens de serviço em uma oficina mecânica, com base na narrativa fornecida. Este projeto tem como foco criar um modelo que represente as entidades, relacionamentos e atributos necessários para atender às necessidades operacionais da oficina.

---

## Descrição do Contexto
O sistema proposto é voltado para controle e gestão da execução de ordens de serviço em uma oficina mecânica, considerando os seguintes elementos:

1. **Clientes e Veículos:**
   - Os clientes levam seus veículos à oficina para serviços como conserto ou revisões periódicas.
   - Cada veículo é associado a um cliente.

2. **Equipe e Serviços:**
   - Os veículos são atribuídos a uma equipe de mecânicos, responsável por identificar os serviços necessários e criar uma Ordem de Serviço (OS).
   - Os mecânicos possuem as seguintes informações:
     - Código
     - Nome
     - Endereço
     - Especialidade

3. **Ordem de Serviço (OS):**
   - Cada OS inclui:
     - Número
     - Data de emissão
     - Valor total (calculado com base em mão de obra e peças)
     - Status (ex.: "Aguardando aprovação", "Em andamento", "Concluído")
     - Data para conclusão dos trabalhos
   - A partir da OS, é consultada uma tabela de referência para calcular o valor de cada serviço.
   - O valor das peças utilizadas também compõe o valor final da OS.
   - O cliente deve autorizar a execução dos serviços.

4. **Execução dos Serviços:**
   - A mesma equipe que cria a OS também é responsável por avaliar e executar os serviços solicitados.
  



