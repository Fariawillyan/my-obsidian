1. **Classes de Alto Nível (High-Level Classes)**:
    
    - São classes que contêm a lógica de negócios e as regras de alto nível do sistema.
    - Normalmente, essas classes estão mais próximas do domínio do problema e são menos dependentes de detalhes de implementação.
    - Elas encapsulam as políticas e estratégias do negócio.
    - Classes de alto nível são geralmente menos voláteis em relação a mudanças no ambiente externo, como mudanças na interface do usuário ou no banco de dados.
    - Exemplos de classes de alto nível podem incluir casos de uso, entidades do domínio e interatores.
2. **Classes de Baixo Nível (Low-Level Classes)**:
    
    - São classes que lidam com detalhes de implementação e são responsáveis pela manipulação de dados e comunicação com recursos externos.
    - Elas são mais concretas e geralmente estão mais próximas da infraestrutura do sistema, como bancos de dados, sistema de arquivos, rede, etc... Famosos **detalhes**.
    - Classes de baixo nível geralmente têm mais dependências externas e são mais propensas a mudanças devido a alterações nos detalhes de implementação.
    - Exemplos de classes de baixo nível podem incluir classes de acesso a dados (como DAOs - Data Access Objects), classes de serviços, classes de infraestrutura (como classes de conexão de banco de dados) e classes de utilitários.

O princípio por trás da arquitetura limpa é que as classes de alto nível devem depender das classes de baixo nível, mas não o contrário. Isso significa que as classes de alto nível devem ser independentes dos detalhes de implementação das classes de baixo nível. Isso promove uma arquitetura mais modular e flexível, facilitando a manutenção e evolução do sistema ao longo do tempo.

- Sempre usar interfaces para desacoplar o código para respeitar os limites e camadas da aplicação. Respeitando, podemos trocar facilmente os *plugins*.