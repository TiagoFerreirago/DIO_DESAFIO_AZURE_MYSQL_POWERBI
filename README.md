# Integrando Dados com MySQL na Azure e Transformando com Power BI

Desafio de projeto que une **banco de dados na nuvem** e **transformação de dados**: criação de uma instância MySQL na Azure, o schema de uma base disponível no GitHub, conexão com o Power BI e tratamento dos dados no Power Query.

## Objetivo

1. Criar uma instância do **MySQL na Azure**.
2. Criar o banco de dados com base na base disponível no GitHub.
3. Integrar o **Power BI** com o MySQL na Azure.
4. Verificar problemas na base e realizar a **transformação dos dados**.

## Tecnologias utilizadas

- Microsoft Azure (Azure Database for MySQL)
- Azure Cloud Shell
- MySQL Workbench
- Power BI Desktop (Power Query)
- SQL

## Etapas do desafio

1. **Descrevendo o desafio de projeto**
2. **Criando uma instância do MySQL na Azure**
3. **Explorando o recurso**: visão geral da instância do MySQL
4. **Conectando ao banco de dados com o Cloud Shell**
5. **Criando regra no firewall da Azure** para permitir o acesso ao banco de dados
6. **Conectando ao MySQL na Azure com o Workbench**
7. **Integrando o Power BI com o MySQL na Azure**

## Mesclar vs. Acrescentar

Neste caso podemos usar apenas **Mesclar**, e não **Acrescentar**, porque:

- A **mesclagem** compara colunas de duas tabelas (chaves) e permite escolher o tipo de junção, agregando informações de tabelas diferentes que se relacionam. É o que precisamos para trazer o nome do departamento para a tabela de colaboradores.
- O **acrescentar** adiciona os dados de duas tabelas na **vertical** (empilha linhas), o que só faz sentido quando as tabelas compartilham a mesma estrutura de colunas. Não é o caso de `employee` e `department`.

## Como reproduzir

1. Crie uma instância do **Azure Database for MySQL** no portal da Azure.
2. Crie uma **regra de firewall** liberando o seu IP.
3. Conecte-se pelo **Cloud Shell** ou pelo **MySQL Workbench**.
4. Execute os scripts da base disponível no GitHub para criar e popular o banco.
5. No Power BI Desktop, escolha **Obter dados > Banco de dados MySQL** e informe servidor e credenciais.
6. Aplique as transformações descritas neste README no Power Query.

## Autor

#### Github: https://github.com/TiagoFerreirago

#### Linkedin: https://www.linkedin.com/in/tiagoferreira97/
