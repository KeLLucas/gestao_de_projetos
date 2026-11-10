# Gerenciamento das Aquisições — FieldOps

## 1. Identificação

| Campo | Informação |
| --- | --- |
| Projeto | FieldOps — Plataforma de Inspeção em Campo |
| Patrocinador | Instituição |
| Gerente do projeto | DevOps |
| Público usuário | Técnicos |
| Prazo | Semestre letivo |
| Orçamento | Não há orçamento formal definido |
| Versão | 1.0 |
| Data de elaboração | 05/11/2026 |

## 2. Objetivo

Identificar possíveis aquisições de produtos, serviços ou recursos externos necessários ao desenvolvimento, à validação e à entrega do FieldOps. A tabela serve como planejamento inicial e deverá ser revisada pela equipe antes de qualquer contratação.

**Observação:** os itens abaixo são necessidades potenciais. A inclusão na tabela não significa que a compra será realizada. Sempre que possível, a equipe poderá utilizar recursos institucionais ou ferramentas gratuitas. Os custos não confirmados estão indicados como “a cotar” ou “R$ 0,00 — recurso existente/gratuito a confirmar”.

## 3. Planejamento das aquisições

| ID | Item ou serviço | Urgência | Justificativa | Fornecedor potencial | Quantidade | Custo unitário estimado | Custo total estimado | Observações |
| --- | --- | --- | --- | --- | ---: | ---: | ---: | --- |
| AQ-01 | Hospedagem de ambiente de desenvolvimento/testes | Média | Disponibilizar ambiente compartilhado para validação da aplicação | Provedor de nuvem ou serviço institucional | 1 mês | A cotar | A cotar | Verificar se a instituição oferece infraestrutura |
| AQ-02 | Banco de dados para testes | Alta | Armazenar dados de clientes, equipamentos, inspeções e evidências durante os testes | Serviço gerenciado ou infraestrutura da equipe | 1 ambiente | R$ 0,00* | R$ 0,00* | PostgreSQL pode ser executado localmente ou em contêiner |
| AQ-03 | Serviço de armazenamento de imagens | Média | Armazenar fotografias e evidências das inspeções, caso não seja usado armazenamento local/institucional | Provedor de armazenamento em nuvem | 1 serviço | A cotar | A cotar | Avaliar volume, segurança e política de retenção |
| AQ-04 | Domínio para demonstração | Baixa | Facilitar o acesso ao painel ou à demonstração, se houver publicação pública | Registrador de domínios | 1 domínio | A cotar | A cotar | Não é obrigatório se houver endereço institucional ou ambiente de demonstração |
| AQ-05 | Certificado HTTPS | Média | Proteger a comunicação com ambientes publicados | Autoridade certificadora ou serviço de hospedagem | 1 certificado | R$ 0,00* | R$ 0,00* | Certificados gratuitos podem atender ao ambiente acadêmico |
| AQ-06 | Ferramenta de repositório e controle de versão | Alta | Hospedar código, controlar alterações e trabalhar com branches e pull requests | GitHub ou serviço institucional | 3 repositórios | R$ 0,00* | R$ 0,00* | Considera plano gratuito ou acesso já disponível |
| AQ-07 | Ferramenta de gestão de tarefas | Média | Organizar backlog, atividades, responsáveis e andamento | GitHub Projects ou ferramenta institucional | 1 espaço | R$ 0,00* | R$ 0,00* | Confirmar disponibilidade no plano utilizado |
| AQ-08 | Ferramenta de comunicação da equipe | Alta | Apoiar reuniões, alinhamentos e comunicação assíncrona | Ferramenta institucional ou serviço gratuito | 1 espaço | R$ 0,00* | R$ 0,00* | Utilizar ferramenta já adotada pela equipe |
| AQ-09 | Dispositivo Android para testes | Alta | Validar o aplicativo móvel em equipamento real | Equipamento da equipe ou instituição | 1 unidade | R$ 0,00* | R$ 0,00* | Considera empréstimo ou equipamento já disponível |
| AQ-10 | Leitor de QR Code ou câmera de dispositivo | Alta | Testar a identificação de equipamentos por QR Code | Equipamento da equipe ou instituição | 1 unidade | R$ 0,00* | R$ 0,00* | A câmera do celular pode ser suficiente |
| AQ-11 | Etiquetas QR Code | Média | Identificar equipamentos usados nos cenários de teste | Gráfica ou impressão institucional | 20 unidades | A cotar | A cotar | Quantidade provisória para demonstração |
| AQ-12 | Impressão de documentação | Baixa | Disponibilizar cópias físicas caso sejam exigidas na apresentação | Gráfica ou setor institucional | A definir | A cotar | A cotar | Preferir entrega digital se aceita |
| AQ-13 | Serviço de monitoramento/logs | Baixa | Acompanhar erros e comportamento dos ambientes de teste | Ferramenta gratuita ou serviço de observabilidade | 1 serviço | R$ 0,00* | R$ 0,00* | Avaliar limites do plano gratuito |
| AQ-14 | Ferramenta de testes de API | Alta | Executar e documentar testes dos endpoints da API | Ferramenta gratuita ou institucional | 1 licença | R$ 0,00* | R$ 0,00* | Exemplo: ferramenta com plano gratuito |
| AQ-15 | Serviço de backup do ambiente | Média | Permitir recuperação dos dados de teste quando necessário | Infraestrutura institucional ou provedor de nuvem | 1 serviço | A cotar | A cotar | Definir frequência e retenção |

