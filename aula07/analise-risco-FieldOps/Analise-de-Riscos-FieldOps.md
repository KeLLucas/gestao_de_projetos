# Análise de Riscos — FieldOps

## 1. Identificação

| Campo | Informação |
| --- | --- |
| **Projeto** | FieldOps — Plataforma de Inspeção em Campo |
| **Patrocinador** | Instituição |
| **Gerente do projeto** | DevOps |
| **Prazo de referência** | Semestre letivo |
| **Orçamento** | Não há orçamento formal aprovado |
| **Público usuário** | Técnicos que realizam inspeções em campo |
| **Data de elaboração** | 04/11/2026 |
| **Versão** | 1.0 |
| **Status** | Proposta para validação da equipe |

## 2. Objetivo e abordagem do gerenciamento de riscos

O objetivo deste documento é identificar eventos incertos que possam afetar o escopo, o prazo, a qualidade, os custos ou a entrega do FieldOps, avaliar sua importância e definir respostas preventivas e contingenciais.

O gerenciamento será realizado de forma contínua:

1. Identificar riscos durante o planejamento, desenvolvimento, integração e validação.
2. Registrar cada risco descrevendo sua causa, o evento incerto e a consequência.
3. Avaliar probabilidade e impacto para estabelecer a prioridade.
4. Definir uma estratégia de resposta e um responsável por acompanhar cada risco.
5. Revisar o registro periodicamente e sempre que houver mudança relevante no projeto.
6. Registrar novos riscos, alterações de prioridade e a eficácia das respostas.

**Responsável pela coordenação:** Gerente do Projeto (DevOps).
**Participação:** responsáveis pelas equipes de API, Mobile, Painel Administrativo e Qualidade, além do Product Owner/representante do produto.

## 3. Critérios de avaliação

### 3.1 Probabilidade

| Nível | Valor | Interpretação |
| --- | ---: | --- |
| Muito baixa | 0,10 | Pouco provável durante o projeto |
| Baixa | 0,20 | Pode ocorrer, mas não é esperado |
| Média | 0,30 | Existe possibilidade relevante de ocorrência |
| Alta | 0,50 | É provável que ocorra |
| Muito alta | 0,80 | Há forte possibilidade de ocorrência |

### 3.2 Impacto

Para esta análise, o impacto é pontuado de 1 a 5 em cada objetivo. A escala foi adaptada ao contexto e à dimensão acadêmica do FieldOps.

| Nível | Pontuação | Interpretação |
| --- | ---: | --- |
| Muito baixo | 1 | Efeito localizado, facilmente corrigido, sem alteração relevante na entrega |
| Baixo | 2 | Pequeno retrabalho ou atraso absorvível pela equipe |
| Moderado | 3 | Afeta uma funcionalidade ou etapa e exige replanejamento |
| Alto | 4 | Compromete uma entrega importante, exige retrabalho significativo ou ameaça o prazo |
| Muito alto | 5 | Pode impedir uma funcionalidade essencial ou comprometer a entrega do projeto |

Os impactos são avaliados em quatro dimensões: **custo, prazo, escopo e qualidade**.

### 3.3 Cálculo da severidade e prioridade

- **Impacto médio:** média das pontuações de custo, prazo, escopo e qualidade.
- **Severidade:** probabilidade × impacto médio.
- **Prioridade:** classificação da severidade para orientar o tratamento.

| Severidade | Prioridade | Tratamento |
| ---: | --- | --- |
| Igual ou superior a 2,00 | Alta | Definir resposta e acompanhar em toda reunião de status |
| De 1,00 a 1,99 | Média | Definir resposta e revisar periodicamente |
| Inferior a 1,00 | Baixa | Monitorar; agir se houver mudança de probabilidade ou impacto |

> A fórmula e os limites acima são critérios adotados para esta análise do FieldOps. A apresentação da Aula 07 demonstra a combinação de probabilidade e impacto para calcular a severidade e ordenar os riscos; os limites devem ser ajustados se o professor ou a equipe estabelecerem outra escala.

## 4. Registro e análise qualitativa dos riscos

Na descrição de cada risco:

- **Causa:** condição que pode originar o risco.
- **Risco:** evento incerto que pode acontecer.
- **Consequência:** efeito possível nos objetivos do projeto.

