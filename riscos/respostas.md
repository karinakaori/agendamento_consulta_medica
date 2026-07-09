# Estrategias de Resposta aos Riscos

## Respostas propostas

| ID | Risco | Estrategia | Justificativa | Acoes associadas |
| --- | --- | --- | --- | --- |
| R01 | Falha ou atraso na integracao com o prontuario externo | Mitigar | A integracao nao pode ser eliminada, pois e critica para o produto. A melhor resposta e reduzir incerteza tecnica e dependencia de informacao incompleta. | Solicitar documentacao atualizada da API; criar contrato de integracao; implementar mocks para testes; definir responsavel tecnico pela comunicacao com o fornecedor; reservar tempo para estabilizacao. |
| R02 | Mudancas de requisitos no fluxo de agendamento | Mitigar | Mudancas sao esperadas, mas precisam passar por controle de impacto para nao comprometer escopo e prazo. | Criar registro de mudancas; avaliar impacto antes da aprovacao; priorizar requisitos com stakeholders; atualizar criterios de aceite; separar mudancas urgentes de melhorias futuras. |
| R03 | Sobrecarga da equipe | Mitigar | A equipe e pequena e ja apresenta sinais de dificuldade para cumprir prazos. Reduzir pressao operacional ajuda a preservar qualidade. | Replanejar sprint ou cronograma; reduzir escopo nao essencial; limitar trabalho em progresso; redistribuir tarefas; considerar apoio temporario em testes ou desenvolvimento. |
| R04 | Baixa cobertura de testes em fluxos criticos | Mitigar | O impacto de falhas em agendamento e integracao e alto. E necessario aumentar previsibilidade da qualidade. | Priorizar testes dos fluxos criticos; automatizar testes de regressao quando viavel; definir checklist de homologacao; envolver desenvolvedores em testes exploratorios; testar cenarios de erro da API externa. |
| R05 | Retrabalho por documentacao insuficiente | Mitigar | Documentacao continua reduz perda de conhecimento e evita reinterpretacoes. | Manter atas curtas de reunioes; registrar decisoes em Markdown; atualizar regras de negocio apos mudancas; usar LLM para transformar anotacoes em documentos padronizados. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Transferir/Mitigar | Parte do risco depende de fornecedor externo, mas o projeto pode reduzir impacto com controles internos. | Definir SLA ou canal de suporte; criar tratamento de falhas; implementar tentativas controladas; prever mensagens claras ao usuario; registrar incidentes de integracao. |
| R07 | Problemas de seguranca e privacidade de dados | Evitar/Mitigar | O risco envolve dados sensiveis. Algumas praticas inseguras devem ser evitadas, e controles tecnicos devem ser adotados. | Evitar inserir dados reais em ferramentas publicas de IA; anonimizar dados em testes; revisar logs; aplicar controle de acesso; validar trafego seguro; revisar requisitos de privacidade. |
| R08 | Comunicacao insuficiente com stakeholders | Mitigar | Uma comunicacao clara favorece decisoes rapidas e reduz desalinhamento. | Enviar relatorio objetivo de status; destacar riscos, impacto e decisoes necessarias; manter frequencia semanal; usar linguagem acessivel para publico nao tecnico. |

## Plano de acao priorizado

1. Resolver incertezas da integracao com o prontuario externo.
2. Formalizar controle de mudancas no fluxo de agendamento.
3. Replanejar capacidade da equipe considerando escopo real.
4. Fortalecer testes de regressao e validacao dos fluxos criticos.
5. Reforcar documentacao, comunicacao e seguranca no tratamento de dados.

## Criterios de acompanhamento

- Riscos criticos revisados semanalmente.
- Mudancas aprovadas somente apos avaliacao de impacto.
- Integracao validada com cenarios de sucesso, erro, lentidao e indisponibilidade.
- Comunicados de status enviados com riscos, acoes e decisoes pendentes.
- Documentos atualizados sempre que houver mudanca relevante.
