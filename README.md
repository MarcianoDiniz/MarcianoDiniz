<!---
MarcianoDiniz/MarcianoDiniz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
---
mermaid
flowchart TD

subgraph cluster_Usuarios
    Usuario[Usuários]
end

subgraph cluster_Agentes
    Agentes[Empresas e Bancos]
end

subgraph cluster_Sistema
    Sistema[Servidor Central]
    Subsistema1[Gestão de Pedidos e Contratos]
    Subsistema2[Construção de Páginas WWW]
end

subgraph cluster_Dados
    Dados_Clientes[Dados dos Clientes]
    Dados_Automoveis[Dados dos Automóveis]
    Dados_Contratos[Dados dos Contratos]
    Dados_Credito[Contratos de Crédito]
end

Usuario --> Dados_Clientes
Agentes --> Dados_Contratos
Agentes --> Dados_Automoveis
Usuario --> Subsistema1
Sistema --> Subsistema1
Sistema --> Subsistema2
Sistema --> Dados_Clientes
Sistema --> Dados_Automoveis
Sistema --> Dados_Contratos
Sistema --> Dados_Credito
---

       
    
    

