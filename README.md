# FAQChatBot — Zero Um Cursos
 
Sistema web de suporte técnico automatizado com FAQ e chatbot integrado, desenvolvido para plataformas de ensino online. Permite que alunos resolvam dúvidas comuns sem intervenção humana, com redirecionamento para atendente quando necessário.
 
Projeto Integrado Multidisciplinar IV (PIM IV) — UNIP, curso de Análise e Desenvolvimento de Sistemas (2025).
 
---
 
## Sobre o projeto
 
A **Zero Um Cursos** é uma plataforma EAD fictícia criada para o projeto. O sistema oferece:
 
- FAQ com perguntas frequentes categorizadas
- Chatbot conversacional com fluxo de perguntas e respostas
- Redirecionamento de chamados por e-mail quando a IA não resolve
- Sistema de feedback do usuário ao final de cada atendimento
- Cadastro e autenticação de usuários com criptografia de senha (BCrypt)
- Recuperação de senha por e-mail
- Interface responsiva (desktop e mobile)
- Conformidade com a LGPD (Lei 13.709/2018)
---
 
## Tecnologias
 
- **Back-end:** ASP.NET Core MVC (C#)
- **Front-end:** HTML, CSS, JavaScript
- **Banco de dados:** SQL Server (LocalDB) com Entity Framework Core (Code First)
- **Segurança:** BCrypt para hashing de senhas, HTTPS com TLS
- **Documentação:** LaTeX, Doxygen
- **IDE:** Visual Studio 2022
---
 
## Funcionalidades principais
 
- Login e cadastro de usuários (CPF, e-mail, telefone, senha com validação)
- Dashboard com progresso de cursos do aluno (apenas visual)
- FAQ com perguntas organizadas por categoria
- Chatbot interativo desenvolvido do zero com fluxo de estados, matching de palavras-chave e respostas automáticas
- Redirecionamento de chamado para especialista via e-mail (apenas visual)
- Coleta de feedback ao final de cada atendimento
- Log de conversas para histórico e análise
- Painel de privacidade (exportar dados, editar perfil, excluir conta — LGPD)
---
 
## Documentação completa
 
A documentação técnica inclui escopo, cronograma, regras de negócio, requisitos funcionais e não funcionais, 7 tipos de diagramas UML, manual de uso com interfaces, código-fonte comentado, diagrama ER e seção de segurança/LGPD.
 
[Ver documentação completa (PDF)](./docs/PIM-IV-ZeroUmCursos.pdf)
 
### Diagramas incluídos
 
- Diagrama de Casos de Uso
- Diagrama de Classe
- Diagrama de Sequência (Login, ChatBot, FAQ)
- Diagrama de Pacote
- Diagrama de Colaboração
- Diagrama de Componentes
- Diagrama de Atividades
- Diagrama Entidade-Relacionamento (ER)
---
 
## Como rodar o projeto
 
### Pré-requisitos
 
- Visual Studio 2022 ou superior
- .NET SDK 8.0+
- SQL Server LocalDB (incluído no Visual Studio)
### Passo a passo
 
1. Clone o repositório:
```bash
git clone https://github.com/Rafael-Rase/FAQChatBot-ZeroUm-Cursos.git
```
 
2. Abra o arquivo `FAQChatBot.sln` no Visual Studio
3. Configure o banco de dados via terminal integrado (`Ctrl + '`):
```bash
cd <caminho até a pasta do .csproj>
dotnet ef database drop
dotnet ef database update
```
 
> O banco precisa ser recriado ao rodar em uma máquina diferente da original (LocalDB).
 
4. Execute o projeto com `F5`
---
 
## Estrutura do repositório
 
```
FAQChatBot-ZeroUm-Cursos/
├── FAQChatBot/         # Código-fonte principal (ASP.NET Core MVC)
│   ├── Models/         # Entidades e AppDbContext (Code First)
│   ├── Views/          # Interfaces (.cshtml + CSS/JS)
│   ├── Controllers/    # HomeController (autenticação, dashboard, FAQ)
├── html/               # Documentação gerada pelo Doxygen
├── latex/              # Fonte LaTeX da documentação
├── docs/               # Documentação completa em PDF (PIM IV)
├── FAQChatBot.sln      # Solution do Visual Studio
└── README.md
```
 
---
 
## Autor principal
 
**Rafael Segura de Castro** — responsável por diagramas UML, requisitos funcionais e de negócio, modelagem do banco de dados, desenvolvimento back-end, homologação e manutenção do código.
 
Projeto desenvolvido em equipe com: Diogo Gonçalves, Erbeson Nunes, Felipe Sizani, Guilherme Mazzini e Patrick Bortolin.
 