| ID | Causa | Risco (evento incerto) | Consequência | Prob. | Custo | Prazo | Escopo | Qualidade | Impacto médio | Severidade | Prioridade |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- |
| R01 | Requisitos ou critérios de aceite ainda não validados por todos os envolvidos | Mudanças relevantes de escopo durante o desenvolvimento | Retrabalho, aumento de esforço e atraso nas entregas | 0,50 | 3 | 4 | 5 | 3 | 3,75 | 1,88 | Média |
| R02 | Disponibilidade limitada dos integrantes e conciliação com atividades acadêmicas | Responsáveis não conseguirem dedicar o tempo previsto às tarefas | Atividades acumuladas e atraso no cronograma | 0,50 | 2 | 5 | 4 | 3 | 3,50 | 1,75 | Média |
| R03 | Contratos, formatos de dados ou decisões técnicas divergentes entre API, Mobile e Painel | Componentes não se integrarem corretamente | Retrabalho de integração e atraso na homologação | 0,50 | 3 | 4 | 4 | 5 | 4,00 | 2,00 | Alta |
| R04 | Condições de iluminação, câmera, impressão ou posicionamento do QR Code | Leitura do QR Code falhar em parte dos equipamentos ou ambientes | Técnico não conseguir confirmar o equipamento com confiabilidade | 0,30 | 2 | 3 | 4 | 4 | 3,25 | 0,98 | Baixa |
| R05 | Conectividade instável em locais de inspeção e dependência de envio ao servidor | Fotos ou evidências não serem enviadas corretamente | Perda ou atraso no registro de evidências e necessidade de repetir a operação | 0,50 | 3 | 4 | 4 | 5 | 4,00 | 2,00 | Alta |
| R06 | Regras de sincronização offline ainda não definidas ou testadas | Dados locais entrarem em conflito, duplicarem ou não sincronizarem | Registros inconsistentes e perda de informações de inspeção | 0,30 | 3 | 4 | 5 | 5 | 4,25 | 1,28 | Média |
| R07 | Falhas na autenticação, autorização ou validação de permissões | Usuário acessar dados ou operações que não deveria | Exposição ou alteração indevida de informações | 0,20 | 4 | 4 | 5 | 5 | 4,50 | 0,90 | Baixa |
| R08 | Tratamento inadequado de dados pessoais, imagens ou localização | Dados serem coletados, armazenados ou compartilhados sem os cuidados necessários | Risco de privacidade, necessidade de correção e perda de confiança | 0,20 | 3 | 4 | 4 | 5 | 4,00 | 0,80 | Baixa |
| R09 | Ambiente de desenvolvimento, banco de dados ou configuração de execução divergente entre integrantes | Aplicação funcionar em um ambiente e falhar em outro | Tempo gasto em configuração e atraso no desenvolvimento/testes | 0,30 | 2 | 3 | 3 | 4 | 3,00 | 0,90 | Baixa |
| R10 | Cobertura insuficiente de testes e validação tardia das funcionalidades | Defeitos importantes serem descobertos somente na integração ou apresentação | Correções urgentes, regressões e redução da qualidade | 0,50 | 3 | 4 | 4 | 5 | 4,00 | 2,00 | Alta |
| R11 | Dependência de bibliotecas, serviços ou ferramentas externas | Dependência apresentar incompatibilidade, indisponibilidade ou mudança relevante | Substituição técnica, retrabalho e possível atraso | 0,20 | 2 | 3 | 3 | 4 | 3,00 | 0,60 | Baixa |
| R12 | Falta de validação com técnicos ou representantes do público usuário | Fluxos desenvolvidos não atenderem às necessidades reais de inspeção | Baixa usabilidade e necessidade de alterar telas ou processos | 0,30 | 2 | 4 | 4 | 4 | 3,50 | 1,05 | Média |
| R13 | Cronograma acadêmico limitado e dependências entre equipes | Integração e homologação não serem concluídas antes do prazo final | Entrega incompleta ou redução do tempo para validação | 0,50 | 2 | 5 | 4 | 4 | 3,75 | 1,88 | Média |
| R14 | Documentação técnica e decisões não serem atualizadas junto com o código | Equipes trabalharem com instruções desatualizadas ou diferentes | Erros de integração, retrabalho e dificuldade de manutenção | 0,30 | 2 | 3 | 3 | 4 | 3,00 | 0,90 | Baixa |
| R15 | Mudanças serem feitas sem revisão adequada ou sem execução dos checks de CI | Alteração com defeito ser integrada à branch principal | Instabilidade da aplicação e regressões | 0,30 | 2 | 3 | 3 | 5 | 3,25 | 0,98 | Baixa |

### 4.1 Principais riscos priorizados

Com base na severidade estimada, os riscos classificados como **altos** são:

- **R03 — Falha de integração entre componentes:** pode afetar simultaneamente API, Mobile e Painel Administrativo.
- **R05 — Falha no envio de evidências:** pode comprometer o registro de fotos e a conclusão de inspeções.
- **R10 — Defeitos descobertos tardiamente:** pode reduzir o tempo disponível para correção e homologação.

Os riscos de prioridade média também precisam de acompanhamento, especialmente mudanças de escopo (R01), disponibilidade da equipe (R02), sincronização offline (R06), validação com usuários (R12) e prazo acadêmico (R13).

