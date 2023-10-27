- 👋 Hi, I’m @MarcianoDiniz
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
MarcianoDiniz/MarcianoDiniz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
'''flowchart TB
    subgraph Sistema
        subgraph "Usuários"
            Cliente -->|Cadastrar| Cadastro
            Cliente -->|Introduzir Pedido| Pedidos
            Cliente -->|Consultar Pedido| Pedidos
            Cliente -->|Cancelar Pedido| Pedidos
        end
        subgraph "Agentes"
            Empresa -->|Modificar Pedido| Pedidos
            Empresa -->|Avaliar Pedido| Pedidos
            Banco -->|Modificar Pedido| Pedidos
            Banco -->|Avaliar Pedido| Pedidos
        end
        Cadastro -->|Armazenar Dados| Banco de Dados
        Pedidos -->|Análise Financeira| Agentes
        Pedidos -->|Execução de Contrato| Agentes
    end
    subgraph "Contratantes"
        Cadastro
        subgraph "Dados de Identificação"
            Cadastro
        end
        Profissão -->|Armazenar| Banco de Dados
        Entidades Empregadoras -->|Armazenar| Banco de Dados
        Rendimentos -->|Armazenar| Banco de Dados
    end
    subgraph "Automóveis"
        Matrícula -->|Armazenar| Banco de Dados
        Ano -->|Armazenar| Banco de Dados
        Marca -->|Armazenar| Banco de Dados
        Modelo -->|Armazenar| Banco de Dados
        Placa -->|Armazenar| Banco de Dados
    end
    subgraph "Contratos de Crédito"
        Banco
    end
    subgraph "Servidor Central"
    subgraph "Computadores Locais"
        Cliente
        Empresa
    end
    Banco -->|Concessão de Crédito| Contratos de Crédito
    Banco -->|Concessão de Crédito| Banco de Dados
    subgraph "Construção de Páginas WWW"
    end
    subgraph "Internet"
    end

