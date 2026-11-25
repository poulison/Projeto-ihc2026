# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 23/10/2026

**Revisão:** 25/11/2026

**Equipe:** 14 — Estoque com ML

**Integrantes:** Paulo Andre de Oliveira Hirata — 22.125.072-3; Victor Merker Binda — 22.125.075-6.

**Status:** 🟦 revisada após feedback

**Responsabilidade:** 1 solução por equipe.

## Objetivo da atividade

Definir requisitos de uso para quem decide reposições e confere divergências em pequenos comércios. O projeto adota o Ciclo de Vida da Engenharia de Usabilidade de Mayhew. A [Entrega 7](07_coleta_dados.md) prevê a investigação das hipóteses sobre a rotina. As metas desta entrega orientam o planejamento e a avaliação nas Entregas 12–14.

O foco mantém as tarefas da [Entrega 5](05_analise_tarefas.md): **T01**, analisar um produto e registrar planejamento de reposição, adiamento ou pendência; **T02**, investigar uma divergência e registrar correção justificada ou pendência. P01 e P02 são personas de expectativa. Idade não comprova habilidade ou dificuldade; recrutamento deve considerar atividade e experiência reais.

### Continuidade com as entregas anteriores

As metas retomam o problema e as lacunas da E1; RC02/RC07/RC08/RC09/RC10 da [E2](02_analise_concorrencia.md), sobre unidade, linguagem, limites, revisão e feedback; a aprendizagem e o contexto de P01/P02 na E3; E4-C01/E4-C02 e R04-01/R04-02; T01/T02 da E5; e PF01/PF02 da E6. Mantém-se Paulo — Mariana/C01/T01 e Victor — Rafael/C02/T02, com consolidação desta entrega pela equipe.

## Delimitação do sistema interativo

| Camada | Escopo | O que será avaliado |
|---|---|---|
| Contribuição técnica do TCC | Previsão de demanda e comparação de modelos a partir de histórico | Desempenho preditivo exige avaliação técnica própria; não será inferido de teste de interface |
| Interação da disciplina | Identificar produto/unidade, consultar saldo e estimativa, registrar decisão; investigar divergência, justificar correção ou pendência | Compreensão, conclusão, tempo, erros, aprendizagem, satisfação e acessibilidade |
| Dados e integrações simulados | A E6 representa decisões, pendências e correções com capturas e cartões. A E11 documenta os caminhos navegáveis no Figma. | Observar interpretação, escolha e recuperação. Persistência, latência real e desempenho do modelo exigem avaliação própria. |

Os primeiros cartões de PF01 e PF02 cobriam parte das tarefas. Na revisão da E6, a equipe acrescentou os desfechos de decisão, correção e pendência. Antes da avaliação, verificar se a versão escolhida permite chegar ao desfecho de cada caso. Registrar qualquer tela ausente como limitação do protótipo.

Na [E6](06_prototipacao_papel.md), o facilitador troca cartões e simula as respostas da interface. Esse formato permite discutir o significado de uma decisão. Para comparar tempos, erros e retomadas, usar a versão navegável documentada na [E11](11_figma.md) e registrar a versão utilizada.

O protótipo não envia pedidos a fornecedores. Salvar planejamento não significa comprar. Uma previsão não determina automaticamente quantidade ou momento da reposição: essa capacidade depende de confirmação técnica e de regras comerciais. Em T02, corrigir um item não significa concluir todos os registros.

## 1. Características da plataforma

### Capacidades e restrições da plataforma

| Aspecto | Condição no projeto | Consequência para a interação |
|---|---|---|
| Aplicação web de estoque em português | Catálogo, vendas, análises e histórico dão contexto à reposição. Os protótipos representam decisão, correção justificada e pendência. | Identificar produto e unidade ao longo da tarefa e mostrar o desfecho do registro. |
| Navegador, tela e entrada | O computador é a referência de avaliação. O espaço visível e a forma de navegar por teclado condicionam a disposição dos controles. | Manter saldo e unidade juntos. Verificar se o foco chega a revisar, confirmar e voltar numa sequência previsível. |
| Rede e processamento | O tempo de previsão e a latência de gravação em produção ainda são desconhecidos. No protótipo, espera e falha são simuladas. | Mostrar a data da estimativa. Se a gravação ficar incerta, oferecer consulta ao registro antes de permitir nova tentativa. |

### Limitações do domínio e dos dados