**Atenção:** a prioridade é resultado da escala estimada, não uma garantia de que um risco de prioridade baixa seja inofensivo. Riscos de segurança e privacidade devem ser acompanhados mesmo quando a multiplicação resultar em severidade menor.

## 5. Planejamento das respostas aos riscos

As respostas seguem as quatro abordagens apresentadas na Aula 07: evitar, transferir, mitigar e aceitar. Para os riscos do FieldOps, a mitigação é a abordagem mais utilizada, pois permite reduzir a probabilidade ou o impacto sem retirar funcionalidades essenciais do escopo.

| ID | Abordagem | Ação preventiva / resposta planejada | Plano de contingência ou reação | Responsável pelo acompanhamento |
| --- | --- | --- | --- | --- |
| R01 | Mitigar | Validar requisitos e critérios de aceite antes de iniciar cada funcionalidade; registrar mudanças no backlog e avaliar impacto em prazo e escopo | Repriorizar o backlog e submeter mudanças relevantes à aprovação do responsável pelo produto e do gerente do projeto | Product Owner / Gerente do Projeto |
| R02 | Mitigar | Dividir tarefas em entregas menores, explicitar responsáveis e revisar capacidade da equipe a cada sprint | Redistribuir tarefas, reduzir trabalho em andamento e renegociar prioridades | Gerente do Projeto / líderes de equipe |
| R03 | Mitigar | Definir contratos de API, formatos de dados, convenções e exemplos de integração antes da implementação conjunta; realizar integração incremental | Isolar a interface com contrato temporário documentado, corrigir incompatibilidades e replanejar a integração | Responsáveis API, Mobile e Admin |
| R04 | Mitigar | Testar leitura com diferentes câmeras, distâncias, iluminação e qualidade de impressão; prever identificação manual como alternativa, se aprovada | Permitir localizar o equipamento por identificador alternativo definido pelo produto e registrar a falha para correção | Equipe Mobile / API |
| R05 | Mitigar | Validar tamanho e formato de imagem, tratar falhas de rede, indicar estado do envio e preservar evidência pendente até confirmação do servidor | Manter evidência na fila local, informar o técnico e tentar novo envio quando houver conexão | Equipe Mobile / API |
| R06 | Mitigar | Definir identificadores únicos, estados de sincronização, regras de conflito e testes de reconexão antes de liberar o fluxo offline | Preservar cópias locais, registrar conflito para resolução controlada e evitar sobrescrita silenciosa | Equipe Mobile / API |
| R07 | Mitigar | Definir perfis e permissões, validar autorização no backend, revisar endpoints e testar acesso indevido | Revogar credenciais ou permissões afetadas, corrigir a falha e revisar registros de acesso disponíveis | Equipe API / responsável por segurança |
| R08 | Mitigar | Mapear dados pessoais tratados, limitar coleta ao necessário, restringir acesso e definir armazenamento e retenção de imagens/localização | Suspender o fluxo afetado, restringir acesso e comunicar os responsáveis do projeto para avaliação e correção | Gerente do Projeto / API / Mobile |
| R09 | Mitigar | Documentar configuração, padronizar variáveis de ambiente e usar instruções reproduzíveis para executar e testar os componentes | Recriar o ambiente seguindo a documentação e corrigir diferenças de configuração | DevOps / equipes técnicas |
| R10 | Mitigar | Planejar testes por funcionalidade, automatizar validações possíveis e testar continuamente durante o desenvolvimento | Priorizar correção de defeitos que bloqueiam fluxos essenciais e executar regressão antes da entrega | QA / responsáveis de cada componente |
| R11 | Mitigar | Avaliar dependências antes de adotá-las, fixar versões e documentar alternativas técnicas | Substituir a dependência ou implementar alternativa compatível, avaliando impacto no cronograma | Equipe técnica responsável |
| R12 | Mitigar | Validar protótipos e fluxos com representantes dos usuários antes de concluir as telas e regras | Ajustar os fluxos prioritários e registrar funcionalidades não essenciais para avaliação posterior | Product Owner / equipe Admin e Mobile |
| R13 | Mitigar | Acompanhar marcos e dependências semanalmente; reservar tempo para integração, testes e correções | Priorizar o caminho crítico e as funcionalidades essenciais, negociando escopo quando necessário | Gerente do Projeto / líderes |
| R14 | Mitigar | Atualizar README, documentação técnica e decisões junto com mudanças relevantes; revisar documentação em PRs | Realizar revisão concentrada da documentação e comunicar as correções às equipes | DevOps / responsáveis técnicos |
| R15 | Mitigar | Exigir Pull Request, revisão, checks automatizados e proteção da branch principal | Reverter a alteração problemática, corrigir em nova branch e executar novamente os checks | DevOps / revisores do PR |

