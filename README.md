# sml-bank-back-end

- Aplicação de internet banking. 

## Fluxo de Controle de Versão Git

> #### MAIN
* Branch que contém todo código em produção.
* Não é commitada diretamente.

> #### DEVELOP
* Uma ramificação da main, é usada para criar branches de novas features.
* Features finalizadas, são mescladas a ela.
* A partir dela se cria uma release, como nova versão.

> #### FEATURE
* Branch para desenvolvimento de uma nova funcionalidade.
* Criada a partir da developmente, após finalizada é mesclada a development novamente.

> #### RELEASE
* Branch que contém um ciclo de lançamento.
* Criada a partir da development, quando esta possuir uma ou mais novas features finalizadas.
* Nela só são realizadas alterações de segurança, documentação ou correção de bugs, não recebendo novas funcionalidades.
* Após validada, é mesclada a main, criando uma nova versão do sistema.

> #### HOTFIX
* Branch usada para correções do código em produção.
* Criada a partir da main, após corrigidos os erros é mesclada a main e a branch develop, adicionando a main um número de versão atualizado.

> #### RESUMO FLUXO
* main => develop => feature | feature => develop => release => main
* main => hotfix | hotfix => main / develop / release

> #### PADRÕES DE NOMENCLATURA DOS COMMITS
* feat: Descrição de nova feature.
* fix: Descrição de correção de erro.
* docs: Descrição de documentação, readme, etc.
* test: Descrição de teste.
* build: Descrição de alterações em arquivos de build ou dependências.
* perf: Descrição para alterações de performance.
* style: Descrição para alterações em estilização.
* refactor: Descrição de refatoração de código.
* chore: Descrição para atualizações de buid, configurações, gitignore, etc.
* ci: Descrição de alterações de integração contínua.

## Tecnologias
* NodeJs
* Javascript
* Express
* Sequelize
* MySql

## Execução do Sistema

> #### INSTALAR DEPENDÊNCIAS DO PROJETO

```
npm install
```

> #### RODAR SERVIDOR

```
npm run dev
```