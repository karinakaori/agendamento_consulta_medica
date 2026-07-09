# Analise Qualitativa dos Riscos

## Criterios utilizados

A analise considera probabilidade, impacto e prioridade de tratamento.

| Nivel | Probabilidade | Impacto |
| --- | --- | --- |
| Baixo | Pouco provavel no contexto atual | Afeta pouco o prazo, custo, escopo ou qualidade |
| Medio | Pode ocorrer se nao houver controle | Afeta entregas importantes, mas com recuperacao possivel |
| Alto | Ja existem sinais claros de ocorrencia | Pode comprometer prazo, qualidade, seguranca ou entrega |

## Matriz de analise

| ID | Risco | Probabilidade | Impacto | Prioridade | Impactos principais | Fatores condicionantes |
| --- | --- | --- | --- | --- | --- | --- |
| R01 | Falha ou atraso na integracao com o prontuario externo | Alta | Alto | Critica | Bloqueio de funcionalidade essencial, atraso na homologacao, retrabalho tecnico. | Documentacao incompleta da API, mudancas recentes no sistema externo, dependencia de terceiros. |
| R02 | Mudancas de requisitos no fluxo de agendamento | Alta | Medio/Alto | Alta | Aumento de escopo, replanejamento, retrabalho em telas, regras e testes. | Solicitacoes sem controle formal, regras de negocio ainda em amadurecimento, baixa priorizacao. |
| R03 | Sobrecarga da equipe | Alta | Alto | Critica | Queda de produtividade, aumento de defeitos, atraso nas entregas e desgaste da equipe. | Equipe pequena, apenas 1 tester, acumulacao de mudancas e integracao critica instavel. |
| R04 | Baixa cobertura de testes em fluxos criticos | Media | Alto | Alta | Defeitos em agendamento, notificacoes ou integracao podem chegar a homologacao ou producao. | Pouco tempo para testes regressivos, fluxo de negocio com muitas validacoes, concentracao da validacao em uma pessoa. |
| R05 | Retrabalho por documentacao insuficiente | Media | Medio | Media | Perda de historico de decisoes, divergencia entre stakeholders e equipe tecnica. | Falta de padrao para atas, decisoes, mudancas e criterios de aceite. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Media | Alto | Alta | Falhas na confirmacao de consultas, experiencia ruim do usuario e dependencia operacional. | SLA desconhecido, ambiente externo instavel, ausencia de estrategia de contingencia. |
| R07 | Problemas de seguranca e privacidade de dados | Media | Alto | Alta | Exposicao de dados sensiveis, risco legal, perda de confianca e necessidade de correcao urgente. | Tratamento de dados de saude, logs inadequados, trafego sem controles, uso indevido de ferramentas externas. |
| R08 | Comunicacao insuficiente com stakeholders | Media | Medio | Media | Decisoes tardias, expectativas desalinhadas e pressao por prazo sem visibilidade tecnica. | Relatorios pouco objetivos, falta de narrativa de risco, ausencia de opcoes de decisao. |

## Sintese da analise

O maior ponto de atencao do projeto e a dependencia da integracao com o sistema externo de prontuario. Como essa integracao e critica, qualquer instabilidade afeta diretamente a entrega. Ao mesmo tempo, as mudancas no fluxo de agendamento aumentam o escopo e pressionam uma equipe pequena, o que eleva a chance de atraso e queda de qualidade.

Os riscos de seguranca tambem precisam ser tratados com prioridade, pois o aplicativo lida com informacoes de saude. Mesmo que nao bloqueiem imediatamente o cronograma, podem gerar impactos graves se forem descobertos tarde.