## 6. Monitoramento e controle dos riscos

O registro de riscos deve ser revisado durante todo o ciclo de vida do FieldOps.

| Atividade de controle | Frequência sugerida | Responsável | Evidência |
| --- | --- | --- | --- |
| Revisar riscos altos e mudanças de prioridade | Em cada reunião de acompanhamento | Gerente do Projeto e responsáveis | Atualização do registro de riscos |
| Verificar riscos técnicos de integração, evidências e sincronização | A cada sprint e integração relevante | API, Mobile, Admin e QA | Resultados de testes e issues |
| Verificar riscos de qualidade e regressão | A cada Pull Request e ciclo de testes | QA e revisores | Checks de CI, testes e PRs |
| Identificar novos riscos e registrar ocorrências | Continuamente | Todos os integrantes | Registro atualizado / issue |
| Avaliar eficácia das respostas | A cada marco do cronograma | Gerente do Projeto e responsáveis | Situação do risco e ações concluídas |

### 6.1 Gatilhos para reavaliação

Um risco deve ser reavaliado quando ocorrer uma destas situações:

- Uma atividade dependente atrasar ou ficar bloqueada.
- Uma mudança de requisito afetar o escopo ou os critérios de aceite.
- Uma integração apresentar falhas repetidas.
- Testes identificarem perda, duplicidade ou inconsistência de dados.
- Uma falha de segurança ou privacidade for identificada.
- A equipe perder disponibilidade ou um responsável deixar de atuar na atividade.
- Um marco do cronograma ficar ameaçado.

### 6.2 Estados de acompanhamento

Para manter o registro atualizado, cada risco poderá receber um dos seguintes estados:

- **Aberto:** identificado e ainda sujeito à ocorrência.
- **Em tratamento:** ações preventivas ou corretivas em andamento.
- **Ocorrido:** o evento aconteceu e o plano de contingência deve ser aplicado.
- **Encerrado:** não exige mais acompanhamento ativo, com justificativa registrada.

## 7. Análise quantitativa — limites desta versão

A atividade da aula apresenta a análise quantitativa como o processo de analisar numericamente os efeitos dos riscos nos objetivos gerais do projeto. Nesta versão, foi aplicada uma avaliação numérica simplificada por probabilidade, impacto médio e severidade.

Não foram calculados valores financeiros esperados ou simulações de prazo porque ainda não há orçamento formal aprovado, histórico de ocorrências nem estimativas confiáveis de custo para cada evento. Para uma análise quantitativa mais aprofundada, a equipe precisaria levantar, por exemplo:

- custo estimado de retrabalho por tipo de falha;
- duração provável de atrasos;
- esforço necessário para corrigir defeitos;
- frequência real de falhas observadas nos testes;
- impacto de indisponibilidade ou perda de evidências.

Assim, os números deste documento devem ser entendidos como **estimativas de priorização**, e não como previsões financeiras ou estatísticas comprovadas.

## 8. Observação sobre o enunciado da atividade

Na apresentação da Aula 07, a atividade é intitulada **“Análise de Riscos do Projeto FieldOps”**. Entretanto, o texto complementar solicita informações como destinatários, responsáveis, canais, frequência, formato e momento de realização, que são campos característicos de um Plano de Comunicação (atividade da Aula 06).

Este documento prioriza a análise de riscos, pois corresponde ao título e ao conteúdo principal da Aula 07. Recomenda-se confirmar com o professor se o trecho sobre comunicação foi mantido por engano ou se existe uma entrega complementar.

## 9. Premissas e pontos pendentes de validação

- As probabilidades e os impactos foram estimados para planejamento acadêmico e precisam ser revisados pela equipe.
- Os responsáveis estão indicados por papel ou equipe, sem atribuir nomes pessoais não informados.
- A classificação de prioridade usa uma escala adaptada e explícita neste documento.
- As ações relacionadas a sincronização offline, armazenamento de evidências, permissões e dados pessoais devem ser comparadas com os requisitos efetivamente aprovados do FieldOps.
- O risco de leitura de QR Code pressupõe que essa funcionalidade permaneça no escopo, conforme o backlog conhecido.
- O plano deve ser atualizado quando houver novas decisões, testes, mudanças de escopo ou alterações no cronograma.

## 10. Checklist de validação

- [x] Identificar riscos relacionados ao escopo conhecido do FieldOps.
- [x] Descrever causa, evento e consequência de cada risco.
- [x] Definir critérios de probabilidade e impacto.
- [x] Calcular impacto médio e severidade.
- [x] Classificar os riscos por prioridade.
- [x] Definir abordagem e resposta para cada risco.
- [x] Indicar responsáveis por papel/equipe.
- [x] Definir frequência e evidências de monitoramento.
