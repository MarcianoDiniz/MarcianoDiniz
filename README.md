graph TD

subgraph cluster_Usuarios
    Cliente[Clientes (Usuários Individuais)]
end

subgraph cluster_Agentes
    Empresas[Empresas]
    Bancos[Bancos]
end

subgraph cluster_Servidor
    ServidorCentral[Servidor Central]
end

subgraph cluster_BD
    BancoDados[Banco de Dados]
end

subgraph cluster_PaginasWeb
    PaginasWWW[Construção de Páginas WWW]
end

Cliente -->|Ações| Cadastro
Cliente -->|Ações| Pedidos
Cliente -->|Ações| Consultas
Cliente -->|Ações| Cancelamentos

Empresas -->|Ações| Modificação
Empresas -->|Ações| Avaliação

Bancos -->|Ações| Modificação
Bancos -->|Ações| Avaliação
Bancos -->|Ações| Concessão de Crédito

Pedidos -->|Ações| Análise Financeira

Análise Financeira -->|Ações| Execução do Contrato

Cadastro -->|Armazenamento| BancoDados
Pedidos -->|Armazenamento| BancoDados
Contratos -->|Armazenamento| BancoDados
Clientes -->|Armazenamento| BancoDados
Empresas -->|Armazenamento| BancoDados
Bancos -->|Armazenamento| BancoDados
Automóveis -->|Armazenamento| BancoDados
Crédito -->|Armazenamento| BancoDados

PaginasWWW -->|Construção| ServidorCentral


