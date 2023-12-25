# Sistema de Controle de Ordens de Serviço em Oficina Mecânica

## Descrição do Projeto

Este banco de dados foi projetado para gerenciar e controlar a execução de ordens de serviço em uma oficina mecânica, incluindo clientes, equipes de mecânicos, serviços prestados e peças utilizadas.

### Entidades:

1. **Cliente**
   - ID do Cliente (Chave Primária)
   - Nome do Cliente
   - Veículo do Cliente

2. **Equipe Mecânica**
   - ID da Equipe (Chave Primária)
   - Código do Mecânico (Chave Estrangeira)
   - Nome do Mecânico
   - Endereço do Mecânico
   - Especialidade do Mecânico

3. **Ordem de Serviço (OS)**
   - Número da OS (Chave Primária)
   - ID do Cliente (Chave Estrangeira)
   - ID da Equipe (Chave Estrangeira)
   - Data de Emissão
   - Valor Total da OS
   - Status da OS
   - Data para Conclusão dos Trabalhos

4. **Serviços**
   - ID do Serviço (Chave Primária)
   - Descrição do Serviço
   - Valor do Serviço

5. **Peças**
   - ID da Peça (Chave Primária)
   - Descrição da Peça
   - Valor da Peça

### Relacionamentos:

- Cliente (Ordem de Serviço) -> Relacionamento 1:N
- Equipe Mecânica (Ordem de Serviço) -> Relacionamento 1:N
- Ordem de Serviço (Serviços) -> Relacionamento N:M
- Ordem de Serviço (Peças) -> Relacionamento N:M


![oficina drawio](https://github.com/JuanVictorf/DiagramaOficina/assets/68507832/6d43dce4-1636-4fa1-80c2-a7d9ef11fa63)
