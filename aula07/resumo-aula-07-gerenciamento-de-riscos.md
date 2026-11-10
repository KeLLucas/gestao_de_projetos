# Resumo — Aula 07: Gerenciamento de Riscos

## 1. Visão geral

A aula apresenta o gerenciamento de riscos como um conjunto de processos para identificar, analisar, responder e acompanhar situações incertas que podem afetar os objetivos do projeto.

O material aborda:

- Os processos de gerenciamento de riscos.
- A definição de escalas de impacto.
- As opções de resposta aos riscos.
- Um exemplo de análise de probabilidade x impacto.
- Um exemplo de planejamento de respostas.
- A atividade de análise de riscos do FieldOps.

## 2. Processos de gerenciamento de riscos

A apresentação lista seis processos:

1. **Planejar o gerenciamento dos riscos:** definir como conduzir as atividades de gerenciamento dos riscos do projeto.
2. **Identificar os riscos:** determinar os riscos que podem afetar o projeto e documentar suas características.
3. **Realizar a análise qualitativa dos riscos:** priorizar os riscos para análise ou ação posterior, avaliando e combinando sua probabilidade de ocorrência e seu impacto.
4. **Realizar a análise quantitativa dos riscos:** analisar numericamente o efeito dos riscos identificados nos objetivos gerais do projeto.
5. **Planejar as respostas aos riscos:** criar opções e ações para aumentar as oportunidades e reduzir as ameaças aos objetivos do projeto.
6. **Controlar os riscos:** implementar os planos de resposta, acompanhar os riscos identificados, monitorar riscos residuais, identificar novos riscos e avaliar a eficácia do gerenciamento durante todo o projeto.

## 3. Causa, risco e consequência

Um risco deve ser descrito de forma clara, permitindo compreender por que pode acontecer e qual será seu efeito no projeto.

| Elemento | Significado |
| --- | --- |
| **Causa** | Fator ou condição que pode originar o risco. |
| **Risco** | Evento incerto que pode ocorrer durante o projeto. |
| **Consequência** | Efeito que o risco pode provocar nos objetivos do projeto. |

**Exemplo apresentado na aula:**

- **Causa:** dependência de uma API externa.
- **Risco:** a API pode ficar indisponível durante o desenvolvimento.
- **Consequência:** atraso nos testes e na entrega do sistema.

A apresentação recomenda evitar registros genéricos, como “o projeto pode atrasar”. É necessário identificar o que pode causar o atraso e qual será o impacto.

## 4. Definição da escala de impacto

A aula apresenta uma escala de cinco níveis para avaliar o impacto de um risco nos objetivos do projeto:

| Nível | Valor apresentado |
| --- | ---: |
| Muito baixo | 0,05 |
| Baixo | 0,10 |
| Moderado | 0,20 |
| Alto | 0,40 |
| Muito alto | 0,80 |

A tabela da apresentação exemplifica como esses níveis podem ser interpretados em quatro objetivos:

| Objetivo | Muito baixo | Baixo | Moderado | Alto | Muito alto |
| --- | --- | --- | --- | --- | --- |
| **Custo** | Aumento insignificante | Aumento inferior a 10% | Aumento de 10% a 20% | Aumento de 20% a 40% | Aumento superior a 40% |
| **Tempo** | Aumento insignificante | Aumento inferior a 5% | Aumento de 5% a 10% | Aumento de 10% a 20% | Aumento superior a 20% |
| **Escopo** | Diminuição pouco notável | Áreas secundárias afetadas | Áreas principais afetadas | Redução inaceitável para o patrocinador | Produto final efetivamente inútil |
| **Qualidade** | Degradação pouco notável | Somente aplicações muito exigentes afetadas | Redução da qualidade exige aprovação do patrocinador | Redução inaceitável para o patrocinador | Produto final efetivamente inútil |

## 5. Definição das respostas para os riscos