Um histórico incompleto pode impedir uma estimativa. Nessa situação, T01 deve identificar o dado ausente e permitir registrar a próxima verificação. Em T02, unidade ambígua, origem incerta de uma movimentação ou falta de autorização impedem justificar uma correção. O caminho de pendência conserva o saldo e informa o que falta conferir.

### Hipóteses a verificar

A E7 investiga quais dispositivos as pessoas usam, o volume de produtos consultados, quem decide ou confere e como o atendimento interrompe o trabalho. Essas respostas orientarão o suporte a celular, a necessidade de filtros, as permissões e a retomada. Uma pessoa pode exercer ambos os papéis.

## 2. Princípios gerais do projeto

### 2.1 Princípios de negócio

| Regra do domínio | Consequência para T01 ou T02 |
|---|---|
| A decisão de compra cabe à pessoa responsável. Salvar um planejamento é um registro interno. | Em T01, Mariana pode planejar, adiar ou deixar pendente. A confirmação informa qual decisão ficou salva. |
| Estoque comprometido já tem destino. Uma estimativa ausente indica informação insuficiente. | Em T01, separar físico, comprometido e disponível. Explicar a lacuna da previsão e permitir uma decisão pendente. |
| Uma diferença numérica exige investigação. Corrigir requer origem confirmada e autorização. | Em T02, vincular a alteração ao item, à unidade, à fonte, ao responsável e ao motivo. Se faltar fundamento, manter o saldo e registrar a próxima conferência. |
| O encerramento vale para o item investigado. | Identificar o que foi resolvido e os registros que ainda exigem conferência. |
| A equipe limita a coleta e o acesso ao necessário. | Usar dados demonstrativos nas telas e códigos nas sessões. Restringir os registros individuais à equipe conforme a E7. |

### 2.2 Princípios de interface

| Princípio | Aplicação e verificação no protótipo |
|---|---|
| Linguagem do comércio e reconhecimento | Em F02, manter visíveis produto, unidade e três quantidades de estoque. Pedir que a pessoa explique quantas unidades pode vender. |
| Consistência e controle | Preservar rótulos entre escolha, revisão e confirmação. Verificar se Mariana consegue editar a quantidade antes de confirmar em F05. |
| Visibilidade e recuperação | Em F06E, oferecer consulta ao registro diante de uma gravação incerta. Em F06R, mostrar como reabrir o rascunho após falha confirmada. |
| Prevenção de erros | Em F11 e F12, aproximar fontes e revisão do saldo. Verificar se Rafael consegue seguir para pendência quando as fontes divergem. |
| Continuidade da tarefa | Na retomada por F02P ou F10P, mostrar item, etapa e próxima ação. Observar se a pessoa identifica onde estava antes de continuar. |
| Acessibilidade | Verificar contraste e rótulos textuais no aviso de previsão ausente em F02B e no erro de quantidade em F04E. Conferir tamanho do alvo de confirmação em F05. Na implementação web, testar ordem e visibilidade do foco e acionamento por teclado. |

Os estados citados constam do [catálogo da E11](11_figma.md). As verificações de acessibilidade devem identificar componente, versão, critério e evidência observada.

**Referências complementares verificadas em 23/10/2026:**