\* **R$ 0,00 não representa uma cotação comercial:** indica apenas a hipótese de uso de recurso gratuito, licença já disponível, equipamento emprestado ou infraestrutura existente. A equipe deve confirmar a disponibilidade e eventuais limites.

## 4. Critérios para seleção de fornecedores

Antes de contratar ou utilizar um fornecedor, a equipe deverá avaliar:

- Atendimento aos requisitos técnicos do FieldOps.
- Custo e condições de pagamento.
- Segurança e proteção dos dados.
- Disponibilidade e confiabilidade do serviço.
- Suporte técnico e documentação.
- Condições de uso, limites do plano e possibilidade de cancelamento.
- Critérios de qualidade, inspeção e aceitação do serviço.
- Garantia, manutenção e suporte, quando aplicáveis.

## 5. Controle das aquisições

| Controle | Como será realizado |
| --- | --- |
| Responsável pela necessidade | Integrante ou equipe que solicitou o recurso |
| Avaliação técnica | Equipe técnica responsável pelo componente |
| Avaliação de custo | Gerente do projeto e equipe |
| Aprovação | Patrocinador/instituição, conforme regras aplicáveis |
| Acompanhamento | Verificar entrega, funcionamento e atendimento ao combinado |
| Encerramento | Confirmar recebimento/aceitação e registrar pendências |

Nenhuma contratação deve ser considerada aprovada apenas por constar neste documento. A aprovação deverá seguir as regras da instituição e a disponibilidade de recursos do projeto.

## 6. Encerramento das aquisições

Quando uma aquisição for concluída, a equipe deverá:

1. Verificar se o produto ou serviço foi entregue.
2. Conferir se atende aos critérios técnicos e de qualidade definidos.
3. Registrar problemas, correções ou pendências.
4. Confirmar o aceite pelo responsável.
5. Registrar o encerramento da aquisição e eventuais obrigações restantes.

## 7. Premissas e limitações

- O FieldOps é um projeto acadêmico desenvolvido ao longo do semestre.
- Não foi informado orçamento formal aprovado.
- Não foram fornecidas cotações comerciais reais.
- Os fornecedores citados são categorias de fornecedores ou opções potenciais, não fornecedores contratados.
- A equipe deve priorizar recursos já disponíveis e soluções gratuitas adequadas.
- Quantidades e urgências são propostas iniciais e precisam ser validadas com o backlog e o plano de execução.

## 8. Checklist de validação

- [ ] Confirmar quais recursos já são disponibilizados pela instituição.
- [ ] Validar a necessidade real de cada aquisição com as equipes de API, Mobile, Admin e QA.
- [ ] Obter cotações para os itens que realmente exigirem compra.
- [ ] Confirmar quantidade, custo e fornecedor antes de qualquer contratação.
- [ ] Verificar critérios de qualidade, segurança, suporte e aceitação.
- [ ] Obter as aprovações necessárias.
- [ ] Atualizar esta tabela conforme as aquisições forem realizadas.
