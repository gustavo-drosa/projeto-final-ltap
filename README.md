# Sistema de Cadastro de Bandas

Sistema desktop desenvolvido em C# Windows Forms para gerenciamento e cadastro de bandas musicais.

## 📋 Descrição

Este projeto é um sistema de cadastro que permite gerenciar informações sobre bandas musicais, incluindo nome, número de integrantes, ranking e gênero musical. O sistema utiliza MySQL como banco de dados e oferece uma interface gráfica intuitiva para cadastro e busca de informações.

## 🚀 Tecnologias Utilizadas

- **C# (.NET Framework)** - Linguagem de programação
- **Windows Forms** - Framework para interface gráfica
- **MySQL 8.1.0** - Sistema de gerenciamento de banco de dados
- **ADO.NET** - Acesso a dados
- **Visual Studio** - IDE de desenvolvimento

## 📦 Dependências

O projeto utiliza as seguintes bibliotecas NuGet:

- MySql.Data 8.1.0

## Telas da aplicação
### LOGIN
![Tela de login](assets/TelaLogin.png)
### CADASTRO DE BANDAS
![Tela de cadastro de bandas](assets/TelaCadastro.png)
### CONSULTA E BUSCA
![Tela de consulta e busca](assets/TelaBuscar.png)
### ATUALIZAR BANDA
![Tela de atualização de banda](assets/TelaAlterar.png)
### ADICIONAR NOVO GÊNERO
![Tela de adicionar novo gênero](assets/TelaAdicionarGenero.png)

## 🗄️ Estrutura do Banco de Dados

O sistema utiliza duas tabelas principais:

### Tabela `generos`
- `idgenero` (INT, AUTO_INCREMENT, PRIMARY KEY)
- `genero` (VARCHAR(45))

Gêneros pré-cadastrados: Rock, Metal, Pagode, Gospel, Funk

### Tabela `bandas`
- `idbandas` (INT, AUTO_INCREMENT, PRIMARY KEY)
- `nome` (VARCHAR(45))
- `integrantes` (INT)
- `ranking` (INT)
- `fk_genero` (INT, FOREIGN KEY)

### Stored Procedures

- `sp_insereBanda` - Insere uma nova banda no banco
- `sp_listaBandas` - Lista todas as bandas com seus gêneros
- `sp_listaGeneros` - Lista todos os gêneros disponíveis

## ⚙️ Instalação e Configuração

### Pré-requisitos

- Visual Studio 2019 ou superior
- MySQL Server 8.0 ou superior
- .NET Framework 4.7.2 ou superior


## 🎯 Funcionalidades

- ✅ **Cadastro de Bandas** - Adicione novas bandas com informações completas
- 🔍 **Busca de Bandas** - Pesquise bandas cadastradas
- 📝 **Alteração de Dados** - Edite informações de bandas existentes
- 🗑️ **Remoção de Bandas** - Exclua registros do sistema
- 🎵 **Gerenciamento de Gêneros** - Adicione novos gêneros musicais
- 📊 **Visualização em Lista** - Veja todas as bandas cadastradas

## 🎨 Interface

O sistema possui uma interface com navegação por abas:

- **Aba Cadastro** - Formulário para inserir novas bandas
- **Aba Busca** - Interface para pesquisar e visualizar bandas cadastradas

A navegação é facilitada por botões laterais com indicador visual de aba selecionada.


## 📝 Licença

Este projeto é um trabalho acadêmico desenvolvido para fins educacionais.

## 👥 Autor

Desenvolvido como projeto da disciplina de Linguagens e Técnicas Avançadas de Programação

---

**Nota**: Este é um projeto modelo para fins educacionais. Certifique-se de implementar as validações e tratamento de erros adequados antes de usar em produção.
