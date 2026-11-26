# MedSinc

**Sistema web para gestão de plantões médicos | TCC de Ciência da Computação na UNIP**

O MedSinc reúne agenda, oportunidades de plantão e acompanhamento financeiro em uma única interface. Foi desenvolvido em equipe como Trabalho de Conclusão de Curso. Esta página apresenta o projeto e reúne o acesso ao código e à documentação técnica.

## O que o sistema faz

| Módulo | Funcionalidade |
| --- | --- |
| Agenda de plantões | Organiza os plantões cadastrados e permite acompanhar a agenda. |
| Marketplace | Centraliza oportunidades de plantão e candidaturas. |
| Finanças | Registra e acompanha informações financeiras, incluindo gastos. |
| Pacientes e atendimentos | Organiza os registros de pacientes e atendimentos. |
| Conta e notificações | Gerencia a autenticação e as notificações do sistema. |

## Arquitetura e código-fonte

A interface web consome a API Flask para executar as operações do sistema. A API separa rotas HTTP, regras de negócio e acesso ao banco. Os dados são persistidos em MySQL, com modelos SQLAlchemy e migrações Alembic.

| Componente | Tecnologias | Repositório original |
| --- | --- | --- |
| Interface web | React, TypeScript, Vite, Tailwind CSS e Recharts | [Frontend](https://github.com/HierroPagotto/plantaoMedicoFinance) |
| API e persistência | Python, Flask, SQLAlchemy, Alembic e MySQL | [Backend](https://github.com/HierroPagotto/MedSincBackend) |

## Como executar localmente

1. **Banco de dados.** Instale o MySQL 8 e crie um banco local para o projeto.
2. **Backend.** Com Python 3.10 ou superior, instale as dependências com `pip install -r requirements.txt`. Preencha as variáveis locais seguindo o [guia do backend](https://github.com/HierroPagotto/MedSincBackend#configuração) e inicie a API com `python run.py`.
3. **Frontend.** Com Node.js 20 ou superior, instale as dependências com `npm install`. Configure o endereço da API conforme o [guia do frontend](https://github.com/HierroPagotto/plantaoMedicoFinance#configuração) e execute `npm run dev`.

## Créditos

TCC desenvolvido em equipe no curso de Ciência da Computação da Universidade Paulista (UNIP). Os repositórios originais estão na conta de [Hierro Pagotto](https://github.com/HierroPagotto) e registram o histórico do código. [Rian Nascimento Fagundes](https://github.com/RianNFagundes) integrou a equipe do projeto.
