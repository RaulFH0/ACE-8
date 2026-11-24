# Sistema MEI Social — Gestão de Produtos e Estoque

## Sobre o projeto

Projeto da Atividade Curricular de Extensão (ACE 8), da disciplina Análise e Projeto de Sistemas II, do curso de Sistemas de Informação da UniCatólica — 2026.2.

O MVP busca auxiliar pequenos empreendimentos na organização de produtos e no controle de estoque.

**Instituição parceira:** Brilhante Farma — Capistrano/CE.

## Funcionalidades

- Cadastro e consulta de produtos.
- Pesquisa de produtos por nome.
- Atualização de estoque.
- Definição de estoque mínimo.
- Identificação de produtos para reposição.
- Catálogo público de produtos.
- Isolamento de produtos por estabelecimento.

## Tecnologias utilizadas

- Python, FastAPI, SQLAlchemy, SQLite e Pydantic.
- React, TypeScript e Vite.
- Pytest, Git e GitHub.

## Arquitetura e modelagem

O sistema utiliza arquitetura em camadas, separando interface, API, validação e persistência.

A modelagem contempla diagramas UML de casos de uso, classes e sequência, princípios SOLID e GRASP e estudo dos padrões GoF.

## Endpoints da API

| Método | Endpoint | Descrição |
|---|---|---|
| GET | /mei/produtos | Listar produtos |
| GET | /mei/produtos/buscar | Buscar produtos |
| POST | /mei/produtos | Cadastrar produto |
| PATCH | /mei/produtos/{produto_id}/estoque | Atualizar estoque |
| PATCH | /mei/produtos/{produto_id}/estoque-minimo | Definir estoque mínimo |
| GET | /lojas/{slug}/produtos | Catálogo público |

## Execução local

### Backend

Utilize Python 3.11 em um ambiente virtual.

- Instalar dependências: `python -m pip install -r requirements.txt`
- Iniciar API: `python -m uvicorn main:app --host 127.0.0.1 --port 8000`
- Swagger: http://127.0.0.1:8000/docs

### Frontend

- Acessar a pasta: `cd frontend`
- Instalar dependências: `npm install`
- Iniciar aplicação: `npm run dev`

Acesse o endereço informado pelo Vite.

## Testes automatizados

Em 23/11/2026, foram executados 26 testes automatizados, todos aprovados.

**Resultado: 26 passed in 65.23s.**

Os testes avaliaram estoque, estoque mínimo e isolamento de produtos entre estabelecimentos.

## Aplicação prática

A proposta de extensão contempla a demonstração do MVP na Brilhante Farma, apresentando funcionalidades de cadastro de produtos, controle de estoque e identificação de itens para reposição.

As evidências da atividade prática integram o relatório acadêmico.

## Repositório

https://github.com/RaulFH0/ACE-8

O projeto reaproveita funcionalidades do Sistema MEI, mantendo uma versão independente para a atividade de extensão.

---

**UniCatólica — ACE 8 — 2026.2**
