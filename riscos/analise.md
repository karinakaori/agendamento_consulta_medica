# Análise Qualitativa dos Riscos

## Criterios utilizados

A análise considera probabilidade, impacto e prioridade de tratamento.

| Nivel | Probabilidade | Impacto |
| --- | --- | --- |
| Baixo | Pouco provável no contexto atual | Afeta pouco o prazo, custo, escopo ou qualidade |
| Médio | Pode ocorrer se não houver controle | Afeta entregas importantes, mas com recuperação possível |
| Alto | Já existem sinais claros de ocorrência | Pode comprometer prazo, qualidade, segurança ou entrega |

## Matriz de análise

| ID | Risco | Probabilidade | Impacto | Prioridade | Impactos principais | Fatores condicionantes |
| --- | --- | --- | --- | --- | --- | --- |
| R01 | Falha ou atraso na integração com o prontuário externo | Alta | Alto | Crítica | Bloqueio de funcionalidade essencial, atraso na homologação, retrabalho técnico. | Documentação incompleta da API, mudanças recentes no sistema externo, dependência de terceiros. |
| R02 | Mudanças de requisitos no fluxo de agendamento | Alta | Médio/Alto | Alta | Aumento de escopo, replanejamento, retrabalho em telas, regras e testes. | Solicitações sem controle formal, regras de negócio ainda em amadurecimento, baixa priorização. |
| R03 | Sobrecarga da equipe | Alta | Alto | Crítica | Queda de produtividade, aumento de defeitos, atraso nas entregas e desgaste da equipe. | Equipe pequena, apenas 1 tester, acumulação de mudanças e integração crítica instável. |
| R04 | Baixa cobertura de testes em fluxos críticos | Média | Alto | Alta | Defeitos em agendamento, notificações ou integração podem chegar à homologação ou produção. | Pouco tempo para testes regressivos, fluxo de negócio com muitas validações, concentração da validação em uma pessoa. |
| R05 | Retrabalho por documentação insuficiente | Média | Médio | Média | Perda de histórico de decisões, divergência entre stakeholders e equipe técnica. | Falta de padrão para atas, decisões, mudanças e critérios de aceite. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Média | Alto | Alta | Falhas na confirmação de consultas, experiência ruim do usuário e dependência operacional. | SLA desconhecido, ambiente externo instável, ausência de estratégia de contingência. |
| R07 | Problemas de segurança e privacidade de dados | Média | Alto | Alta | Exposição de dados sensíveis, risco legal, perda de confiança e necessidade de correção urgente. | Tratamento de dados de saúde, logs inadequados, tráfego sem controles, uso indevido de ferramentas externas. |
| R08 | Comunicação insuficiente com stakeholders | Média | Médio | Média | Decisões tardias, expectativas desalinhadas e pressão por prazo sem visibilidade técnica. | Relatórios pouco objetivos, falta de narrativa de risco, ausência de opções de decisão. |

## Síntese da análise

O maior ponto de atenção do projeto é a dependência da integração com o sistema externo de prontuário. Como essa integração é crítica, qualquer instabilidade afeta diretamente a entrega. Ao mesmo tempo, as mudanças no fluxo de agendamento aumentam o escopo e pressionam uma equipe pequena, o que eleva a chance de atraso e queda de qualidade.

Os riscos de segurança também precisam ser tratados com prioridade, pois o aplicativo lida com informações de saúde. Mesmo que não bloqueiem imediatamente o cronograma, podem gerar impactos graves se forem descobertos tarde.
