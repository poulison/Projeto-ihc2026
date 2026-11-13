# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 23/10/2026

**Revisão:** 08/11/2026

**Equipe:** 14 — Estoque com ML

**Integrantes:** Paulo Andre de Oliveira Hirata — 22.125.072-3; Victor Merker Binda — 22.125.075-6.

**Status:** 🟩 concluída.

**Responsabilidade:** 1 solução por equipe.

## Objetivo da atividade

Definir requisitos e critérios verificáveis para a interação de responsáveis por pequenos comércios com informações de estoque e previsão. O ciclo adotado é iterativo e centrado nos usuários: compreender contexto, especificar necessidades, projetar alternativas, prototipar, avaliar e revisar. A [Entrega 7](07_coleta_dados.md) investigará as hipóteses; as metas abaixo orientarão as Entregas 12–14.

O foco mantém as tarefas da [Entrega 5](05_analise_tarefas.md): **T01**, analisar um produto e registrar planejamento de reposição, adiamento ou pendência; **T02**, investigar uma divergência e registrar correção justificada ou pendência. P01 e P02 são personas de expectativa. Idade não comprova habilidade ou dificuldade; recrutamento deve considerar atividade e experiência reais.

### Continuidade com as entregas anteriores

As metas retomam o problema e as lacunas da E1; RC02/RC07/RC08/RC09/RC10 da [E2](02_analise_concorrencia.md), sobre unidade, linguagem, limites, revisão e feedback; a aprendizagem e o contexto de P01/P02 na E3; E4-C01/E4-C02 e R04-01/R04-02; T01/T02 da E5; e PF01/PF02 da E6. Mantém-se Paulo — Mariana/C01/T01 e Victor — Rafael/C02/T02, com consolidação desta entrega pela equipe.

## Delimitação do sistema interativo

| Camada | Escopo | O que será avaliado |
|---|---|---|
| Contribuição técnica do TCC | Previsão de demanda e comparação de modelos a partir de histórico | Desempenho preditivo exige avaliação técnica própria; não será inferido de teste de interface |
| Interação da disciplina | Identificar produto/unidade, consultar saldo e estimativa, registrar decisão; investigar divergência, justificar correção ou pendência | Compreensão, conclusão, tempo, erros, aprendizagem, satisfação e acessibilidade |
| Dados e integrações simulados | E6 contém capturas estáticas com dados demonstrativos; salvamento de decisão, correção, pendência e falhas de gravação ainda são estados a preparar | Avaliar interpretação e fluxo; não comprova integração, persistência real, latência ou qualidade do modelo |

A [Entrega 6](06_prototipacao_papel.md) cobre parcialmente T01 em PF01 e apenas o início de T02 em PF02. Antes de medir conclusão completa, será necessário representar registro de decisão, correção justificada e pendência. Uma tarefa interrompida por ausência de tela deve ser classificada como limitação do protótipo, não incapacidade do participante.

**Fidelidade das representações disponíveis.** Conforme **Principios Diretrizes Design.pdf**, pp. 22–32, wireframe é representação de baixa fidelidade, voltada a documentação e comunicação rápida; mockup é representação estática de média a alta fidelidade, útil para revisar a parte visual e coletar impressões; protótipo é interativo, de média a alta fidelidade, e é a representação indicada para teste de usabilidade com simulação das interfaces finais. A E6 está no primeiro grupo: capturas estáticas sem interação própria, navegadas pelo facilitador. Por isso as metas de tempo, erro e retomada só produzem valores comparáveis sobre a versão navegável prevista para a E11; aplicadas às capturas atuais, mediriam a condução do facilitador tanto quanto a interface.

O protótipo não envia pedidos a fornecedores. Salvar planejamento não significa comprar. Uma previsão não determina automaticamente quantidade ou momento da reposição: essa capacidade depende de confirmação técnica e de regras comerciais. Em T02, corrigir um item não significa concluir todos os registros.

