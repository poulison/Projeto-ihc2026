# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 23/10/2026

**Equipe:** 14 — Estoque com ML

**Integrantes:** Paulo Andre de Oliveira Hirata — 22.125.072-3; Victor Merker Binda — 22.125.075-6.

**Status:** 🟨 em andamento.

**Responsabilidade:** solução consolidada da equipe.

## Objetivo e contexto

Definir requisitos e critérios verificáveis para a interação de responsáveis por pequenos comércios com informações de estoque e previsão. O ciclo adotado é iterativo e centrado nos usuários: compreender contexto, especificar necessidades, projetar alternativas, prototipar, avaliar e revisar. A [Entrega 7](07_coleta_dados.md) investigará as hipóteses; as metas abaixo orientarão as Entregas 12–14.

O foco mantém as tarefas da [Entrega 5](05_analise_tarefas.md): **T01**, analisar um produto e registrar planejamento de reposição, adiamento ou pendência; **T02**, investigar uma divergência e registrar correção justificada ou pendência. P01 e P02 são personas de expectativa. Idade não comprova habilidade ou dificuldade; recrutamento deve considerar atividade e experiência reais.

## Delimitação do sistema interativo

| Camada | Escopo | O que será avaliado |
|---|---|---|
| Contribuição técnica do TCC | Previsão de demanda e comparação de modelos a partir de histórico | Desempenho preditivo exige avaliação técnica própria; não será inferido de teste de interface |
| Interação da disciplina | Identificar produto/unidade, consultar saldo e estimativa, registrar decisão; investigar divergência, justificar correção ou pendência | Compreensão, conclusão, tempo, erros, aprendizagem, satisfação e acessibilidade |
| Dados e integrações simulados | Produtos, saldos, estimativas, salvamento e estados de falha em protótipo | Avaliar interpretação e fluxo; não comprova integração, persistência real, latência ou qualidade do modelo |

O protótipo não envia pedidos a fornecedores. Salvar planejamento não significa comprar. Uma previsão não determina automaticamente quantidade ou momento da reposição: essa capacidade depende de confirmação técnica e de regras comerciais. Em T02, corrigir um item não significa concluir todos os registros.

## 1. Características da plataforma

As características abaixo são decisões propostas para IHC, não descrição de software já implementado.

| Característica | Descrição proposta / condição | Consequência para IHC |
|---|---|---|
| Software | Aplicação web em português; protótipo navegável antes de integração | Fluxos e termos consistentes; não exigir conhecimento de ML |
| Hardware/dispositivos | Computador com teclado/mouse e celular com toque; disponibilidade a investigar em E7 | Adaptar conteúdo sem ocultar unidades ou ações; testar separadamente cada dispositivo coberto |
| Capacidades | Consulta de produto, saldo e origem; estimativa quando disponível; registro revisável de decisão; conferência e pendência | Apoiar T01/T02 com informação suficiente e encerramento explícito |
| Restrições | Dados incompletos, incorretos ou desatualizados; catálogo e regras ainda não confirmados | Informar ausência/atualização; permitir pendência, sem tratar ausência de previsão como zero |
| Conectividade/latência | Condições reais desconhecidas; simular falha e espera para avaliação | Diferenciar salvando, salvo e falha; preservar rascunho e permitir verificação antes de reenviar |
| Segurança/privacidade | Protótipo com dados fictícios; pesquisa com acesso restrito | Não exibir clientes reais nem divulgar respostas brutas; mostrar apenas dados necessários |
| Volume/histórico | Volume real a investigar; conjunto controlado para teste | Exibir identificação completa; justificar busca/filtros pela tarefa e avaliar localização sem presumir milhares de itens |
| Processamento | Tempo de previsão ainda desconhecido | Mostrar estado e data do resultado; não inventar percentual ou garantia de atualização |
| Papéis/permissões | Proprietário e auxiliar são hipóteses; mesma pessoa pode executar ambas as tarefas | Confirmar autorização antes de definir perfis fixos; registrar autoria/motivo de alterações quando aplicável |
| Interrupções | Atendimento pode interromper a análise; hipótese de E3/E4 | Preservar produto, etapa, rascunho e situação de salvamento; revalidar dados alterados |

## 2. Princípios gerais do projeto

