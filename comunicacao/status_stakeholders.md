# Comunicação para Stakeholders

## Status do projeto

O projeto do aplicativo de agendamento de consultas médicas está em fase intermediária de desenvolvimento. Funcionalidades importantes já foram iniciadas e parcialmente implementadas, incluindo cadastro de usuários, gestão de agenda, agendamento, notificações e integração com o sistema externo de prontuário.

Nas últimas semanas, foram identificados pontos de atenção que podem afetar prazo, escopo e qualidade da entrega. O principal risco está relacionado à integração com o prontuário externo, que apresentou instabilidade e depende de documentação de API mais clara. Além disso, houve novas solicitações de mudança no fluxo de agendamento, incluindo validações e regras de negócio adicionais.

## Principais riscos

O risco mais crítico é a integração com o sistema externo, pois ela é essencial para a entrega do produto. Caso a instabilidade continue, podem ocorrer atrasos na homologação e necessidade de retrabalho técnico.

Também existe risco de aumento de escopo. As novas regras de agendamento são relevantes, mas precisam ser avaliadas quanto ao impacto em prazo, desenvolvimento e testes.

Outro ponto importante é a capacidade da equipe. Atualmente, o projeto conta com 4 desenvolvedores e 1 tester. Com o aumento das demandas e a necessidade de validar fluxos críticos, há risco de sobrecarga e redução da qualidade se o trabalho não for replanejado.

## Ações em andamento

Para reduzir esses riscos, serão adotadas as seguintes ações:

- consolidar dúvidas técnicas e solicitar documentação atualizada da API externa;
- criar cenários de teste com mock da integração para não bloquear todo o desenvolvimento;
- registrar formalmente as mudanças de requisitos e avaliar impacto antes da aprovação;
- priorizar os fluxos críticos de agendamento e integração;
- reforçar a documentação das decisões tomadas durante o projeto;
- revisar cuidados de segurança e privacidade no tratamento de dados sensíveis.

## Decisões necessárias

Para manter previsibilidade, os stakeholders precisam apoiar três decisões:

1. Priorizar quais mudanças no fluxo de agendamento devem entrar na próxima entrega.
2. Definir se funcionalidades não críticas podem ser postergadas para reduzir risco de atraso.
3. Apoiar a comunicação com o fornecedor ou responsável pelo sistema externo de prontuário.

## Próximos passos

Na próxima etapa, a equipe deve focar na estabilização da integração, na validação dos fluxos mais importantes e no replanejamento do escopo conforme a capacidade real disponível. Um novo status deve ser compartilhado após a validação técnica da API externa e a revisão das mudanças solicitadas.

Com essas medidas, o projeto ganha maior controle sobre riscos, melhora a transparência para tomada de decisão e reduz a chance de retrabalho nas próximas entregas.