## 1. Características da plataforma

As características distinguem o que foi documentado na E6 e os requisitos propostos para sua evolução. Não atribuem às capturas funções que elas não demonstram.

| Característica | Descrição proposta / condição | Consequência para IHC |
|---|---|---|
| Software | Aplicação web em português representada pelas telas estáticas da E6; navegação simulada pelo facilitador | Fluxos e termos consistentes; não exigir conhecimento de ML |
| Hardware/dispositivos | Computador como referência das capturas da E6; celular é possibilidade da E3 a investigar na E7, sem responsividade já comprovada | Adaptar conteúdo sem ocultar unidades ou ações; testar separadamente cada dispositivo coberto |
| Capacidades | E6: catálogo, vendas, análises, previsão e histórico de execuções. Evolução proposta: registro de decisão, correção justificada e pendência | Apoiar T01/T02 com informação suficiente e encerramento explícito |
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

Correspondência, simplicidade, controle, consistência, eficiência e visibilidade retomam **Principios Diretrizes Design.pdf**, pp. 3–13. Exigir evidência antes de corrigir decorre de E4-C02/T02; as recomendações da E2 complementam o vocabulário e a apresentação. São orientações de design, não resultados de testes.

**Referências complementares verificadas em 23/10/2026:**

- [WCAG 2.2, W3C](https://www.w3.org/TR/WCAG22/): adotar como critérios de projeto contraste de texto comum de pelo menos 4,5:1 (1.4.3, observadas as exceções), informação não dependente apenas de cor (1.4.1), uso por teclado (2.1.1), foco visível (2.4.7) e alvos de pelo menos 24 × 24 pixels CSS ou espaçamento/exceções previstos em 2.5.8. Inspecionar o protótipo visualmente e testar teclado/tecnologia assistiva na implementação. Protótipo navegável não comprova conformidade integral.
- [LGPD, texto oficial](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm): os princípios de necessidade e segurança do art. 6º orientam minimização e proteção dos dados pessoais. A E7 especifica armazenamento, acesso e descarte; este trabalho não declara conformidade jurídica integral.

### 2.1 Guia de estilo e padrões a definir antes da avaliação

O mesmo material distingue princípios, padrões de design e guia de estilo (pp. 17–21). Padrões descrevem boas práticas para um problema recorrente, não são soluções prontas e não asseguram por si a qualidade do produto; por isso entram aqui como proposta a verificar na avaliação, não como decisão validada.

| Escopo do guia de estilo (p. 21) | Decisão mínima para este projeto | Como será verificada |
|---|---|---|
| Layout | Identificação do produto, saldo e ações de registro em posição fixa nas telas de T01 e T02 | Inspeção comparativa das telas |
| Tipografia | Números de saldo, unidade e período legíveis; nenhum texto essencial apenas dentro de imagem | Inspeção e critério 1.4.3 da seção 2 |
| Simbolismo | Ícones sempre acompanhados de rótulo textual | Inspeção |
| Cores | Divergência, pendência e falha nunca indicadas somente por cor | Critério 1.4.1 |
| Visualização de informação | Gráficos e estimativas sempre com período, unidade e aviso de variação | Perguntas de compreensão de MU02 |
| Elementos de interface | Mesmo widget e mesmo rótulo para a mesma ação: “Salvar decisão”, “Registrar pendência”, “Corrigir com justificativa” | Inspeção e MU04 |

Padrões considerados, descritos no formato de pp. 18–19 (nome, problema, solução, quando usar): **painéis colapsáveis** para as evidências consultadas em T02, desde que o conteúdo recolhido continue localizável, já que a desvantagem apontada no material é justamente ocultar elementos; **confirmação explícita** apenas antes de ações difíceis de reverter, conforme a seção 2, evitando confirmações rotineiras que o usuário passe a aceitar automaticamente. O material desaconselha acordeão dentro de assistente; se o registro de decisão for dividido em etapas, as evidências não devem ficar em painéis recolhidos dentro dessas etapas.

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

### 3.2 Metas quantitativas

#### Contexto e condições de medição

**População:** adultos que desempenham a atividade correspondente. Para a rodada final prevista no repositório, planejar **dois participantes**, conforme os dois integrantes: um com experiência de reposição e outro de conferência; ambos podem fazer as duas tarefas apenas se sua experiência justificar. Informar o denominador por tarefa, sem reunir perfis artificialmente. Com uma pessoa elegível por tarefa, relatar 1/1 ou 0/1 e tempos individuais; não generalizar porcentagens para a população. A amostra de descoberta da E7 tem finalidade distinta. Os dois participantes finais não podem ser integrantes da equipe, conforme a E14. Registrar exposição prévia ao protótipo ou participação na E7 como possível influência na aprendizagem.

**Ambiente:** mesma versão do protótipo, conjunto fictício de dados e dispositivo definido para a sessão. Dar dois minutos de familiarização geral, sem ensinar os caminhos avaliados. Ler instruções de objetivo, sem nomes de botões. Ajuda do moderador conta como ajuda; consulta à ajuda da própria interface é permitida e registrada. Se houver bloqueio ou pedido de ajuda, registrar o ponto, auxiliar para preservar o conforto e classificar a tentativa como assistida.

**Onde coletar os dados (Planejamento Avaliacao IHC.pdf, pp. 13–15).** A medição ocorrerá em ambiente controlado, e não no comércio em funcionamento, porque o conjunto de casos precisa ser o mesmo para todos os participantes e o registro de tempo e de erros exige controlar interferências. A contrapartida é conhecida: situações típicas do balcão — atendimento simultâneo, ruído, pressa do cliente — não aparecerão, e por isso a interrupção é simulada em MU07, cujo resultado não representa a frequência real de interrupções. Não há sala de observação com vidro espelhado; o facilitador ficará na mesma sala, o que deve ser registrado como possível influência sobre o comportamento observado. Avaliação em contexto real de uso, se vier a ser viável, fica como complemento posterior e não como substituição.

| Caso | Instrução de objetivo ao participante | Critério de conclusão |
|---|---|---|
| T01-A, dados suficientes | Analise a garrafa azul de 500 ml e registre o que decidiu sobre sua reposição | Identificar produto, reconhecer 6 físicas menos 2 comprometidas = 4 disponíveis; considerar contexto e salvar decisão coerente com sua justificativa. Não impor compra de 6 como resposta correta |
| T01-B, dado insuficiente | Analise o item com informação incompleta e registre como prosseguir | Reconhecer lacuna e registrar pendência/próxima verificação; não interpretar ausência de previsão como zero |
| T02-A, duplicidade confirmável | Investigue a diferença dos conjuntos de potes e registre o desfecho | Diante de saldo 8, contagem 10 e duas transcrições confirmadas da mesma saída de 2 conjuntos, corrigir apenas a duplicação e justificar saldo 10; comunicar alcance parcial |
| T02-B, origem incerta | Investigue a diferença quando a origem dos registros não puder ser confirmada | Preservar saldo, registrar pendência e próxima verificação; não inventar entrada para igualar números |
| Retomada | Pausar antes da confirmação por 30 segundos em atividade neutra e depois continuar | Recuperar produto/episódio, próxima ação e situação de salvamento; não duplicar registro |

As quantidades vêm dos casos fictícios da E5 e devem ser preparadas na versão de teste: o catálogo das capturas da E6 não reproduz esses mesmos itens e P07/P08 mostram produtos ilustrativos diferentes, não uma execução contínua. Estimativas adicionais, se necessárias, serão rotuladas como simuladas. Aplicar primeiro o caso A e sua repetição equivalente para MU06; depois B e uma execução separada com pausa para MU07. Não dar correção didática entre as duas primeiras execuções. Registrar toda ajuda; uma segunda tentativa após explicação representa desempenho com treinamento, não aprendizagem autônoma. As perguntas pós-tarefa ficam fora da cronometragem. Na retomada, declarar previamente que haverá pausa; ela não representa a frequência real de interrupções.

#### Métricas e critérios de aceitação

**Todos os limites são propostas iniciais da equipe, sem linha de base medida.** Calibrá-los no piloto e congelar a versão antes do teste principal; não mudar limites depois de ver resultados para transformar falhas em sucesso.

| ID | Dimensão | Métrica e tarefa | Meta inicial | Como medir / justificativa |
|---|---|---|---|---|
| MU01 | Eficácia | Conclusão correta sem ajuda do moderador, separada por T01-A e T02-A | Pelo menos 80%; com 1 ou 2 elegíveis por tarefa, todos devem concluir | 100 × conclusões independentes / primeiras tentativas elegíveis. Repetições não entram nesse denominador. Etapas corretas e registro conferido, não apenas clique final |
| MU02 | Compreensão | Participantes que explicam todos os pontos essenciais de T01 | 100% dos elegíveis | Após T01-A e T01-B, perguntar o significado dos dados e do registro, sem revelar respostas. Verificar: 4 disponíveis em A; estimativa não é garantia; ausência não é zero em B; salvar não envia compra. Cada erro crítico orienta revisão |
| MU03 | Eficiência | Tempo ativo de conclusão independente | T01-A até 180 s; T02-A até 300 s por participante | Do início após leitura até registro correto e conferido; reservar mais tempo para investigação de T02 |
| MU04 | Segurança | Erros críticos por tentativa, inclusive casos B | Zero | Contar produto/unidade errados, ajuste sem evidência, duplicação e conclusão falsa de conferência; mesmo um caso exige revisão |
| MU05 | Satisfação | Nota de satisfação pós-tarefa | Pelo menos 4/5 por participante e tarefa | Perguntar “Quão satisfeito(a) ficou com a experiência de realizar esta tarefa?”: 1 muito insatisfeito(a), 2 insatisfeito(a), 3 nem satisfeito(a) nem insatisfeito(a), 4 satisfeito(a), 5 muito satisfeito(a). Pedir motivo; escala própria, não SUS |
| MU06 | Aprendizagem | Segunda execução equivalente sem ajuda após familiarização com a primeira | Todos os elegíveis concluem sem ajuda e sem erro crítico | Comparar sucesso, ajuda e erros entre primeira e segunda execução, mudando produto/valores e mantendo complexidade. Se ambas tiverem sucesso independente, registrar manutenção da autonomia, sem alegar ganho medido. Mede aprendizagem imediata, não memorização de longo prazo |
| MU07 | Retomada | Tempo para identificar contexto e próxima ação depois da pausa | Até 30 s, sem duplicação, por participante | Cronometrar após retorno; pedir identificação do estado e observar ação. A pausa em si fica fora do tempo ativo |

Em MU03, registrar também tempo total, espera do sistema, pausa, ajuda e eventual falha. Não converter desistência em conclusão rápida nem calcular eficiência apenas omitindo falhas. Se uma tentativa for assistida ou não concluída por dificuldade de interação, marcar tempo até interrupção e meta não atingida. Se houver ausência de tela ou falha do ambiente que impeça medir, registrar não avaliada. Em protótipo sem backend, essa medida caracteriza apenas o fluxo simulado.

Para MU01, informar separadamente elegíveis, primeiras tentativas iniciadas, tentativas avaliáveis e não avaliadas, com seus motivos. Calcular a taxa apenas sobre as primeiras tentativas avaliáveis; manter falhas e tentativas assistidas no denominador. Se faltar algum caso previsto por limitação do protótipo, o valor parcial não permite declarar a meta global atingida. Com denominador zero, registrar não avaliada, nunca 0% ou 100%. Em MU05, recusa de nota é dado ausente e deve ser relatada, sem imputar satisfação.

#### Tipos de dados coletados e produzidos

Classificação conforme **Planejamento Avaliacao IHC.pdf**, pp. 16–19. Ela define o tratamento possível de cada medida e evita cálculos indevidos.

| Medida | Nominal, ordinal, de intervalo ou de razão | Qualitativo ou quantitativo | Objetivo ou subjetivo |
|---|---|---|---|
| MU01 — desfecho da tentativa: independente, assistida, não concluída, não avaliada | Nominal, são categorias sem ordem | Qualitativo, resumido em frequências | Objetivo, observado na sessão |
| MU02 — pontos essenciais explicados | Nominal por ponto; contagem de acertos por participante | Qualitativo na fala, quantitativo na contagem | Objetivo quanto à verificação, a partir da explicação do participante |
| MU03 — tempo ativo até a conclusão | De razão, tem zero verdadeiro | Quantitativo | Objetivo, cronometrado |
| MU04 — erros críticos por tentativa | De razão, contagem | Quantitativo | Objetivo, observado |
| MU05 — nota de satisfação de 1 a 5 | Ordinal; a distância entre 4 e 5 não equivale à distância entre 1 e 2 | Quantitativo apenas como ordem | Subjetivo, precisa ser expresso pelo participante |
| MU06 — comparação entre primeira e segunda execução | Nominal no desfecho, ordinal na comparação | Qualitativo com apoio de contagens | Objetivo |
| MU07 — tempo para identificar contexto e próxima ação | De razão | Quantitativo | Objetivo |
| Motivo da nota, comentários e dificuldades relatadas | Nominal, depois de categorizado em temas | Qualitativo | Subjetivo |

Consequências para a análise: em MU05, relatar a distribuição e a mediana, não a média aritmética, porque a escala é ordinal; não somar notas de satisfação com contagens de erro em um índice único; e tratar os pesos da seção 3.3 como importância de projeto, não como escala de medida. Dados subjetivos registram opinião declarada e não comprovam desempenho; dados objetivos registram o que foi observado e não explicam o motivo. As duas categorias são coletadas juntas exatamente porque uma não substitui a outra.

**Registro mínimo por tentativa:** código; perfil; dispositivo; versão; tarefa/caso; início/fim; espera/pausa; conclusão independente/assistida/não concluída; erros e evidências; pontos de compreensão; nota; comentário. Para grupos maiores, apresentar também distribuição e mediana, sem esconder casos individuais. MU04 prevalece sobre rapidez ou satisfação.

### 3.3 Priorização das metas

Pesos representam importância de projeto, não porcentagens de sucesso nem resultados obtidos.

| Meta | Peso | Motivo |
|---|---:|---|
| MU01 — eficácia | 25% | Concluir o objetivo |
| MU02 — compreensão | 20% | Interpretar dados e limites |
| MU03 — eficiência | 10% | Respeitar rotina sem incentivar pressa |
| MU04 — segurança | 20% | Evitar alteração ou decisão indevida |
| MU05 — satisfação | 10% | Investigar satisfação com a experiência |
| MU06 — aprendizagem | 10% | Favorecer autonomia |
| MU07 — retomada | 5% | Recuperar trabalho interrompido |
| **Total** | **100%** | |

Os pesos não compensam falhas críticas. Não calcular uma nota média que esconda erro de segurança.

## 4. Como o ciclo será iterado

**Avaliação formativa e somativa (Planejamento Avaliacao IHC.pdf, pp. 11–12).** As revisões de protótipo, a inspeção heurística da E13 e as repetições de tarefa após reprojeto são formativas: acontecem antes de existir solução pronta, servem para comparar alternativas e localizar problemas de interação e aceitam representações de qualquer fidelidade. A rodada final da E14, sobre a versão congelada do protótipo, é somativa em relação a esta disciplina, porque compara cada resultado com as metas MU01–MU07. Ela não é somativa em relação ao produto: o sistema não está implementado, de modo que seus resultados não autorizam afirmar a qualidade de uso do sistema final.

| Etapa | Atividades e artefatos | Critério de revisão |
|---|---|---|
| Compreender contexto | Aplicar E7 e confrontar hipóteses com E1/E3/E4 | Se os papéis ou práticas diferirem, revisar personas, cenários e rastreabilidade |
| Especificar requisitos | Consolidar necessidades e metas desta E8 | Confirmar dependências técnicas e ajustar limites no piloto |
| Projetar alternativas | Usar HTA/GOMS/CTT da E5; desenvolver modelo conceitual, MoLIC e protótipos E6/E9–E11 | Caminhos de decisão, correção e pendência precisam de início, retorno e término claros |
| Avaliar formativamente | Revisar protótipo e aplicar inspeção heurística da E13 | Corrigir ambiguidades, problemas de feedback e erros críticos antes do teste principal |
| Avaliar com usuários | Detalhar DECIDE na E12 e executar E14 com instrumentos, consentimento e casos definidos | Comparar cada resultado com sua meta e documentar limitações |
| Reprojetar e verificar | Priorizar problemas, alterar fluxo/texto/estado e repetir tarefas afetadas | Registrar versão, mudança, motivo, nova evidência e problemas persistentes |

Exemplos de revisão: se “salvar” for interpretado como comprar, alterar rótulo e confirmação e testar MU02 novamente; se a diferença 8/10 provocar ajuste sem evidência, revisar acesso às fontes e caminho de pendência e repetir T02-B; se a pausa causar duplicação, revisar feedback de gravação e repetir MU07. São gatilhos previstos, não achados observados.

A equipe consolida a avaliação, preservando a autoria das tarefas registrada na E5. A matriz deverá ligar necessidade → tarefa → decisão de interface → meta → evidência → mudança. Não tratar desempenho preditivo, redução de rupturas ou economia financeira como resultados deste teste de IHC.

### Especificação para preparar e registrar a avaliação

| Item | Regra operacional |
|---|---|
| Base de T01-A | Identidade completa da garrafa; 6 físicas, 2 comprometidas, 4 disponíveis; prazo do fornecedor e restrição de recursos da E4. Anexar histórico e estimativa fictícios com período e unidade antes do piloto; a quantidade escolhida pelo usuário não tem um único gabarito |
| Base de T01-B | Mesma tarefa, mas sem confirmação do histórico de procura e sem estimativa disponível; permitir registrar pendência e próxima verificação |
| Base de T02-A | Conjunto de três potes como uma unidade comercial; saldo 8, contagem 10; pedido e anotação que confirmam a mesma saída de 2 conjuntos, com confirmação da origem por Mariana representada no material fictício |
| Base de T02-B | Mesma diferença, sem confirmação da origem; igualdade numérica sozinha não autoriza correção |
| Sucesso | Critérios da tabela de casos cumpridos e resultado final conferido; pendência é sucesso no caso de informação insuficiente, mas não conclusão da compra ou da conferência global |
| Erro crítico | Registro final em produto/unidade errados, ajuste sem fonte confirmada, duplicação ou interpretação de conferência parcial como total. Desvio corrigido antes de salvar é registrado separadamente como erro recuperado |
| Tempo | MU03 usa a primeira tentativa de A. Tempo ativo = tempo total menos espera comprovada do sistema/facilitador e pausas; manter ambos no registro. Em imagens estáticas, não comparar esse tempo diretamente com tempo de uma aplicação implementada |
| Retomada | Pausa controlada de 30 s antes de confirmar, em execução separada; cronometrar a identificação do produto, estado e próxima ação após o retorno. Não contam os 30 s de pausa |
| Interrupção da sessão | Encerrar por pedido do participante, desconforto ou bloqueio. Para padronizar, oferecer encerramento/ajuda após 6 min em T01-A e 10 min em T02-A; esses limites de sessão não são as metas de eficiência |
| Estados dos resultados | Atingida / não atingida / não avaliada. Fluxo ausente ou falha do ambiente: não avaliada e limitação explicitada. Não descartar esses casos silenciosamente nem declarar sucesso global |

**Perguntas de compreensão de T01:** “Quantas unidades estão livres para novas vendas e por quê?”, “O que a estimativa informa e o que não garante?”, “O que significa não haver previsão exibida?” e “O que aconteceu depois que você salvou a decisão?”. Aceitar explicações equivalentes em linguagem cotidiana. Não antecipar os quatro pontos corretos durante a execução.

**Ficha por tentativa:** código do participante; perfil e experiência; exposição prévia; data; versão do protótipo; dispositivo; caso; início/fim; espera; pausa; tempo ativo; conclusão independente/assistida/não concluída/não avaliada; erros críticos/recuperados; resposta de compreensão; nota de satisfação; observação; meta; decisão de revisão. Guardar os registros individuais de forma restrita, conforme E7; publicar apenas síntese sem identificação.

### O que está concluído e o que será feito depois

A especificação exigida nesta entrega está concluída: plataforma, limites, princípios, metas qualitativas e quantitativas, pesos e ciclo de revisão. Metas são requisitos propostos; não é necessário inventar uma avaliação para concluir sua definição. O preenchimento dos resultados pertence ao planejamento e execução das Entregas 12–14. Antes disso, a equipe deverá preparar os dados fictícios, completar no protótipo os caminhos ausentes da E6, fazer piloto, calibrar os limites e registrar a versão definitiva. Regras comerciais e recomendação calculada seguem dependentes da confirmação do escopo técnico. Esta revisão não modifica as outras entregas.

## Checklist

- [x] Plataforma, capacidades, restrições e consequências de IHC explicitadas.
- [x] Contribuição técnica separada da interação e dos dados simulados.
- [x] Princípios contextualizados e referências complementares identificadas.
- [x] Metas qualitativas, métricas, população, tarefas e limites definidos.
- [x] Pesos somam 100% e não são métricas de desempenho.
- [x] Tipos de dados classificados, com as consequências para a análise.
- [x] Fidelidade das representações, guia de estilo mínimo e padrões propostos registrados.
- [x] Local da medição e papel formativo ou somativo de cada etapa explicitados.
- [x] Ciclo de revisão e ligação com E12–E14 definidos.
- [ ] Pilotar e calibrar metas antes do teste principal.
- [ ] Medir resultados e revisar o protótipo com evidências reais.

## Referências

- **Principios Diretrizes Design.pdf**, pp. 2–13 para os princípios que orientam as decisões, pp. 17–21 para padrões de design e escopo do guia de estilo e pp. 22–32 para fidelidade de wireframe, protótipo e mockup; nenhum deles substitui análise e avaliação.
- **Planejamento Avaliacao IHC.pdf**, pp. 4–5 para as perspectivas de avaliação, pp. 11–12 para avaliação formativa e somativa, pp. 13–15 para contexto de uso e laboratório, pp. 16–19 para os tipos de dados, pp. 25–26 para preparação e piloto e pp. 33–38 para interpretação, relato e o framework DECIDE detalhado na E12.
- **CC8122-HTA (1).pdf** e **CC8122-GOMS-CTT (1).pdf**: apoio à modelagem já documentada na E5; tarefas e critérios desta entrega preservam T01/T02 existentes.
- Materiais fornecidos, identificados nos slides como Barbosa e Silva (2010), complementados pelas referências oficiais citadas na seção 2. Limites numéricos e pesos desta entrega são escolhas propostas para o projeto, não valores prescritos nos slides.
