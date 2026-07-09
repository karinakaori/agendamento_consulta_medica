# Identificacao de Riscos

## Contexto

O projeto consiste em um aplicativo movel para agendamento de consultas medicas. A equipe possui 4 desenvolvedores e 1 tester. A integracao com o sistema externo de prontuario e critica para a entrega do projeto.

Nas ultimas semanas, foram observados tres sinais de alerta:

- instabilidade na integracao com o prontuario externo;
- solicitacoes de mudancas no fluxo de agendamento;
- aumento da carga de trabalho e dificuldade para cumprir prazos.

## Riscos identificados

| ID | Risco | Descricao breve | Contexto de ocorrencia |
| --- | --- | --- | --- |
| R01 | Falha ou atraso na integracao com o prontuario externo | A API externa pode permanecer instavel, mudar sem aviso ou continuar com documentacao insuficiente. | Ocorre durante desenvolvimento, testes integrados e homologacao da integracao. |
| R02 | Mudancas de requisitos no fluxo de agendamento | Novas validacoes e regras de negocio podem alterar funcionalidades ja implementadas. | Ocorre quando stakeholders solicitam ajustes sem analise formal de impacto. |
| R03 | Sobrecarga da equipe | A equipe pode nao conseguir absorver novas demandas sem comprometer prazo ou qualidade. | Ocorre pela combinacao de escopo crescente, integracao instavel e equipe reduzida. |
| R04 | Baixa cobertura de testes em fluxos criticos | Funcionalidades de agendamento e integracao podem ser entregues com defeitos nao identificados. | Ocorre quando o unico tester precisa validar muitas mudancas em pouco tempo. |
| R05 | Retrabalho por documentacao insuficiente | Decisoes, regras de negocio e detalhes tecnicos podem ficar dispersos ou desatualizados. | Ocorre em reunioes, alteracoes de API e mudancas de escopo sem registro estruturado. |
| R06 | Indisponibilidade ou baixo desempenho do sistema externo | Mesmo com a integracao implementada, o prontuario externo pode apresentar lentidao ou indisponibilidade. | Ocorre em ambiente de testes, homologacao ou producao, afetando confirmacao e consulta de dados. |
| R07 | Problemas de seguranca e privacidade de dados | Dados sensiveis de pacientes podem ser expostos ou tratados de forma inadequada. | Ocorre em cadastro, integracao, logs, notificacoes e trafego de dados entre sistemas. |
| R08 | Comunicacao insuficiente com stakeholders | Stakeholders podem nao compreender impactos de mudancas e riscos tecnicos. | Ocorre quando o status do projeto e comunicado apenas como lista de problemas, sem decisoes e proximos passos. |

## Riscos mais relevantes

Os riscos mais relevantes para resposta prioritaria sao:

- `R01`, por ser critico para a entrega do produto;
- `R02`, por afetar escopo, prazo e retrabalho;
- `R03`, por impactar diretamente capacidade de execucao;
- `R07`, por envolver dados sensiveis de pacientes e conformidade.
