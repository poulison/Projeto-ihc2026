# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 23/10/2026

**Revisão:** 08/11/2026

**Equipe:** 14 — Estoque com ML

**Status:** ✅ entrega fechada — partes A e B, instrumentos integrais, protocolo e aspectos éticos concluídos. As pendências de execução (formulários online, piloto e aplicação) estão declaradas no checklist e não foram simuladas.

**Responsabilidade:** 1 solução integrada por equipe, com partes individuais conforme o modelo da atividade.

## Objetivo da atividade

Investigar como responsáveis por pequenos comércios decidem reposições e conferem divergências para revisar P01 (Mariana), P02 (Rafael) e as tarefas T01/T02 da [Entrega 5](05_analise_tarefas.md). As personas são de expectativa, não participantes reais.

A Parte A segue as cinco categorias dos slides 2–7 de **CC8122-Identificacao Necessidades-A.pdf**: usuário, tecnologia, domínio, tarefas e motivações/valores. A Parte B utiliza questionário e entrevista conforme **CC8122-Identificacao Necessidades-B.pdf**, slides 2–9 e 20–21. A amostragem e os instrumentos abaixo são propostas específicas da equipe.

### Continuidade com as entregas anteriores

| Referência | Conteúdo preservado e aplicação na coleta |
|---|---|
| [E1 — problema](01_conhecendo_o_problema.md) | Investigar pequenos comércios e os relatos limitados de contagem e ruptura, sem apresentar hipóteses como fatos |
| [E2 — concorrência](02_analise_concorrencia.md) | RC02/RC07/RC08 orientam unidade, vocabulário e incerteza; RC09/RC11 orientam revisão e fontes de dados. Recursos dos concorrentes não comprovam necessidades locais |
| [E3 — personas e jornada](03_personas_contexto_jornada.md) | Paulo — Mariana/P01; Victor — Rafael/P02. Investigar autonomia, ajuda e interrupções sem deduzir habilidade pela idade |
| [E4 — cenários](04_cenarios_problema.md) | E4-C01/R04-01: disponibilidade, prazo, recursos e acompanhamento. E4-C02/R04-02: fontes, causa da divergência e comunicação |
| [E5 — tarefas](05_analise_tarefas.md) | T01 continua com Paulo e T02 com Victor. A coleta investiga a rotina que fundamenta esses modelos |
| [E6 — protótipo](06_prototipacao_papel.md) | PF01/PF02 oferecem cobertura parcial das tarefas. Investigar linguagem e dados antes de completar os fluxos; telas existentes não validam necessidades |

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

Mantêm-se as descrições por extenso da [rastreabilidade](../RASTREABILIDADE.md), sem recuperar códigos antigos.

| Hipótese/lacuna | Evidência atual | Decisão dependente da resposta | Prioridade |
|---|---|---|---|
| Responsável pelo estoque como usuário prioritário; apoio operacional de um auxiliar | Papéis hipotéticos de E1/E3 | Quem executa T01/T02 e quem autoriza alterações | Alta |
| Processo e dados atuais; registros distribuídos entre ferramentas | Relatos da equipe sobre contagem e ruptura; processo completo desconhecido | Fontes, entrada de dados e necessidade de consolidação | Alta |
| Conhecimento comercial e familiaridade com métricas; pouca familiaridade digital de Mariana | Construção de P01 | Vocabulário, aprendizagem e ajuda | Alta |
| Compreensão dos resultados sem formação em ML; percepção de incerteza e confiança | Sem pesquisa primária | Explicação de estimativas e de informação insuficiente | Alta |
| Esforço e falhas na consolidação manual | Duplicidade fictícia em E4-C02 | Evidências para corrigir ou deixar pendente | Alta |
| Controle humano da decisão; acúmulo de tarefas e interrupções | Propostas em E3/E4 | Revisão, salvamento e retomada | Alta |
| Necessidade de histórico de previsões e decisões; vendas online | Hipóteses de E1/E3 | Histórico e canais efetivamente necessários | Média |
| Benefício das previsões para antecipar reposições | Benefício esperado, não medido | Investigar utilidade percebida; efeito real requer acompanhamento posterior | Média |
| Escopo formal do TCC | Recomendação calculada não confirmada | Confirmar dados, horizonte e funções com orientador | Alta |

## Parte A — necessidades e requisitos de IHC

### A01 — Paulo Andre de Oliveira Hirata

**Autor(a):** Paulo Andre de Oliveira Hirata — 22.125.072-3.