| Princípio/referência | Aplicação ao contexto | Requisito decorrente e verificação |
|---|---|---|
| Correspondência com expectativas | Usuário pensa em produtos, unidades e compra | Usar termos comerciais; mostrar físico, comprometido e disponível separados; pedir interpretação em T01 |
| Simplicidade e reconhecimento | Evitar memória de números entre telas | Manter produto, unidade e informações de apoio visíveis na revisão; observar retornos desnecessários |
| Controle e liberdade | Decisão comercial permanece humana | Permitir revisar, cancelar, adiar ou deixar pendente; não enviar compra ao salvar |
| Consistência | Mesma ação deve ter mesmo nome e resultado | Padronizar “Salvar decisão”, “Registrar pendência” e mensagens; inspecionar telas e estados |
| Visibilidade e feedback | Usuário precisa saber se concluiu | Exibir salvando/salvo/falha e diferenciar item resolvido de conferência completa |
| Prevenção e recuperação de erros | Diferença de saldo não prova a causa | Exigir evidência e justificativa antes de corrigir; permitir pendência sem ajuste arbitrário |
| Contexto e eficiência | Interrupções e múltiplos papéis | Retomada sem duplicar decisão/alteração; acesso ao resumo e à etapa anterior |
| Acessibilidade | Repertório e necessidades variados | Texto legível, informação além da cor, rótulos claros, teclado e foco visível; verificar critérios abaixo |
| Privacidade e minimização | Respostas de pesquisa e possíveis registros identificáveis | Coletar somente dados necessários, restringir acesso e não usar dados reais no protótipo |

Os sete primeiros princípios são aplicados a partir de **Principios Diretrizes Design.pdf**, pp. 3–13, complementados pelas tarefas do projeto. São orientações de design, não resultados de testes.

**Referências complementares verificadas em 23/10/2026:**