- [WCAG 2.2, W3C](https://www.w3.org/TR/WCAG22/): adotar como critérios de projeto contraste de texto comum de pelo menos 4,5:1 (1.4.3, observadas as exceções), informação não dependente apenas de cor (1.4.1), uso por teclado (2.1.1), foco visível (2.4.7) e alvos de pelo menos 24 × 24 pixels CSS ou espaçamento/exceções previstos em 2.5.8. Inspecionar o protótipo visualmente e testar teclado/tecnologia assistiva na implementação. Protótipo navegável não comprova conformidade integral.
- [LGPD, texto oficial](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm): os princípios de necessidade e segurança do art. 6º orientam minimização e proteção dos dados pessoais. A E7 especifica armazenamento, acesso e descarte; este trabalho não declara conformidade jurídica integral.

### 2.3 Guia de estilo e padrões a definir antes da avaliação

O material de aula *Princípios e Diretrizes de Design* (pp. 17–21) orienta a escolha de padrões e o registro das decisões no guia de estilo. Aplicar as decisões abaixo às telas de T01 e T02 e revê-las a partir das dificuldades observadas.

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

**Ambiente controlado.** Usar o mesmo dispositivo e os mesmos casos para comparar tentativas. Registrar a presença do facilitador e simular a pausa de MU07 em execução separada. A frequência real de interrupções deve ser investigada no contexto de trabalho.

| Caso | Instrução de objetivo ao participante | Critério de conclusão |
|---|---|---|
| T01-A, dados suficientes | Analise a garrafa azul de 500 ml e registre o que decidiu sobre sua reposição | Identificar produto, reconhecer 6 físicas menos 2 comprometidas = 4 disponíveis; considerar contexto e salvar decisão coerente com sua justificativa. Não impor compra de 6 como resposta correta |
| T01-B, dado insuficiente | Analise o item com informação incompleta e registre como prosseguir | Reconhecer lacuna e registrar pendência/próxima verificação; não interpretar ausência de previsão como zero |
| T02-A, duplicidade confirmável | Investigue a diferença dos conjuntos de potes e registre o desfecho | Diante de saldo 8, contagem 10 e duas transcrições confirmadas da mesma saída de 2 conjuntos, corrigir apenas a duplicação e justificar saldo 10; comunicar alcance parcial |
| T02-B, origem incerta | Investigue a diferença quando a origem dos registros não puder ser confirmada | Preservar saldo, registrar pendência e próxima verificação; não inventar entrada para igualar números |
| Retomada | Pausar antes da confirmação por 30 segundos em atividade neutra e depois continuar | Recuperar produto/episódio, próxima ação e situação de salvamento; não duplicar registro |

Usar os casos fictícios da E5 e conferir produto, unidade, valores e estado inicial na versão da E11 selecionada para a sessão. Para MU06, aplicar primeiro o caso A e depois um caso equivalente com outros valores, sem correção didática entre eles. Aplicar B e testar a pausa de MU07 em execução separada. Registrar ajuda e excluir as perguntas pós-tarefa da cronometragem.

#### Métricas e critérios de aceitação

**Todos os limites são propostas iniciais da equipe, sem linha de base medida.** Como a equipe decidiu não fazer piloto (25/11/2026), os limites ficam como estão e a versão é congelada antes do teste principal; não mudar limites depois de ver resultados para transformar falhas em sucesso.

| ID | Dimensão | Métrica e tarefa | Meta inicial | Como medir / justificativa |
|---|---|---|---|---|
| MU01 | Eficácia | Conclusão correta sem ajuda do moderador, separada por T01-A e T02-A | Pelo menos 80%; com 1 ou 2 elegíveis por tarefa, todos devem concluir | 100 × conclusões independentes / primeiras tentativas elegíveis e avaliáveis. Repetições não entram nesse denominador. Etapas corretas e registro conferido, não apenas clique final |
| MU02 | Compreensão | Participantes que explicam todos os pontos essenciais de T01 | 100% dos elegíveis | Após T01-A e T01-B, perguntar o significado dos dados e do registro, sem revelar respostas. Verificar: 4 disponíveis em A; estimativa não é garantia; ausência não é zero em B; salvar não envia compra. Cada erro crítico orienta revisão |
| MU03 | Eficiência | Tempo ativo de conclusão independente | T01-A até 180 s; T02-A até 300 s por participante | Do início após leitura até registro correto e conferido; reservar mais tempo para investigação de T02 |
| MU04 | Segurança | Erros críticos por tentativa, inclusive casos B | Zero | Contar produto/unidade errados, ajuste sem evidência, duplicação e conclusão falsa de conferência; mesmo um caso exige revisão |
| MU05 | Satisfação | Nota de satisfação pós-tarefa | Pelo menos 4/5 por participante e tarefa | Perguntar “Quão satisfeito(a) ficou com a experiência de realizar esta tarefa?”: 1 muito insatisfeito(a), 2 insatisfeito(a), 3 nem satisfeito(a) nem insatisfeito(a), 4 satisfeito(a), 5 muito satisfeito(a). Pedir motivo; escala própria, não SUS |
| MU06 | Aprendizagem | Segunda execução equivalente sem ajuda após familiarização com a primeira | Todos os elegíveis concluem sem ajuda e sem erro crítico | Comparar sucesso, ajuda e erros entre primeira e segunda execução, mudando produto/valores e mantendo complexidade. Se ambas tiverem sucesso independente, registrar manutenção da autonomia, sem alegar ganho medido. Mede aprendizagem imediata, não memorização de longo prazo |
| MU07 | Retomada | Tempo para identificar contexto e próxima ação depois da pausa | Até 30 s, sem duplicação, por participante | Cronometrar após retorno; pedir identificação do estado e observar ação. A pausa em si fica fora do tempo ativo |

Em MU03, registrar também tempo total, espera do sistema, pausa, ajuda e eventual falha. Não converter desistência em conclusão rápida nem calcular eficiência apenas omitindo falhas. Se uma tentativa for assistida ou não concluída por dificuldade de interação, marcar tempo até interrupção e meta não atingida. Se houver ausência de tela ou falha do ambiente que impeça medir, registrar não avaliada. Em protótipo sem backend, essa medida caracteriza apenas o fluxo simulado.

Para MU01, informar separadamente elegíveis, primeiras tentativas iniciadas, tentativas avaliáveis e não avaliadas, com seus motivos. Calcular a taxa apenas sobre as primeiras tentativas avaliáveis; manter falhas e tentativas assistidas no denominador. Se faltar algum caso previsto por limitação do protótipo, o valor parcial não permite declarar a meta global atingida. Com denominador zero, registrar não avaliada, nunca 0% ou 100%. Em MU05, recusa de nota é dado ausente e deve ser relatada, sem imputar satisfação.

#### Tipos de dados coletados e produzidos

A classificação segue o material de aula *Planejamento da Avaliação de IHC* (pp. 16–19) e orienta o tratamento de cada medida.

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

### 3.3 Priorização das cinco metas de Nielsen

Os pesos expressam as prioridades de projeto propostas pela equipe. MU01–MU07 permanecem como critérios operacionais da seção 3.2.

| Meta de Nielsen | Peso | Justificativa e relação com as medidas |
|---|---:|---|
| Baixa taxa de erros | 35% | Ajustar o saldo sem confirmar a origem afeta decisões seguintes. MU04 acompanha os erros críticos, MU02 verifica a interpretação de valores e MU01 verifica se a tarefa terminou corretamente. |
| Facilidade de aprendizado | 25% | Uma pessoa em seu primeiro uso precisa localizar o item, compreender as opções e concluir com autonomia. MU01 e MU02 caracterizam a primeira tentativa. MU06 compara a repetição equivalente. |
| Eficiência | 20% | A decisão precisa caber na rotina do comércio. MU03 mede o tempo ativo de uma conclusão independente. Interpretar a primeira tentativa à luz da experiência registrada e da curva de aprendizado. |
| Facilidade de memorização | 10% | Quem volta a conferir o estoque precisa reconhecer o caminho e recuperar o contexto. MU07 observa a retomada após uma pausa breve. Para medir retenção após dias sem uso, seria necessária outra sessão. |
| Satisfação positiva do usuário | 10% | A nota e o motivo registrados em MU05 mostram como a pessoa percebeu a experiência, inclusive quando concluiu a tarefa corretamente. |
| **Total** | **100%** | |

Um erro crítico em MU04 exige revisão mesmo que a tarefa seja rápida e receba nota alta. Os pesos orientam decisões de design e não são usados para somar os resultados dos testes.

## 4. Como o ciclo será iterado

Adotamos o **Ciclo de Vida da Engenharia de Usabilidade de Deborah Mayhew**. No recorte da Entrega 8, a equipe especifica os requisitos que orientarão o design.

**Onde o projeto está no modelo (25/11/2026).** A fase 1 está concluída como planejamento. Seus requisitos ainda dependem da coleta da E7. Na fase 2, os níveis 1 a 3 têm artefatos. O projeto está na **avaliação iterativa do nível 3**: a inspeção heurística (E13) está em andamento e a observação com usuários (E14) está prevista. A próxima etapa produz os achados da E13 e da E14 e a revisão do protótipo que deles resultar.

| Etapa do modelo de Mayhew | Artefato do projeto | Situação |
|---|---|---|
| **Fase 1 · Análise de requisitos** | | |
| Perfil do usuário | Personas P01/P02 (E3), problema e público (E1) | Concluído como hipótese; a validar pela E7 |
| Análise contextual das tarefas | Cenários E4-C01/C02 (E4); HTA, GOMS e CTT de T01/T02 (E5) | Concluído |
| Capacidades e restrições da plataforma | Seção 1 desta entrega | Concluído |
| Princípios gerais de design | Seção 2: negócio e interface | Concluído |
| Metas de usabilidade | Seção 3: qualitativas, MU01–MU07 e pesos de Nielsen | Concluído; limites mantidos sem piloto |
| Guia de estilo | Seção 2.3, com as decisões mínimas | Iniciado; atualizado em cada nível de design |
| **Fase 2 · Design, testes e desenvolvimento** | | |
| Nível 1 · modelo conceitual e mockups | Cartões da E6; modelo conceitual e DCC (E9); MoLIC M01/M02 (E10) | Concluído |
| Nível 1 · avaliação iterativa do modelo conceitual | Walkthrough da E6 com W01 (23/11) | Concluído, sem mudanças estruturais |
| Níveis 2 e 3 · padrões de tela e projeto detalhado | Protótipo navegável no Figma, com 28 estados (E11) | Concluído; revisado em 25/11 |
| Níveis 2 e 3 · avaliação iterativa | Plano DECIDE (E12), inspeção heurística (E13), observação com usuários (E14) | **Etapa atual**: E13 em andamento, E14 prevista |
| **Fase 3 · Instalação** | Acompanhamento do uso real | Fora do escopo da disciplina |

O retorno a etapas anteriores segue a regra do modelo. Um problema de **interpretação** (o que um dado ou uma ação significa) volta ao nível 1, ou seja, ao modelo conceitual e à MoLIC. Um problema de **apresentação** (rótulo, posição, estado ausente) volta aos níveis 2 e 3 e ao guia de estilo. Um achado sobre **quem faz o quê** na rotina volta à fase 1. Em todos os casos, a mudança é registrada na matriz de rastreabilidade, e a tarefa afetada é avaliada de novo.

| Fase do modelo | Aplicação no projeto | Quando voltar e o que rever |
|---|---|---|
| 1. Análise de requisitos | E3 e E4 descrevem perfis e cenários. E5 decompõe as tarefas. E7 prepara a investigação da rotina. E8 reúne características da plataforma, princípios, metas e decisões iniciais do guia de estilo. | Se a coleta mostrar que outra pessoa autoriza correções, rever R04-02, o fluxo de T02 e os controles de permissão antes de redesenhar as telas. |
| 2. Design, avaliação e desenvolvimento | No nível conceitual, E6 e E9 exploram decisões e caminhos. A MoLIC de E10 explicita a interação. No desenho de telas e no detalhamento, E11 aplica os padrões do guia e representa revisão, falha e retomada. E12 planeja a avaliação, E13 orienta a inspeção e E14 prevê a observação das tarefas. | Se alguém interpretar a confirmação em T01 como compra enviada, rever o rótulo e o resumo, atualizar o guia e repetir a verificação de MU02. Se T02 permitir correção sem evidência, rever o fluxo de pendência e testar novamente o caso B com MU04. |
| 3. Instalação e acompanhamento | Fase posterior a uma implantação real. Caberá acompanhar o uso no comércio e recolher dificuldades com registros, permissões e interrupções em condições reais. | Relatos recorrentes podem reabrir requisitos ou indicar ajustes de tela. Registrar o motivo, a versão alterada e a evidência obtida na nova avaliação. |

Na revisão formativa, a equipe modifica o protótipo e repete a tarefa afetada. Na rodada final da disciplina, compara os resultados da versão congelada com cada meta e registra limitações. A [matriz de rastreabilidade](../RASTREABILIDADE.md) liga as decisões às evidências previstas. O [plano DECIDE](12_planejamento_avaliacao.md) organiza as sessões.

**Preparação da avaliação.** Usar os casos A e B definidos na seção 3.2. Na ficha de cada tentativa, registrar versão, perfil, dispositivo, caso, tempo total e ativo, ajuda, erros críticos ou recuperados, explicações e motivo da nota. Em MU03, oferecer ajuda ou encerramento após 6 minutos em T01-A e 10 minutos em T02-A. Em MU07, a pausa controlada de 30 segundos antecede a medição do tempo de retomada. Se o fluxo necessário faltar, registrar a limitação e classificar a meta como não avaliada. Manter os registros individuais em acesso restrito.

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

- FEI, disciplina CC8122 — materiais de aula fornecidos pelo professor. *Princípios e Diretrizes de Design*, pp. 2–32, fundamenta os princípios, o guia de estilo e a fidelidade dos protótipos. *Planejamento da Avaliação de IHC*, pp. 11–19, 25–26 e 33–38, fundamenta as condições de avaliação, o piloto e o tratamento dos dados.
- FEI, disciplina CC8122 — materiais de aula *HTA* e *GOMS e CTT*, aplicados na [análise de tarefas da E5](05_analise_tarefas.md).
- Mayhew, Deborah J. (1999). Modelo de ciclo de vida utilizado na seção 4. [The Usability Engineering Lifecycle, Morgan Kaufmann](https://shop.elsevier.com/books/the-usability-engineering-lifecycle/mayhew/978-0-08-052028-5).
- Nielsen, Jakob (2012). Definição das cinco dimensões priorizadas na seção 3.3. [Usability 101, Nielsen Norman Group](https://www.nngroup.com/articles/usability-101-introduction-to-usability/jn/).
