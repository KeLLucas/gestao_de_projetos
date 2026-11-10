# EAP — Estrutura Analítica do Projeto

---

## Identificação

| Campo | Informação |
| --- | --- |
| **Projeto** | FieldOps — Plataforma de Inspeção em Campo |
| **Gerente do projeto** | DevOps |
| **Patrocinador** | Instituição |
| **Data** | 04/11/2026 |
| **Versão** | 1.0 |
| **Prazo previsto** | Até o final do semestre |
| **Orçamento** | Sem orçamento formal definido |

---

## Estrutura Analítica do Projeto

```text
FIELDOPS — PLATAFORMA DE INSPEÇÃO EM CAMPO
│
├── 1. GESTÃO E DOCUMENTAÇÃO DO PROJETO
│   ├── 1.1 Termo de Abertura do Projeto (TAP)
│   ├── 1.2 Backlog e requisitos do produto
│   └── 1.3 Repositórios e documentação de desenvolvimento
│
├── 2. API / BACKEND
│   ├── 2.1 Serviços de cadastros operacionais
│   ├── 2.2 Serviços de modelos de inspeção
│   └── 2.3 Serviços de planejamento e execução de inspeções
│
├── 3. PAINEL ADMINISTRATIVO
│   ├── 3.1 Interfaces de clientes, locais e equipamentos
│   ├── 3.2 Gestão de modelos de inspeção
│   └── 3.3 Planejamento e acompanhamento de inspeções
│
├── 4. APLICATIVO MÓVEL
│   ├── 4.1 Execução de inspeções em campo
│   ├── 4.2 Identificação de equipamentos por QR Code
│   └── 4.3 Registro e envio de evidências
│
└── 5. INTEGRAÇÃO, QUALIDADE E ENTREGA
    ├── 5.1 Integração entre API, painel administrativo e aplicativo
    ├── 5.2 Validação automatizada e testes
    └── 5.3 Documentação final e entrega do produto
```

---

## Dicionário da EAP

| Código | Elemento | Descrição |
| --- | --- | --- |
| 1.0 | Gestão e documentação do projeto | Artefatos necessários para orientar, organizar e registrar o projeto FieldOps. |
| 1.1 | Termo de Abertura do Projeto (TAP) | Documento que formaliza o projeto, sua justificativa, objetivos, responsáveis, prazo, premissas e restrições. |
| 1.2 | Backlog e requisitos do produto | Conjunto organizado de épicos e histórias de usuário que descrevem as funcionalidades e necessidades do FieldOps. |
| 1.3 | Repositórios e documentação de desenvolvimento | Repositórios da API, do aplicativo móvel e do painel administrativo, acompanhados de README e orientações de desenvolvimento e contribuição. |
| 2.0 | API / Backend | Serviços de backend responsáveis por disponibilizar e integrar os dados e as regras necessárias aos componentes do FieldOps. |
| 2.1 | Serviços de cadastros operacionais | Recursos da API relacionados ao cadastro de clientes, locais vinculados a clientes, equipamentos vinculados a locais, QR Code único por equipamento e pesquisa dos registros. |
| 2.2 | Serviços de modelos de inspeção | Recursos da API relacionados à estruturação dos modelos, seções, itens, respostas, obrigatoriedade, evidências, prévia, publicação e registro da versão publicada. |
| 2.3 | Serviços de planejamento e execução de inspeções | Recursos da API relacionados ao agendamento, seleção de cliente/local/equipamento, atribuição, prioridade, prazo, instruções, cancelamento e dados necessários ao acompanhamento e à execução. |
| 3.0 | Painel administrativo | Interface web destinada à administração e supervisão das informações e inspeções do FieldOps. |
| 3.1 | Interfaces de clientes, locais e equipamentos | Telas para consultar e administrar clientes, seus locais e os equipamentos associados, incluindo identificação por QR Code e recursos de pesquisa. |
| 3.2 | Gestão de modelos de inspeção | Interfaces para criar e organizar modelos, seções e itens, definir respostas e evidências, visualizar a prévia e publicar modelos. |
| 3.3 | Planejamento e acompanhamento de inspeções | Interfaces para agendar inspeções, selecionar os registros relacionados, atribuir responsáveis, definir prioridade e prazo, cancelar e acompanhar inspeções com filtros. |
| 4.0 | Aplicativo móvel | Aplicativo utilizado pelos técnicos para consultar e executar inspeções em campo. |
| 4.1 | Execução de inspeções em campo | Recursos móveis para baixar e visualizar inspeções, filtrar a lista, iniciar a execução, apresentar checklist dinâmico, registrar respostas, salvar informações localmente, acompanhar o progresso, adicionar observações e concluir a inspeção. |
| 4.2 | Identificação de equipamentos por QR Code | Recurso de leitura de QR Code para confirmar o equipamento relacionado à inspeção. |
| 4.3 | Registro e envio de evidências | Recursos para capturar fotos e visualizar prévias, associar evidências, tratar envios pendentes, registrar localização e não conformidades e acompanhar evidências. |
| 5.0 | Integração, qualidade e entrega | Entregáveis que permitem verificar o funcionamento conjunto dos componentes e preparar o resultado do projeto. |
| 5.1 | Integração entre API, painel administrativo e aplicativo | Comunicação integrada entre os três componentes do FieldOps para disponibilizar dados e funcionalidades aos seus usuários. |
| 5.2 | Validação automatizada e testes | Verificações de qualidade e testes dos componentes e de suas integrações, incluindo validações automatizadas configuradas nos repositórios. |
| 5.3 | Documentação final e entrega do produto | Documentação consolidada do projeto e versão integrada do FieldOps preparada para apresentação e entrega acadêmica. |