- [WCAG 2.2, W3C](https://www.w3.org/TR/WCAG22/): adotar como critérios de projeto contraste de texto comum de pelo menos 4,5:1 (1.4.3, observadas as exceções), informação não dependente apenas de cor (1.4.1), uso por teclado (2.1.1), foco visível (2.4.7) e alvos de pelo menos 24 × 24 pixels CSS ou espaçamento/exceções previstos em 2.5.8. Inspecionar o protótipo visualmente e testar teclado/tecnologia assistiva na implementação. Protótipo navegável não comprova conformidade integral.
- [LGPD, texto oficial](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm): os princípios de necessidade e segurança do art. 6º orientam minimização e proteção dos dados pessoais. A E7 especifica armazenamento, acesso e descarte; este trabalho não declara conformidade jurídica integral.

## 3. Metas de usabilidade

### 3.1 Metas qualitativas

| Meta | Público/tarefa | Evidência desejada | Justificativa |
|---|---|---|---|
| Compreender disponibilidade e previsão | Responsáveis por reposição, T01 | Explicar saldo disponível, período da estimativa e possibilidade de variação com suas palavras | Evitar decisão baseada em falsa certeza |
| Manter controle da decisão | T01 | Reconhecer planejamento, adiamento e pendência; saber que não houve compra automática | Preservar responsabilidade comercial |
| Corrigir com fundamento | Responsáveis por conferência, T02 | Explicar fonte, motivo e alcance da alteração; não ajustar sem causa confirmada | Proteger integridade dos dados |
| Aprender com autonomia | Pessoas iniciantes no protótipo, ambas as tarefas | Repetir uma tarefa equivalente com menos orientação e encontrar ajuda | Testar a proposta de apoio ao primeiro uso |
| Retomar após pausa | Ambos os perfis | Identificar produto, etapa, ação seguinte e estado de salvamento | Evitar retrabalho e duplicidade |
| Sentir clareza e segurança | Ambos os perfis | Relatar pontos compreendidos e dúvidas sem receio de clicar ou corrigir | Complementar medidas de desempenho |

### 3.2 Condições e tarefas de medição

**População:** adultos que desempenham a atividade correspondente. Para a rodada final prevista no repositório, planejar **dois participantes**, conforme os dois integrantes: um com experiência de reposição e outro de conferência; ambos podem fazer as duas tarefas apenas se sua experiência justificar. Informar o denominador por tarefa, sem reunir perfis artificialmente. Com uma pessoa elegível por tarefa, relatar 1/1 ou 0/1 e tempos individuais; não generalizar porcentagens para a população. A amostra de descoberta da E7 é distinta desse teste de usabilidade.

**Ambiente:** mesma versão do protótipo, conjunto fictício de dados e dispositivo definido para a sessão. Dar dois minutos de familiarização geral, sem ensinar os caminhos avaliados. Ler instruções de objetivo, sem nomes de botões. Ajuda do moderador conta como ajuda; consulta à ajuda da própria interface é permitida e registrada. Se houver bloqueio ou pedido de ajuda, registrar o ponto, auxiliar para preservar o conforto e classificar a tentativa como assistida.

| Caso | Instrução de objetivo ao participante | Critério de conclusão |
|---|---|---|
| T01-A, dados suficientes | Analise a garrafa azul de 500 ml e registre o que decidiu sobre sua reposição | Identificar produto, reconhecer 6 físicas menos 2 comprometidas = 4 disponíveis; considerar contexto e salvar decisão coerente com sua justificativa. Não impor compra de 6 como resposta correta |
| T01-B, dado insuficiente | Analise o item com informação incompleta e registre como prosseguir | Reconhecer lacuna e registrar pendência/próxima verificação; não interpretar ausência de previsão como zero |
| T02-A, duplicidade confirmável | Investigue a diferença dos conjuntos de potes e registre o desfecho | Diante de saldo 8, contagem 10 e duas transcrições confirmadas da mesma saída de 2 conjuntos, corrigir apenas a duplicação e justificar saldo 10; comunicar alcance parcial |
| T02-B, origem incerta | Investigue a diferença quando a origem dos registros não puder ser confirmada | Preservar saldo, registrar pendência e próxima verificação; não inventar entrada para igualar números |
| Retomada | Pausar antes da confirmação por 30 segundos em atividade neutra e depois continuar | Recuperar produto/episódio, próxima ação e situação de salvamento; não duplicar registro |

As quantidades vêm dos casos fictícios da E5. Estimativas adicionais, se necessárias, serão rotuladas como simuladas. Aplicar primeiro os casos A; usar B como diagnóstico adicional e registrar efeito de aprendizagem. Na retomada, declarar previamente que haverá pausa; ela não representa a frequência real de interrupções.

### 3.3 Metas quantitativas

**Todos os limites são propostas iniciais da equipe, sem linha de base medida.** Calibrá-los no piloto e congelar a versão antes do teste principal; não mudar limites depois de ver resultados para transformar falhas em sucesso.

| ID | Dimensão | Métrica e tarefa | Meta inicial | Como medir / justificativa |
|---|---|---|---|---|
| MU01 | Eficácia | Conclusão correta sem ajuda do moderador, separada por T01-A e T02-A | Pelo menos 80% dos elegíveis por tarefa; na rodada pequena, todos os elegíveis | Conclusões independentes / tentativas elegíveis. Etapas corretas e registro conferido, não apenas clique final |
| MU02 | Compreensão | Participantes que explicam todos os pontos essenciais de T01 | 100% dos elegíveis | Depois da tarefa, verificar: 4 disponíveis; estimativa não é garantia; ausência não é zero; salvar não envia compra. Cada erro crítico orienta revisão |
| MU03 | Eficiência | Tempo ativo de conclusão independente | T01-A até 180 s; T02-A até 300 s por participante | Do início após leitura até registro correto e conferido; reservar mais tempo para investigação de T02 |
| MU04 | Segurança | Erros críticos por tentativa, inclusive casos B | Zero | Contar produto/unidade errados, ajuste sem evidência, duplicação e conclusão falsa de conferência; mesmo um caso exige revisão |
| MU05 | Satisfação | Nota pós-tarefa de facilidade | Pelo menos 4/5 por participante e tarefa | Perguntar “Quão fácil ou difícil foi realizar esta tarefa?”: 1 muito difícil, 2 difícil, 3 nem fácil nem difícil, 4 fácil, 5 muito fácil. Escala própria, não SUS |
| MU06 | Aprendizagem | Segunda execução equivalente sem ajuda após familiarização com a primeira | Todos os elegíveis concluem sem ajuda e sem erro crítico | Alterar produto/valores mantendo complexidade; registrar ajuda na primeira. Mede aprendizagem imediata, não memorização de longo prazo |
| MU07 | Retomada | Tempo para identificar contexto e próxima ação depois da pausa | Até 30 s, sem duplicação, por participante | Cronometrar após retorno; pedir identificação do estado e observar ação. A pausa em si fica fora do tempo ativo |

Em MU03, registrar também tempo total, espera do sistema, pausa, ajuda e eventual falha. Não converter desistência em conclusão rápida nem calcular eficiência apenas omitindo falhas. Se uma tentativa for assistida ou não concluída, marcar tempo até interrupção e meta não atingida. Em protótipo sem backend, essa medida caracteriza apenas o fluxo simulado.

**Registro mínimo por tentativa:** código; perfil; dispositivo; versão; tarefa/caso; início/fim; espera/pausa; conclusão independente/assistida/não concluída; erros e evidências; pontos de compreensão; nota; comentário. Para grupos maiores, apresentar também distribuição e mediana, sem esconder casos individuais. MU04 prevalece sobre rapidez ou satisfação.

### 3.4 Priorização

Pesos representam importância de projeto, não porcentagens de sucesso nem resultados obtidos.

| Meta | Peso | Motivo |
|---|---:|---|
| MU01 — eficácia | 25% | Concluir o objetivo |
| MU02 — compreensão | 20% | Interpretar dados e limites |
| MU03 — eficiência | 10% | Respeitar rotina sem incentivar pressa |
| MU04 — segurança | 20% | Evitar alteração ou decisão indevida |
| MU05 — satisfação | 10% | Investigar facilidade percebida |
| MU06 — aprendizagem | 10% | Favorecer autonomia |
| MU07 — retomada | 5% | Recuperar trabalho interrompido |
| **Total** | **100%** | |

Os pesos não compensam falhas críticas. Não calcular uma nota média que esconda erro de segurança.

## 4. Ciclo de vida e iteração

| Etapa | Atividades e artefatos | Critério de revisão |
|---|---|---|
| Compreender contexto | Aplicar E7 e confrontar hipóteses com E1/E3/E4 | Se os papéis ou práticas diferirem, revisar personas, cenários e rastreabilidade |
| Especificar requisitos | Consolidar necessidades e metas desta E8 | Confirmar dependências técnicas e ajustar limites no piloto |
| Projetar alternativas | Usar HTA/GOMS/CTT da E5; desenvolver modelo conceitual, MoLIC e protótipos E6/E9–E11 | Caminhos de decisão, correção e pendência precisam de início, retorno e término claros |
| Avaliar formativamente | Revisar protótipo e aplicar inspeção heurística da E13 | Corrigir ambiguidades, problemas de feedback e erros críticos antes do teste principal |
| Avaliar com usuários | Detalhar DECIDE na E12 e executar E14 com instrumentos, consentimento e casos definidos | Comparar cada resultado com sua meta e documentar limitações |
| Reprojetar e verificar | Priorizar problemas, alterar fluxo/texto/estado e repetir tarefas afetadas | Registrar versão, mudança, motivo, nova evidência e problemas persistentes |

Exemplos de revisão: se “salvar” for interpretado como comprar, alterar rótulo e confirmação e testar MU02 novamente; se a diferença 8/10 provocar ajuste sem evidência, revisar acesso às fontes e caminho de pendência e repetir T02-B; se a pausa causar duplicação, revisar feedback de gravação e repetir MU07. São gatilhos previstos, não achados observados.

Paulo conduz a revisão de T01 e Victor a de T02; ambos consolidam resultados e verificam a interpretação do outro. A matriz deverá ligar necessidade → tarefa → decisão de interface → meta → evidência → mudança. Não tratar desempenho preditivo, redução de rupturas ou economia financeira como resultados deste teste de IHC.

## Checklist

- [x] Plataforma, capacidades, restrições e consequências de IHC explicitadas.
- [x] Contribuição técnica separada da interação e dos dados simulados.
- [x] Princípios contextualizados e referências complementares identificadas.
- [x] Metas qualitativas, métricas, população, tarefas e limites definidos.
- [x] Pesos somam 100% e não são métricas de desempenho.
- [x] Ciclo de revisão e ligação com E12–E14 definidos.
- [ ] Pilotar e calibrar metas antes do teste principal.
- [ ] Medir resultados e revisar o protótipo com evidências reais.

## Referências

- **Principios Diretrizes Design.pdf**, pp. 2–13: princípios que orientam as decisões; não substituem análise e avaliação.
- **Planejamento Avaliacao IHC.pdf**, pp. 4–5, 11–12, 25–26 e 33–38: perspectivas, avaliação formativa/somativa, preparação e relato.
- **CC8122-HTA (1).pdf** e **CC8122-GOMS-CTT (1).pdf**: apoio à modelagem já documentada na E5; tarefas e critérios desta entrega preservam T01/T02 existentes.
- Materiais fornecidos, identificados nos slides como Barbosa e Silva (2010), complementados pelas referências oficiais citadas na seção 2. Limites numéricos e pesos desta entrega são escolhas propostas para o projeto, não valores prescritos nos slides.