**Foco:** P01, E4-C01, R04-01 e T01: analisar um produto e registrar uma decisão de reposição.

#### Que dados coletar?

| Categoria / dados a coletar | Hipótese/lacuna relacionada | Necessidade e decisão de design |
|---|---|---|
| Usuário: função, experiência e faixa etária opcional | Usuário prioritário; pouca familiaridade digital | Descrever diversidade sem inferir habilidade pela idade |
| Tecnologia: dispositivos, ferramentas, conexão e autonomia | Registros distribuídos; processo atual | Definir plataforma, entrada de dados e ajuda compatíveis com a rotina |
| Domínio: significado de saldo, reserva e previsão | Conhecimento comercial e familiaridade com métricas | Distinguir disponibilidade, quantidade física e estimativa |
| Tarefas: última reposição, frequência, critérios, responsáveis e interrupções | Controle humano; acúmulo de tarefas | Definir sequência, revisão e retomada de T01 |
| Motivações/valores: prioridades, confiança, receios e aprendizagem | Benefício das previsões; percepção de incerteza | Investigar utilidade e formas de explicação e aprendizado |

#### De quem coletar?

Adultos que participam diretamente de decisões de reposição em pequenos comércios e fizeram isso nos últimos três meses. Incluir usuários de caderno, planilha ou sistema com diferentes níveis de autonomia digital; não exigir idade semelhante à persona. Proprietários definem critérios comerciais; funcionários descrevem a execução. Clientes e fornecedores são afetados por falta/excesso, mas não substituem usuários diretos nesta amostra.

#### Aspectos éticos

Dificuldades podem causar constrangimento. Explicar que não se avalia competência profissional. Não pedir faturamento, dívidas, margens ou nomes de clientes. Oferecer leitura assistida literal, sem orientar respostas, e registrar a modalidade para análise.

### A02 — Victor Merker Binda

**Autor(a):** Victor Merker Binda — 22.125.075-6.

**Foco:** P02, E4-C02, R04-02 e T02: investigar uma divergência e registrar correção justificada ou pendência.

#### Que dados coletar?

| Categoria / dados a coletar | Hipótese/lacuna relacionada | Necessidade e decisão de design |
|---|---|---|
| Usuário: papel, experiência e autonomia para alterar registros | Apoio operacional de um auxiliar | Confirmar se há auxiliar ou se o proprietário acumula tarefas |
| Tecnologia: fontes, transcrição, identificadores e dispositivos | Registros distribuídos; processo atual | Definir consulta de evidências e identificação de produtos |
| Domínio: unidade comercial, reserva, devolução e duplicidade | Conhecimento comercial e familiaridade com métricas | Evitar confusão entre produtos e unidades |
| Tarefas: conferência, causa, autorização, correção, pausa e comunicação | Esforço e falhas; interrupções | Determinar quando corrigir e quando deixar pendente |
| Motivações/valores: confiança no saldo, receio de apagar dados e ajuda | Controle humano; necessidade de histórico | Projetar revisão e alteração rastreável sem atribuir culpa ao usuário |

#### De quem coletar?

Adultos que registram movimentações ou conferem estoque e fizeram uma conferência nos últimos três meses. Buscar auxiliares e proprietários que trabalham sozinhos. A gestão esclarece autorização e processos; equipe técnica e orientador delimitam viabilidade e escopo. O processo efetivo é definido pela organização investigada, não pela persona.

#### Aspectos éticos

Relatos de erros podem expor funcionários. Entrevistar sem chefia acompanhando quando possível, não fornecer relatos individuais ao empregador e não copiar telas identificáveis. Aceitar exemplos sem nomes e sem informações comerciais reservadas.

### Proteções comuns e consentimento