---

## Orientações

A **EAP (Estrutura Analítica do Projeto)** representa uma decomposição hierárquica do escopo do FieldOps. A estrutura está organizada em três níveis:

- **Nível 1 — Projeto:** FieldOps — Plataforma de Inspeção em Campo.
- **Nível 2 — Entregas:** grandes componentes e resultados do projeto.
- **Nível 3 — Pacotes de trabalho:** partes menores e verificáveis de cada entrega.

A EAP descreve **o que será entregue**, não a sequência de atividades que a equipe deverá executar.

### Premissas consideradas

- O FieldOps é composto por três componentes: API, aplicativo móvel para técnicos e painel administrativo para administradores/supervisores.
- O patrocinador indicado no TAP é a instituição.
- A responsabilidade de gerenciamento do projeto está atribuída ao papel de DevOps.
- O prazo previsto é até o final do semestre.
- Não há orçamento formal definido.
- Os usuários do sistema considerados no TAP são os técnicos; o painel também contempla o uso administrativo e de supervisão.

### Limites e pontos a confirmar

Esta versão utiliza as informações e histórias de usuário do FieldOps já definidas nas conversas e nos artefatos mencionados. Os pacotes funcionais detalhados refletem especialmente os épicos conhecidos de cadastros operacionais, modelos de inspeção, planejamento, execução de campo e recursos nativos/evidências.

A descrição dos serviços internos da API foi organizada para representar as capacidades correspondentes a essas funcionalidades. A divisão técnica final entre API, painel e aplicativo deve ser conferida com os respectivos times e com o backlog atualizado. Itens ainda não especificados no material disponível não foram inventados nesta EAP.

---

## Checklist

- [x] O projeto está representado no nível superior.
- [x] As principais entregas foram identificadas.
- [x] As entregas foram decompostas em pacotes de trabalho.
- [x] A estrutura possui três níveis.
- [x] Os elementos possuem códigos.
- [x] A EAP representa entregas, e não uma lista de tarefas.
- [x] O dicionário da EAP foi preenchido.
- [x] A estrutura foi revisada e aprovada pela equipe.

---
