# FAQChatBot

!Importante! Caso de erro no banco de dados do projeto, é preciso dropar as tabelas e cria-las de novo, isso acontece quando é passado o programa para outro pc por causa do uso do localdb

Passo a Passo:
1. Abra o vs code e abra o powershell usando o atalho "crtl + '", ele irá abrir o painel

2. Referencie o endereço de arquivo do seu .csproj ex. cd <endereço da pasta do .csproj>

3. cole o prompt para dropar tabela "dotnet ef database drop" e depois para atualizar "dotnet ef database update"
