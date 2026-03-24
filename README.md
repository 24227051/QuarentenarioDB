# QuarentenarioDB

Banco de dados do Sistema de Gestão de dados do Laboratório de Biologia Molecular do Quarentenário [IAC - Instituto Agronômico de Campinas](https://www.iac.sp.gov.br) desenvolvido como parte do Projeto Integrador da UNIVESP. No repositório [QuarentenarioWeb](https://github.com/24227051/QuarentenarioWeb) se encontra o projeto web que também faz parte desse projeto

### Disciplina
Projeto Integrador em Computação I. Tecnologia da Informação. UNIVESP - Universidade Virtual do Estado de São Paulo

## Motivação
O Projeto Integrador trata de resolução de problemas e os estudantes devem ser expostos a atividades que visam relacionar conteúdos curriculares a práticas profissionais. Cada Projeto Integrador é estruturado para consolidar o conhecimento das disciplinas dos semestres anteriores em atividades práticas que visam buscar a solução para um problema e sua implementação. O objetivo é se chegar a um protótipo funcional que sirva como prova de conceito das ideias propostas. 

## Definição
Gerenciador de amostras no meio bioquímico através de uma interface web com persistência em banco de dados e controle de versão do código-fonte 

### Características
- Gerenciador de Análises
- Gerenciador de Anexos
- Gerenciador de Boletins
- Gerenciador de Materiais
- Gerenciador de Materiais x Patógenos
- Gerenciador de Patógenos
- Gerenciador de Países
- Gerenciador de Tipos Controle
- Gerenciador de Tipos Patógeno

## Requisitos
.NET 10

## Primeiros passos
1. Baixar e instalar o [SQL Server 2025 Express](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads) que é uma versão gratuita destinada à produção de aplicativos pequenos, sites leves e ferramentas de aprendizado.
2. Baixar e instalar o [SQL Server Management Studio](https://learn.microsoft.com/pt-br/ssms/install/install) que é uma ferramenta de gerenciamento do banco de dados.
3. Abrir o SQL Server Management Studio (SSMS) e criar um novo banco de dados chamado quarentanario ou executar o script bancoDados.sql desse repositório.
4. Ainda no SSMS executar o script tabelas.sql desse repositório.
5. Ainda no SSMS executar o script procedures.sql desse repositório.
6. Baixar o arquivo Análises para cada material - Importação.CSV , na pasta Documentos/Quarentena no SharePoint EixoComputacaoVinhedo
7. Ainda no SSMS clicar no banco de dados quarentanario com o botão direito > Tasks > Import Flat File > Escolha o CSV > Nome da Tabela: Importacao. Se der erro exclua a tabela Importacao
8. Executar a procedure sp_importacao
