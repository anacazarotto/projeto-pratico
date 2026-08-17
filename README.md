# Projeto Prático — Gerência e Configuração de Software

Projeto desenvolvido como atividade prática da disciplina **Gerência e Configuração de Software**, com o objetivo de aplicar conceitos de **Git, GitHub, controle de versão, branches, commits, Pull Requests, merge e Versionamento Semântico**.

## 📚 Disciplina

**Gerência e Configuração de Software**

**Avaliação:** A1/1 — Avaliação Prática

## 🎯 Objetivo

Este projeto tem como objetivo demonstrar, na prática, a utilização de ferramentas e conceitos relacionados ao gerenciamento e à configuração de software, utilizando o **Git** para controle de versão e o **GitHub** para gerenciamento do repositório remoto.

Durante o desenvolvimento da atividade foram aplicados conceitos como:

* Criação e configuração de um repositório GitHub;
* Clonagem de um repositório;
* Criação e utilização de branches;
* Padronização de branches utilizando `feature/{identificador}`;
* Criação de commits;
* Envio de alterações para o repositório remoto;
* Criação e revisão de Pull Requests;
* Merge de branches;
* Criação e utilização de tags;
* Versionamento Semântico.

## 🌱 Estratégia de Branches

Para o desenvolvimento de novas funcionalidades, foi utilizada a seguinte convenção para nomeação de branches:

```text
feature/{identificador}
```

Exemplo:

```text
feature/ana
```

A branch de funcionalidade é utilizada para realizar alterações de forma isolada e, posteriormente, integrar essas alterações à branch principal por meio de um **Pull Request**.

## 🔄 Fluxo de Desenvolvimento

O fluxo utilizado no projeto segue, de forma geral, as seguintes etapas:

```text
main
  │
  └── feature/{identificador}
          │
          ├── Alterações
          ├── Commit
          └── Push
                │
                ▼
        Pull Request
                │
                ▼
             Merge
                │
                ▼
              main
                │
                ▼
          Tag de versão
```

Esse fluxo permite manter a branch principal organizada e possibilita a revisão das alterações antes da integração.

## 🏷️ Versionamento Semântico

O **Versionamento Semântico (Semantic Versioning)** é uma convenção utilizada para identificar versões de um software de maneira padronizada.

As versões seguem o formato:

```text
MAJOR.MINOR.PATCH
```

Por exemplo:

```text
1.0.0
```

### MAJOR

O número **MAJOR** deve ser incrementado quando são realizadas alterações incompatíveis com versões anteriores.

Exemplo:

```text
1.0.0 → 2.0.0
```

### MINOR

O número **MINOR** deve ser incrementado quando uma nova funcionalidade é adicionada mantendo a compatibilidade com a versão anterior.

Exemplo:

```text
1.0.0 → 1.1.0
```

### PATCH

O número **PATCH** deve ser incrementado quando são realizadas correções de erros ou pequenas alterações compatíveis com a versão existente.

Exemplo:

```text
1.0.0 → 1.0.1
```

### Primeira versão

Para representar a primeira versão estável do projeto, foi utilizada a versão:

```text
v1.0.0
```

A tag `v1.0.0` representa a primeira versão do projeto após a realização das alterações e integração na branch `main`.

## 📌 Conceitos Aplicados

| Conceito            | Aplicação                                       |
| ------------------- | ----------------------------------------------- |
| Git                 | Controle de versão do projeto                   |
| GitHub              | Hospedagem e gerenciamento do repositório       |
| Branch              | Desenvolvimento isolado de funcionalidades      |
| Commit              | Registro das alterações realizadas              |
| Push                | Envio das alterações para o repositório remoto  |
| Pull Request        | Revisão e integração das alterações             |
| Merge               | Integração da branch de funcionalidade à `main` |
| Tag                 | Identificação de uma versão específica          |
| Semantic Versioning | Padronização das versões do projeto             |

## 🎓 Considerações

A atividade possibilitou a aplicação prática dos principais conceitos de **Gerência e Configuração de Software**, permitindo compreender o fluxo de trabalho utilizando Git e GitHub, desde a criação e desenvolvimento em uma branch até a integração das alterações na branch principal e a identificação de uma versão por meio de uma tag.

O repositório também permite verificar o histórico de commits, branches, Pull Requests, merges e versões criadas durante a realização da atividade.

## 👩‍💻 Autora

**Ana Carla Londero Cazarotto**

Projeto desenvolvido para fins acadêmicos na disciplina de **Gerência e Configuração de Software**.

## Versionamento Semântico

Este projeto segue as práticas de **Versionamento Semântico (SemVer)**, 
um padrão amplamente utilizado para versionar software de forma clara e previsível.

O número de versão segue o formato: **MAJOR.MINOR.PATCH** (ex: 1.0.0)

- **MAJOR**: incrementado quando são feitas alterações incompatíveis com 
  versões anteriores (breaking changes), ou seja, mudanças que quebram 
  a compatibilidade com quem já usa o projeto.
- **MINOR**: incrementado quando novas funcionalidades são adicionadas 
  de forma compatível com versões anteriores (sem quebrar nada que já existia).
- **PATCH**: incrementado quando são feitas correções de bugs que também 
  são compatíveis com versões anteriores.

Exemplo: ao sair de `1.0.0` para `1.1.0`, uma nova funcionalidade foi 
adicionada sem quebrar nada. Ao sair de `1.1.0` para `2.0.0`, houve uma 
mudança que quebra a compatibilidade com a versão anterior.

## Funcionalidade: Cadastro e Autenticação de Usuários (API v2)

Esta funcionalidade foi reestruturada para unificar cadastro e autenticação 
em um único fluxo, alterando o formato anterior de endpoints e removendo 
compatibilidade com a versão anterior da API.