Os quatro princípios do material A, pp. 10–11, orientam as medidas desta coleta. A referência à Resolução 196/96 nos slides é histórica: sua revogação consta da [Resolução CNS 466/2012](https://www.gov.br/conselho-nacional-de-saude/pt-br/atos-normativos/resolucoes/2012/resolucao-no-466.pdf/view). Conferir com o docente o enquadramento institucional antes da aplicação; este plano não declara aprovação ética.

| Princípio (material A) | Como é aplicado nesta coleta |
|---|---|
| Não maleficência — evitar danos previsíveis, imediatos ou tardios | Não perguntar faturamento, dívidas, margens, dados de clientes nem diagnósticos; não relatar ao empregador o desempenho individual de um funcionário; não registrar áudio, vídeo ou tela |
| Justiça e equidade — relevância social e cuidado com participantes vulneráveis | Não recrutar por pressão hierárquica ou familiar; entrevistar sem chefia presente quando possível; oferecer leitura assistida a quem tiver dificuldade de leitura, em vez de excluir a pessoa |
| Autonomia — consentimento livre e esclarecido e proteção de grupos vulneráveis | Convite com objetivo, duração, riscos e contato; aceite registrado; apenas maiores de 18 anos; qualquer pergunta pode ser pulada e a participação interrompida sem prejuízo |
| Beneficência — ponderar riscos e benefícios | Coletar apenas o necessário para rever personas e tarefas; informar que não há benefício individual garantido; o benefício esperado é melhorar o projeto, não resolver o estoque do participante |

Medidas práticas decorrentes, aplicáveis aos dois instrumentos:

- Participação voluntária, com possibilidade de pular perguntas ou desistir sem prejuízo. Não pressionar familiares, subordinados ou colegas.
- Usar códigos Q001/E001. Não pedir documento, endereço, renda ou diagnóstico. Separar contatos de recrutamento das respostas.
- Nesta versão, registrar apenas respostas e notas autorizadas, sem áudio, vídeo ou captura de tela. Gravações futuras exigem autorização específica e revisão do protocolo.
- Armazenar em pasta restrita à equipe, protegida por senha. Compartilhar com docente somente síntese sem identificação. Não colocar dados brutos no GitHub.
- Remover nomes de pessoas, estabelecimentos e detalhes que permitam identificação indireta. Código é pseudonimização, não anonimização automática.
- Prazo proposto: apagar respostas individuais e contatos até 90 dias após a avaliação final da disciplina, salvo exigência institucional comunicada previamente; conservar síntese efetivamente anonimizada.
- Informar o contato do aplicador — victor.merker.bindaa@gmail.com — no convite e fornecer código de sessão. Permitir retirada enquanto o registro puder ser localizado; explicar que após anonimização irreversível não será possível localizar respostas individuais.

**Apresentação e consentimento, para ambos os instrumentos:**

**Contato para dúvidas e retirada de respostas:** Victor Merker Binda — victor.merker.bindaa@gmail.com (endereço confirmado pelo integrante).

> Somos Paulo Andre de Oliveira Hirata e Victor Merker Binda, estudantes de IHC da FEI. Queremos entender como pessoas controlam estoque e decidem reposições. Conforme o convite, a participação será em questionário de cerca de 10 minutos ou entrevista de cerca de 25 minutos. Não é avaliação do seu desempenho. Lembrar dificuldades pode gerar desconforto; você pode pular perguntas ou parar sem prejuízo. Não haverá gravação nem solicitação de dados de clientes ou valores financeiros. A equipe guardará os registros de forma restrita, pelo prazo informado acima, e apresentará somente síntese sem identificação. Não há benefício individual garantido. Você pode esclarecer dúvidas e solicitar retirada usando o contato victor.merker.bindaa@gmail.com e seu código, enquanto o registro puder ser localizado. Você entendeu e aceita participar?

Registrar aceita/não aceita e confirmar idade de 18 anos ou mais. Em caso de recusa, encerrar sem guardar respostas de pesquisa. Incluir o contato confirmado acima no convite e na descrição dos dois formulários.

## Parte B — ferramentas de coleta

Cada integrante prepara uma técnica completa e diferente: Paulo, questionário; Victor, entrevista semiestruturada. O questionário descreve práticas e prioridades de forma comparável; a entrevista aprofunda a sequência e as evidências de um episódio. Ambos investigam necessidades; ainda não são testes de usabilidade do protótipo.

### Escolha dos métodos entre as alternativas do material B

O material B, p. 2, lista sete métodos de coleta. A escolha considerou objetivo, acesso a participantes e prazo, atendendo à orientação de p. 20 de não adotar um método qualquer.

| Método (material B) | Decisão | Justificativa |
|---|---|---|
| Entrevista (p. 3) | **Adotado — I02** | É o método da lista que permite detalhar a sequência de um episódio real de conferência e as evidências consultadas, necessário para T02. Contrapartida: exige treinar o entrevistador e leva tempo por participante |
| Questionário (p. 6) | **Adotado — I01** | Descreve práticas, ferramentas e prioridades de forma comparável entre pessoas, com baixo custo por participante, cobrindo a diversidade de rotinas de T01. Contrapartida: respostas mais superficiais |
| Grupo de foco (p. 10) | Não adotado nesta entrega | Exige reunir de três a dez pessoas no mesmo horário e moderação experiente; além disso, relatar erros de estoque diante de colegas ou da chefia agrava o risco ético descrito em A02 |
| Brainstorming de necessidades e desejos (p. 12) | Não adotado nesta entrega | Pressupõe de 8 a 12 usuários reunidos e explora desejos, enquanto esta etapa precisa primeiro descrever a rotina atual |
| Classificação de cartões (p. 13) | Adiado para o redesenho | Informa arquitetura de informação, menus e navegação; torna-se útil depois que a coleta definir vocabulário e agrupamentos para E9–E11 |
| Estudo de campo (p. 15) | Adiado | Registraria interrupções e distrações no próprio comércio, o que fortaleceria as hipóteses de E3/E4, mas depende de autorização do estabelecimento e de disponibilidade não assegurada nesta etapa |
| Investigação contextual (p. 17) | Adiado | O modelo mestre-aprendiz exigiria acompanhar o trabalho em execução; mesma restrição de acesso do estudo de campo, com envolvimento ainda maior do investigador |

Os dois métodos adotados são declarativos: registram o que a pessoa relata, não o que faz. Observação em contexto, se viável em etapa posterior, poderá confrontar esses relatos.

### Instrumento, protocolo e amostra (material B, p. 20)

- **Instrumento:** o material usado para realizar a coleta. Aqui são o formulário de I01, o roteiro e o formulário de notas de I02, mais o convite e o texto de consentimento.
- **Protocolo de execução:** é o instrumento mais importante porque o mesmo questionário ou roteiro produz dados diferentes conforme a forma de aplicar. Ordem das perguntas, leitura literal, sondagens permitidas, o que o aplicador não pode explicar e o registro da modalidade determinam se as respostas de pessoas diferentes são comparáveis e se o viés do aplicador fica controlado. Os procedimentos padronizados de I01 e I02 cumprem essa função e devem ser seguidos sem improviso; qualquer desvio é anotado na ficha de análise.
- **Amostra:** depende do método e do contexto do projeto. O questionário admite mais participantes porque o custo por resposta é baixo; a entrevista é limitada pelo tempo de condução e de análise. Por isso I01 propõe 8–12 e I02 propõe 3–4 pessoas, por conveniência. Nenhuma das faixas é amostra probabilística nem quantidade prescrita pelos slides.

### Instrumento I01 — Questionário sobre decisão de reposição

**Autor(a):** Paulo Andre de Oliveira Hirata — 22.125.072-3.

**Técnica:** questionário.

**Objetivo:** caracterizar práticas, critérios e necessidades ligadas a T01.

**Público:** A01. **Duração estimada:** 10–15 minutos, a conferir no piloto.

**Amostra planejada (proposta exploratória da equipe, não quantidade exigida nos slides):** 8–12 participantes por conveniência, buscando diversidade de ferramentas e autonomia digital. Não representa estatisticamente todos os pequenos comércios.

#### Procedimento padronizado de aplicação

1. Transpor o questionário para Google Forms ou ferramenta institucional equivalente, conforme material B, p. 21. Desativar coleta de e-mail e exigência de login, quando disponível, e conferir configurações. **Formulário online ainda não publicado; cópia textual completa abaixo.**
2. Fazer piloto com uma pessoa elegível, verificando compreensão, duração e ramificações. Excluir o piloto da análise principal se houver alterações relevantes; registrar versão.
3. Apresentar consentimento, critério etário e Q01; encerrar se não elegível. Demais respostas são opcionais, sempre permitindo “prefiro não responder”.
4. Aplicar individualmente; na leitura assistida, ler literalmente sem explicar respostas corretas. Registrar código, versão e modalidade.
5. Agradecer, fornecer código/contato, exportar para pasta restrita e retirar identificadores eventualmente escritos antes de divulgar síntese.

#### Questionário completo

**Q01. Nos últimos três meses, participou da decisão de comprar produtos para repor estoque de um pequeno comércio?** Sim / não. Se não, encerrar.

**Q02. Qual sua participação?** Múltiplas respostas: decido o que comprar / reúno informações / confiro estoque / aprovo o valor da compra / outra (qual?).

**Q03. Há quanto tempo realiza essa atividade?** Menos de 6 meses / de 6 meses a menos de 2 anos / de 2 a 5 anos / mais de 5 anos.

**Q04. Qual sua faixa etária?** 18–29 / 30–44 / 45–59 / 60 ou mais / prefiro não responder. Opcional; não usar para inferir habilidade.

**Q05. Onde registra ou consulta dados de estoque?** Múltiplas respostas: caderno/papel / planilha / sistema de vendas ou estoque / mensagens / plataforma de vendas online / não mantém registros / outro (qual?). A opção “não mantém registros” é exclusiva das demais.

**Q06. Qual dispositivo mais utiliza nessa atividade?** Celular / computador ou notebook / tablet / não utiliza dispositivo digital / outro. **Q06a. Quando precisa de internet no trabalho, ela está disponível?** Sempre / na maioria das vezes / poucas vezes / nunca / não preciso / não sei.

**Q07. Como usa ferramentas digitais nessa atividade?** Sem ajuda / ajuda apenas em situações novas / ajuda frequente / outra pessoa faz essa parte / não uso.

**Q08. Com que frequência decide reposições?** Diariamente / algumas vezes por semana / semanalmente / quinzenalmente / mensalmente ou menos / quando surge necessidade, sem intervalo fixo / outra frequência.

**Q09. Pensando na última reposição, que informações utilizou para decidir?** Aberta; não fornecer exemplos antes da resposta.

**Q09a. Como o prazo do fornecedor e os recursos disponíveis influenciaram essa decisão, se influenciaram?** Aberta; não solicitar valores financeiros. Aplicar depois de Q09 e distinguir resposta espontânea de resposta estimulada.

**Q10. No último mês, quantas vezes interrompeu uma análise de reposição para atender outra demanda?** Nenhuma / 1–2 / 3–5 / 6 ou mais / não fiz essa análise / não lembro.

**Q11. No último mês, encontrou diferenças entre estoque registrado e disponível?** Não / sim / não mantenho registro / não sei. Se sim, **Q11a. Como lidou com a última diferença?** Aberta, sem nomes ou dados comerciais reservados.

**Q12. Como registra uma decisão de reposição para consultar depois?** Aberta; “não registro” é válido.

**Q12a. Depois da chegada dos produtos, como verifica se a reposição foi adequada?** Aberta; pode responder que não acompanha. Investiga a jornada da E3/E4, sem ampliar o término de T01, que na E5 acaba no registro da decisão.

**Q13. Exemplo fictício: há 6 unidades, mas 2 estão reservadas para pedidos já feitos. Quantas estão livres para novas vendas?** Número livre / não sei. Não corrigir durante a aplicação.

**Q14. Exemplo fictício: “Estimativa de venda: 10 unidades nos próximos 7 dias; os valores reais podem variar”. O que isso significa para você?** Aberta. **Q14a. Que outras informações, se houver, procuraria antes de decidir uma compra?** Aberta.

**Q14b. Em que situações uma estimativa assim ajudaria ou não ajudaria sua rotina?** Aberta; utilidade declarada não demonstra benefício real sobre faltas e excessos.

**Q15. Qual a importância de cada aspecto em uma ferramenta de estoque?** Uma resposta por item: 1 nada importante / 2 pouco importante / 3 moderadamente importante / 4 importante / 5 muito importante / não se aplica. Itens: entender a origem dos valores; poder corrigir uma decisão; terminar rapidamente; consultar decisões anteriores.

**Q16a. Ao consultar informações de estoque, que dificuldades de leitura ou compreensão encontra, se houver?** Aberta; não pedir diagnóstico nem escolaridade.

**Q16. Como prefere aprender uma ferramenta nova?** Múltiplas respostas: demonstração de outra pessoa / instruções escritas / vídeo / experimentar com exemplos / outra forma / não sei.

**Q17. Qual a maior dificuldade na reposição e o que gostaria de melhorar?** Aberta; pode responder que não percebe dificuldade.

#### Tipos de pergunta utilizados

Classificação conforme o material B, pp. 5 e 7–9.

| Tipo (material B) | Perguntas de I01 | Motivo da escolha |
|---|---|---|
| Fechada — escolha de um valor (p. 7) | Q01, Q03, Q06, Q06a, Q07, Q08, Q11 | Respostas comparáveis entre participantes e contagem direta |
| Fechada — escolha de vários valores (p. 7) | Q02, Q05, Q16 | A pessoa pode acumular papéis, ferramentas e formas de aprender; a soma pode exceder o número de participantes |
| Fechada — faixa de valores (p. 7) | Q04, faixa etária; Q10, contagem de interrupções em faixas | Evita pedir idade exata e reduz erro de memória em contagens |
| Escala de Likert (p. 8) | Q15, um item por linha | Mede importância declarada de quatro aspectos com a mesma régua de cinco pontos |
| Diferenciais semânticos (p. 8) | Não utilizado nesta entrega | Os pares de adjetivos do exemplo do slide avaliam a impressão sobre uma interface existente; esta coleta ainda investiga a rotina atual. O recurso fica reservado às avaliações das E12–E14 |
| Aberta (pp. 5 e 9) | Q09, Q09a, Q11a, Q12, Q12a, Q13 como resposta curta numérica com opção “não sei”, Q14, Q14a, Q14b, Q16a, Q17 e os campos “outra/qual?” das fechadas | Exploram critérios, significados e dificuldades sem restringir o tipo ou o tamanho da resposta nem sugerir alternativas |

As perguntas abertas vêm antes das fechadas equivalentes sempre que a alternativa poderia sugerir a resposta: por isso Q09 precede Q09a e Q14 precede Q14a/Q14b. Conforme o material B, p. 6, o questionário tende a produzir respostas mais superficiais que a entrevista; I02 compensa essa limitação aprofundando um episódio.

#### Como os dados serão analisados

Apresentar contagens e denominadores válidos por pergunta, separando omissões, “não sei” e “não se aplica”. Em múltiplas respostas, a soma pode exceder o número de pessoas. Em Q15, apresentar distribuição e mediana por item; a escala mede importância declarada, não satisfação validada.

Agrupar respostas abertas por critérios comerciais, qualidade de dados, confiança, ferramentas e ajuda. Em Q13, interpretação esperada: 4 unidades. Em Q14, procurar reconhecimento de estimativa sujeita a variação, sem exigir jargão. Preservar respostas contrárias às hipóteses. Comparar modalidades e experiências somente descritivamente; opiniões não demonstram eficácia do sistema. Q13/Q14 avaliam os exemplos fornecidos, não a interface. Q14 explicita que os valores variam; a resposta não prova reconhecimento espontâneo da incerteza. Registrar também casos em que a previsão não ajudaria (Q14b).

### Instrumento I02 — Entrevista semiestruturada sobre conferência

**Autor(a):** Victor Merker Binda — 22.125.075-6.

**Técnica:** entrevista semiestruturada.

**Por que semiestruturada (material B, p. 3):** a entrevista estruturada fixaria ordem e texto e impediria aprofundar um episódio inesperado; a não estruturada dificultaria comparar relatos entre participantes e exigiria mais experiência do entrevistador. O roteiro fixo E01–E12 garante os mesmos temas em todas as sessões, e as sondagens previstas permitem detalhar o caso relatado. Como o material alerta que é necessário treinar os entrevistadores, o piloto também serve para o aplicador exercitar sondagem neutra e registro simultâneo.

**Objetivo:** compreender evidências, responsabilidades, correções e pendências em T02.

**Público:** A02. **Duração estimada:** 20–30 minutos.

**Amostra planejada (proposta exploratória da equipe, não quantidade exigida nos slides):** 3–4 participantes por conveniência; buscar auxiliares e proprietários que conferem estoque, se acessíveis. Pessoas podem responder também I01, mas a sobreposição deve ser registrada e não contada como pessoas diferentes.

#### Procedimento padronizado de aplicação

1. Preparar formulário online de notas com código, data, versão, papel, aceite e campos E01–E12, conforme material B, p. 21. O pesquisador registra as respostas durante a conversa. Configuração online pendente.
2. Fazer piloto, combinar local reservado e horário adequado, apresentar consentimento e confirmar conferência nos últimos três meses.
3. Seguir o roteiro; sondagens neutras permitidas: “Pode dar um exemplo?”, “O que aconteceu depois?” e “Como verificou?”. Não oferecer a solução projetada antes do relato atual.
4. Separar paráfrase de fala literal. Não solicitar acesso a sistemas reais. Em interrupção, oferecer retomada ou encerramento.
5. Ler um resumo ao participante para confirmar entendimento, aceitar correções, agradecer e fornecer código/contato. Revisar e desidentificar as notas.

#### Roteiro completo

| Pergunta | Sondagem / dado procurado |
|---|---|
| E01. Qual sua função e como participa da conferência? | Experiência; outras pessoas; proprietário sozinho ou auxiliar; ferramentas e dispositivos utilizados |
| E02. Como foi a última conferência, do começo ao fim? | Gatilho, sequência, ferramentas, duração aproximada e término |
| E03. Como identifica que dois registros tratam do mesmo produto e unidade de venda? | Código, nome, tamanho, kit e ambiguidades |
| E04. Qual foi a última diferença encontrada? Se nunca encontrou, como investigaria uma possível diferença? | Separar relato real de resposta hipotética |
| E05. Que informações verificou para entender a causa? | Fontes, momento e responsável pelos registros; tratamento de reservas, cancelamentos e devoluções, se ocorrerem. Não pressupor duplicidade |
| E06. Quem pode corrigir um registro e como decide o que alterar? | Responsabilidade, autorização e justificativa |
| E07. O que faz quando não consegue confirmar a causa? | Pendência e próxima verificação |
| E08. Já precisou parar uma conferência? Como soube onde continuar? | Interrupção, anotações, estratégias e perdas |
| E09. Como comunica o que resolveu e o que ainda falta conferir? | Item resolvido versus conjunto de registros |
| E10. O que faz confiar ou desconfiar do saldo? | Origem, atualização e consequências de erro, sem valores financeiros |
| E11. Que dificuldades encontra ao aprender ou usar ferramentas dessa tarefa? Como prefere ajuda? | Admitir ausência de dificuldade; vocabulário, leitura, autonomia e receios de alterar registros |
| E12. Exemplo fictício: registro com 8 conjuntos e contagem de 10. O que verificaria antes de alterar? | Após resposta: se duas anotações puderem ser a mesma saída de 2 conjuntos, como confirmaria? Sem confirmação, o que faria? |

**Encerramento:** “O que não perguntamos e é importante nessa atividade?”, seguido de resumo para conferência. E12 é sondagem de raciocínio com dados fictícios; não comprova desempenho real.

#### Como os dados serão analisados

Codificar episódios por identificação/unidade, fonte, causa, confirmação, autorização, correção, pendência, interrupção e comunicação. A equipe consolida a codificação e resolve divergências consultando as notas. Preservar casos contrários e distinguir relato, interpretação e proposta de design. Recorrência nesta amostra não representa prevalência nem prova saturação.

## Síntese

| Evidência futura | Hipóteses/lacunas investigadas | Consequência |
|---|---|---|
| I01 Q01–Q12; I02 E01–E09 | Usuário prioritário, auxiliar, processo atual, registros distribuídos, vendas online, interrupções e falhas manuais | Rever personas, contexto e T01/T02 |
| I01 Q07/Q13–Q17; I02 E03/E10–E12 | Familiaridade digital, vocabulário, compreensão e confiança | Rever explicações, rótulos, ajuda e metas MU02/MU05/MU06 da E8 |
| I01 Q09/Q09a/Q12/Q12a/Q15; I02 E06–E10 | Controle humano e histórico | Definir revisão, rastreabilidade e retomada |
| Consulta ao orientador/documentação técnica | Escopo formal do TCC | Confirmar horizonte e eventual cálculo de reposição |

Depois da coleta, registrar por hipótese: pergunta e código da evidência, participantes que apoiam/contradizem, limitações, estado e mudança de design. Sustentada significa apoiada nesta amostra; contradições podem refutar ou refinar; ausência de dados mantém aberta. Questionários e entrevistas podem sofrer vieses de memória e desejabilidade social; observação futura poderá confrontá-los.

**Situação atual:** nenhum participante ou resultado reportado; nenhuma hipótese confirmada. Benefício real sobre falta/excesso exige acompanhamento posterior.

### Registro e configuração dos instrumentos

**Convite de recrutamento, em versão final:** “Somos estudantes de IHC da FEI e estamos estudando a rotina de estoque de pequenos comércios. Procuramos pessoas adultas que tenham participado de reposição ou conferência nos últimos três meses. A participação é voluntária, sem gravação e sem solicitar valores financeiros ou dados de clientes. O questionário leva aproximadamente 10–15 minutos; a entrevista, 20–30 minutos. Você pode recusar ou interromper sem prejuízo. Dúvidas e pedidos de retirada podem ser enviados a victor.merker.bindaa@gmail.com. Podemos explicar o estudo?” O convite é enviado por Victor Merker Binda, pelo endereço acima, que fica disponível para dúvidas e retirada; não publicar contatos de participantes.

| Configuração | I01 — questionário | I02 — entrevista |
|---|---|---|
| Título online | Estoque com ML — Rotina de reposição | Estoque com ML — Roteiro de conferência |
| Introdução | Texto integral de consentimento desta entrega, prazo de retenção e o contato victor.merker.bindaa@gmail.com | Mesmo texto, com duração da entrevista |
| Triagem obrigatória | Aceite sim/não; 18 anos ou mais sim/não; Q01. Qualquer “não” encerra antes das perguntas de pesquisa | Aceite e maioridade; confirmar conferência nos últimos três meses antes de E01 |
| Conteúdo | Q01–Q17 e subperguntas; todas opcionais após triagem. Q11a somente se Q11 = sim | Campos E01–E12 preenchidos pelo entrevistador; anotar não respondido ou não aplicável sem inferir resposta |
| Tipos | Q02/Q05/Q16: múltipla escolha de várias opções; Q15: escala por item; demais conforme o texto | Campos de texto longo; E12 marcado como exemplo fictício |
| Privacidade | Sem coleta automática de e-mail; verificar ausência de exigência de login; desativar visualização pública de respostas | Formulário de notas restrito à equipe, sem acesso público às respostas |
| Identificação | Código aleatório sem nome, fornecido no convite individual e inserido no formulário; registrar modalidade assistida/autônoma | Código, data, duração, versão do roteiro, aceite e função; contatos guardados separadamente |
| Encerramento | Agradecer; lembrar o código e o canal para dúvidas/retirada | Ler o resumo ao participante e registrar correções de interpretação |

No questionário, revisar incompatibilidades como “não mantém registros” junto a ferramentas. Se a ferramenta não permitir impedir a combinação, orientar no enunciado e registrar a inconsistência sem corrigir por suposição. “Não sei”/“prefiro não responder” em questões múltiplas também devem ser exclusivos das respostas substantivas.

**Ficha mínima de análise, a preencher somente depois da aplicação:** código da pessoa; instrumento/versão; pergunta; resposta ou nota autorizada; relato real/exemplo hipotético; tema; hipótese relacionada; evidência favorável/contrária/inconclusiva; limitação; decisão de design. Para participação nos dois instrumentos, manter ligação privada entre os códigos e contar a pessoa uma única vez no total de participantes.

**Critério para encerrar a análise:** contabilizar participantes elegíveis e respostas válidas; revisar todos os temas e casos discordantes; classificar cada hipótese como sustentada no contexto, refutada, refinada ou ainda aberta; apontar o que muda nas personas/tarefas e justificar o que permanece. Não preencher percentuais, falas ou conclusões antes da coleta.

### O que ainda depende da equipe

O conteúdo escrito, os dois instrumentos, o protocolo de execução, o convite e o termo de consentimento estão fechados nesta versão, já com o contato real, e podem ser aplicados como estão. Para atender também à orientação de ferramenta online do material B, resta transcrever o questionário para um formulário seguindo a tabela de configuração acima e registrar o link neste arquivo — transcrição, não nova redação. Depois, realizar piloto e ajustar a duração. A aplicação e a análise exigem participantes reais, caso sejam solicitadas nesta etapa pelo docente; o modelo do repositório enfatiza planejamento e instrumentos, e não autoriza inventar resultados. As faixas de amostra propostas podem ser revistas antes do recrutamento, com justificativa de acesso e objetivo exploratório.

## Checklist

- [x] Cinco categorias de dados e perfis específicos para cada integrante.
- [x] Hipóteses, tarefas e decisões relacionadas.
- [x] Ética, consentimento e análise contextualizados.
- [x] Duas técnicas distintas, incluindo questionário, com conteúdo integral.
- [x] Escolha dos métodos justificada diante das sete alternativas do material B.
- [x] Tipos de pergunta e papel do protocolo de execução explicitados.
- [x] Definir contato real para dúvidas e retirada: victor.merker.bindaa@gmail.com.
- [x] Convite e termo de consentimento finalizados com o contato real, prontos para envio.
- [ ] Transcrever os instrumentos para formulário online e registrar os links aqui.
- [ ] Realizar piloto, recrutamento e aplicação.
- [ ] Analisar respostas e atualizar hipóteses com evidências.

## Referências

- Material da disciplina, identificado como Barbosa e Silva (2010): **CC8122-Identificacao Necessidades-A.pdf**, pp. 2–13, com os princípios éticos nas pp. 10–11; **CC8122-Identificacao Necessidades-B.pdf**, p. 2 para o conjunto de métodos, pp. 3–9 para entrevista, questionário e tipos de pergunta, pp. 10–19 para os métodos não adotados nesta etapa e pp. 20–21 para instrumento, protocolo, amostra e ferramenta online.
- **Planejamento Avaliacao IHC.pdf**, pp. 25–26 e 33–36: preparação, piloto e limites de interpretação.
- Entregas [1](01_conhecendo_o_problema.md), [2](02_analise_concorrencia.md), [3](03_personas_contexto_jornada.md), [4](04_cenarios_problema.md), [5](05_analise_tarefas.md) e [6](06_prototipacao_papel.md).