A aula apresenta quatro opções de tratamento:

| Opção | Detalhamento |
| --- | --- |
| **Evitar o risco** | Não iniciar ou descontinuar a atividade que dará origem ao risco. |
| **Transferir o risco** | Compartilhar ou transferir uma parte do risco a terceiros. |
| **Mitigar o risco** | Reduzir o impacto ou a probabilidade de ocorrência do risco. |
| **Aceitar o risco** | Tolerar o risco sem tomar uma ação específica, por ser considerado baixo ou porque a capacidade de tratamento é limitada ou o custo é desproporcional ao benefício. |

## 6. Exemplo de probabilidade x impacto

A apresentação mostra uma tabela que registra os riscos e combina probabilidade e impacto para definir severidade e prioridade.

Os campos apresentados incluem:

- ID e nome do risco.
- Descrição.
- Tipo.
- Probabilidade.
- Impacto em custo, prazo e qualidade.
- Média do impacto.
- Severidade.
- Prioridade.

No exemplo, aparecem quatro riscos:

1. **Perda de funcionário:** probabilidade 0,3; média de impacto 4; severidade 1,2; prioridade 1.
2. **Queima de equipamento:** probabilidade 0,1; média de impacto 3; severidade 0,3; prioridade 4.
3. **Queda de energia:** probabilidade 0,2; média de impacto 2; severidade 0,4; prioridade 3.
4. **Dificuldade no treinamento:** probabilidade 0,2; média de impacto 2,67; severidade aproximada 0,53; prioridade 2.

O exemplo demonstra que a prioridade não depende apenas da probabilidade: também considera o impacto do risco. No quadro apresentado, a perda de funcionário recebe a maior prioridade, enquanto a queima de equipamento recebe a menor.

## 7. Exemplo de respostas para riscos

A última tabela demonstra como registrar o tratamento de cada risco. Ela contém:

- ID.
- Risco e descrição.
- Tipo.
- Data de inclusão.
- Abordagem.
- Resposta ou observação.
- Responsável.

Exemplos apresentados:

| Risco | Abordagem | Resposta / observação | Responsável |
| --- | --- | --- | --- |
| Perda de funcionário | Mitigar | Capacitar outro funcionário para substituição | Gerente do Projeto |
| Queima de equipamento | Mitigar | Realizar revisão do equipamento | Coordenador de Infraestrutura |
| Queda de energia | Aceitar | Suspender o trabalho | Gerente do Projeto |
| Dificuldade no treinamento | Mitigar | Tentar outra abordagem de treinamento | Coordenador de Treinamento |

O exemplo mostra que registrar o risco não é suficiente: também é necessário definir uma abordagem, uma resposta e quem ficará responsável por ela.

## 8. Atividade da Aula 07 — Análise de Riscos do FieldOps

A atividade solicita elaborar a **Análise de Riscos do Projeto FieldOps**, considerando toda a documentação e os artefatos disponíveis. O documento deve ser organizado e entregue no repositório do GitHub.

**Atenção a uma inconsistência no enunciado:** embora o título da atividade solicite uma análise de riscos, o restante do texto menciona informações de comunicação, destinatários, responsáveis, canais, frequência, formato e momento de realização — conteúdo que corresponde a um plano de comunicação. Vale confirmar com o professor se essa parte foi mantida por engano de uma atividade anterior ou se também deve ser entregue.

## 9. Para lembrar

- **Causa:** por que o risco pode acontecer.
- **Risco:** o evento incerto.
- **Consequência:** o efeito nos objetivos do projeto.
- **Análise qualitativa:** prioriza os riscos considerando probabilidade e impacto.
- **Análise quantitativa:** analisa numericamente os efeitos dos riscos.
- **Resposta:** define como lidar com o risco — evitar, transferir, mitigar ou aceitar.
- **Controle:** acompanha os riscos e verifica se as respostas estão funcionando.

---
