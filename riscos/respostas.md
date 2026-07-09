# Estratégias de Resposta aos Riscos

## Respostas propostas

| ID | Risco | Estratégia | Justificativa | Ações associadas |
| --- | --- | --- | --- | --- |
| R01 | Falha ou atraso na integração com o prontuário externo | Mitigar | A integração não pode ser eliminada, pois é crítica para o produto. A melhor resposta é reduzir incerteza técnica e dependência de informação incompleta. | Solicitar documentação atualizada da API; criar contrato de integração; implementar mocks para testes; definir responsável técnico pela comunicação com o fornecedor; reservar tempo para estabilização. |
| R02 | Mudanças de requisitos no fluxo de agendamento | Mitigar | Mudanças são esperadas, mas precisam passar por controle de impacto para não comprometer escopo e prazo. | Criar registro de mudanças; avaliar impacto antes da aprovação; priorizar requisitos com stakeholders; atualizar critérios de aceite; separar mudanças urgentes de melhorias futuras. |
| R03 | Sobrecarga da equipe | Mitigar | A equipe é pequena e já apresenta sinais de dificuldade para cumprir prazos. Reduzir pressão operacional ajuda a preservar qualidade. | Replanejar sprint ou cronograma; reduzir escopo não essencial; limitar trabalho em progresso; redistribuir tarefas; considerar apoio temporário em testes ou desenvolvimento. |
| R04 | Baixa cobertura de testes em fluxos críticos | Mitigar | O impacto de falhas em agendamento e integração é alto. É necessário aumentar previsibilidade da qualidade. | Priorizar testes dos fluxos críticos; automatizar testes de regressão quando viável; definir checklist de homologação; envolver desenvolvedores em testes exploratórios; testar cenários de erro da API externa. |
| R05 | Retrabalho por documentação insuficiente | Mitigar | Documentação contínua reduz perda de conhecimento e evita reinterpretações. | Manter atas curtas de reuniões; registrar decisões em Markdown; atualizar regras de negócio após mudanças; usar LLM para transformar anotações em documentos padronizados. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Transferir/Mitigar | Parte do risco depende de fornecedor externo, mas o projeto pode reduzir impacto com controles internos. | Definir SLA ou canal de suporte; criar tratamento de falhas; implementar tentativas controladas; prever mensagens claras ao usuário; registrar incidentes de integração. |
| R07 | Problemas de segurança e privacidade de dados | Evitar/Mitigar | O risco envolve dados sensíveis. Algumas práticas inseguras devem ser evitadas, e controles técnicos devem ser adotados. | Evitar inserir dados reais em ferramentas públicas de IA; anonimizar dados em testes; revisar logs; aplicar controle de acesso; validar tráfego seguro; revisar requisitos de privacidade. |
| R08 | Comunicação insuficiente com stakeholders | Mitigar | Uma comunicação clara favorece decisões rápidas e reduz desalinhamento. | Enviar relatório objetivo de status; destacar riscos, impacto e decisões necessárias; manter frequência semanal; usar linguagem acessível para público não técnico. |

## Plano de ação priorizado

1. Resolver incertezas da integração com o prontuário externo.
2. Formalizar controle de mudanças no fluxo de agendamento.
3. Replanejar capacidade da equipe considerando escopo real.
4. Fortalecer testes de regressão e validação dos fluxos críticos.
5. Reforçar documentação, comunicação e segurança no tratamento de dados.

## Critérios de acompanhamento

- Riscos críticos revisados semanalmente.
- Mudanças aprovadas somente após avaliação de impacto.
- Integração validada com cenários de sucesso, erro, lentidão e indisponibilidade.
- Comunicados de status enviados com riscos, ações e decisões pendentes.
- Documentos atualizados sempre que houver mudanca relevante.
