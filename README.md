[diagrama]
'''mermaid
Cliente --> Cadastro;
Cliente -->|Ações| Pedidos;
Cliente -->|Ações| Consulta;
Cliente -->|Ações| Cancelamentos;

Empresas -->|Ações| Modificação;
Empresas -->|Ações| Avaliação;

Bancos -->|Ações| Modificação;
Bancos -->|Ações| Avaliação;
Bancos -->|Ações| Concessão de Crédito;

Pedidos -->|Ações| Análise Financeira;

Análise Financeira -->|Ações| Execução do Contrato;

Cadastro -->|Armazenamento| BancoDados;
Pedidos -->|Armazenamento| BancoDados;
'''
Contratos -->|Armazenamento| BancoDados;
Clientes -->|Armazenamento| BancoDados;
Empresas -->|Armazenamento| BancoDados;
Bancos -->|Armazenamento| BancoDados;
Automóveis -->|Armazenamento| BancoDados;
Crédito -->|Armazenamento| BancoDados;

PaginasWWW -->|Construção| ServidorCentral;
'''


