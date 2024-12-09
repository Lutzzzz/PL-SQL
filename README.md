# Projeto de Pacotes PL/SQL - Gestão Acadêmica

Este repositório contém o código de pacotes PL/SQL para gerenciar operações acadêmicas em um banco de dados, como a exclusão de alunos, gerenciamento de turmas, disciplinas e professores. O código foi escrito para ser executado em um ambiente Oracle.

## Estrutura do Repositório

- `pacotes.sql`: Contém todos os pacotes PL/SQL e seus respectivos corpos.
- `README.md`: Este arquivo com instruções e explicações sobre os pacotes.

## Pré-requisitos

- Banco de dados Oracle 11g ou superior.
- O banco de dados deve ter as seguintes tabelas criadas:
  - `Aluno`
  - `Matricula`
  - `Disciplina`
  - `Professor`
  - `Turma`

Essas tabelas devem ser configuradas corretamente para que as procedures e funções funcionem sem erros.

## Como Executar o Script

1. **Conectar-se ao Oracle**: Use uma ferramenta de administração de banco de dados como SQL*Plus, SQLcl ou SQL Developer para conectar-se ao seu banco de dados Oracle.

2. **Carregar o Script**:
   - Abra o arquivo `pacotes.sql` e execute o código no seu ambiente Oracle.
   - Certifique-se de que as tabelas estão criadas e que o esquema do banco de dados está configurado corretamente.

3. **Executar Procedures e Funções**:
   - Após executar o script de pacotes, você pode testar as funções e procedures usando os seguintes comandos SQL:

### Exemplos de Execução

#### 1. Listar Turmas por Professor:
   ```sql
   EXEC PKG_PROFESSOR.listar_total_turmas_por_professor;
