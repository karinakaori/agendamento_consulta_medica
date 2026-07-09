# Identificação de Riscos

## Contexto

O projeto consiste em um aplicativo móvel para agendamento de consultas médicas. A equipe possui 4 desenvolvedores e 1 tester. A integração com o sistema externo de prontuário é crítica para a entrega do projeto.

Nas últimas semanas, foram observados três sinais de alerta:

- instabilidade na integração com o prontuário externo;
- solicitações de mudanças no fluxo de agendamento;
- aumento da carga de trabalho e dificuldade para cumprir prazos.

## Riscos identificados

| ID | Risco | Descrição breve | Contexto de ocorrência |
| --- | --- | --- | --- |
| R01 | Falha ou atraso na integração com o prontuário externo | A API externa pode permanecer instável, mudar sem aviso ou continuar com documentação insuficiente. | Ocorre durante desenvolvimento, testes integrados e homologação da integração. |
| R02 | Mudanças de requisitos no fluxo de agendamento | Novas validações e regras de negócio podem alterar funcionalidades já implementadas. | Ocorre quando stakeholders solicitam ajustes sem análise formal de impacto. |
| R03 | Sobrecarga da equipe | A equipe pode não conseguir absorver novas demandas sem comprometer prazo ou qualidade. | Ocorre pela combinação de escopo crescente, integração instável e equipe reduzida. |
| R04 | Baixa cobertura de testes em fluxos críticos | Funcionalidades de agendamento e integração podem ser entregues com defeitos não identificados. | Ocorre quando o único tester precisa validar muitas mudanças em pouco tempo. |
| R05 | Retrabalho por documentação insuficiente | Decisões, regras de negócio e detalhes técnicos podem ficar dispersos ou desatualizados. | Ocorre em reuniões, alterações de API e mudanças de escopo sem registro estruturado. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Mesmo com a integração implementada, o prontuário externo pode apresentar lentidão ou indisponibilidade. | Ocorre em ambiente de testes, homologação ou produção, afetando confirmação e consulta de dados. |
| R07 | Problemas de segurança e privacidade de dados | Dados sensíveis de pacientes podem ser expostos ou tratados de forma inadequada. | Ocorre em cadastro, integração, logs, notificações e tráfego de dados entre sistemas. |
| R08 | Comunicação insuficiente com stakeholders | Stakeholders podem não compreender impactos de mudanças e riscos técnicos. | Ocorre quando o status do projeto é comunicado apenas como lista de problemas, sem decisões e próximos passos. |

## Riscos mais relevantes

Os riscos mais relevantes para resposta prioritária são:

- `R01`, por ser crítico para a entrega do produto;
- `R02`, por afetar escopo, prazo e retrabalho;
- `R03`, por impactar diretamente capacidade de execução;
- `R07`, por envolver dados sensíveis de pacientes e conformidade.
