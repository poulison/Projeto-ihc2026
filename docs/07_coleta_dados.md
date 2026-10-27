# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 23/10/2026

**Equipe:** 14 — Estoque com ML

**Status:** 🟨 em andamento.

**Responsabilidade:** soluções individuais e síntese da equipe.

## Objetivo e fundamentação

Investigar como responsáveis por pequenos comércios decidem reposições e conferem divergências para revisar P01 (Mariana), P02 (Rafael) e as tarefas T01/T02 da [Entrega 5](05_analise_tarefas.md). As personas são de expectativa, não participantes reais.

A Parte A segue as cinco categorias dos slides 2–7 de **CC8122-Identificacao Necessidades-A.pdf**: usuário, tecnologia, domínio, tarefas e motivações/valores. A Parte B utiliza questionário e entrevista conforme **CC8122-Identificacao Necessidades-B.pdf**, slides 3–9 e 20–21. A amostragem e os instrumentos abaixo são propostas específicas da equipe.

## Hipóteses e lacunas prioritárias

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

**Responsável acadêmico proposto:** Paulo Andre de Oliveira Hirata — 22.125.072-3.

**Foco:** P01, E4-C01, R04-01 e T01: analisar um produto e registrar uma decisão de reposição.

| Categoria / dados a coletar | Hipótese/lacuna relacionada | Necessidade e decisão de design |
|---|---|---|
| Usuário: função, experiência e faixa etária opcional | Usuário prioritário; pouca familiaridade digital | Descrever diversidade sem inferir habilidade pela idade |
| Tecnologia: dispositivos, ferramentas, conexão e autonomia | Registros distribuídos; processo atual | Definir plataforma, entrada de dados e ajuda compatíveis com a rotina |
| Domínio: significado de saldo, reserva e previsão | Conhecimento comercial e familiaridade com métricas | Distinguir disponibilidade, quantidade física e estimativa |
| Tarefas: última reposição, frequência, critérios, responsáveis e interrupções | Controle humano; acúmulo de tarefas | Definir sequência, revisão e retomada de T01 |
| Motivações/valores: prioridades, confiança, receios e aprendizagem | Benefício das previsões; percepção de incerteza | Investigar utilidade e formas de explicação e aprendizado |

**De quem coletar:** adultos que participam diretamente de decisões de reposição em pequenos comércios e fizeram isso nos últimos três meses. Incluir usuários de caderno, planilha ou sistema com diferentes níveis de autonomia digital; não exigir idade semelhante à persona. Proprietários definem critérios comerciais; funcionários descrevem a execução. Clientes e fornecedores são afetados por falta/excesso, mas não substituem usuários diretos nesta amostra.

**Aspectos éticos específicos:** dificuldades podem causar constrangimento. Explicar que não se avalia competência profissional. Não pedir faturamento, dívidas, margens ou nomes de clientes. Oferecer leitura assistida literal, sem orientar respostas, e registrar a modalidade para análise.

### A02 — Victor Merker Binda

**Responsável acadêmico proposto:** Victor Merker Binda — 22.125.075-6.

**Foco:** P02, E4-C02, R04-02 e T02: investigar uma divergência e registrar correção justificada ou pendência.

| Categoria / dados a coletar | Hipótese/lacuna relacionada | Necessidade e decisão de design |
|---|---|---|
| Usuário: papel, experiência e autonomia para alterar registros | Apoio operacional de um auxiliar | Confirmar se há auxiliar ou se o proprietário acumula tarefas |
| Tecnologia: fontes, transcrição, identificadores e dispositivos | Registros distribuídos; processo atual | Definir consulta de evidências e identificação de produtos |
| Domínio: unidade comercial, reserva, devolução e duplicidade | Conhecimento comercial e familiaridade com métricas | Evitar confusão entre produtos e unidades |
| Tarefas: conferência, causa, autorização, correção, pausa e comunicação | Esforço e falhas; interrupções | Determinar quando corrigir e quando deixar pendente |
| Motivações/valores: confiança no saldo, receio de apagar dados e ajuda | Controle humano; necessidade de histórico | Projetar revisão e alteração rastreável sem atribuir culpa ao usuário |

**De quem coletar:** adultos que registram movimentações ou conferem estoque e fizeram uma conferência nos últimos três meses. Buscar auxiliares e proprietários que trabalham sozinhos. A gestão esclarece autorização e processos; equipe técnica e orientador delimitam viabilidade e escopo. O processo efetivo é definido pela organização investigada, não pela persona.

**Aspectos éticos específicos:** relatos de erros podem expor funcionários. Entrevistar sem chefia acompanhando quando possível, não fornecer relatos individuais ao empregador e não copiar telas identificáveis. Aceitar exemplos sem nomes e sem informações comerciais reservadas.

### Proteções comuns e consentimento

Aplicar autonomia, prevenção de danos, benefício proporcional e tratamento justo, conforme material A, pp. 9–12. A referência à Resolução 196/96 nos slides é histórica: sua revogação consta da [Resolução CNS 466/2012](https://www.gov.br/conselho-nacional-de-saude/pt-br/atos-normativos/resolucoes/2012/resolucao-no-466.pdf/view). Conferir com o docente o enquadramento institucional antes da aplicação; este plano não declara aprovação ética.

- Participação voluntária, com possibilidade de pular perguntas ou desistir sem prejuízo. Não pressionar familiares, subordinados ou colegas.
- Usar códigos Q001/E001. Não pedir documento, endereço, renda ou diagnóstico. Separar contatos de recrutamento das respostas.
- Nesta versão, registrar apenas respostas e notas autorizadas, sem áudio, vídeo ou captura de tela. Gravações futuras exigem autorização específica e revisão do protocolo.
- Armazenar em pasta restrita à equipe, protegida por senha. Compartilhar com docente somente síntese sem identificação. Não colocar dados brutos no GitHub.
- Remover nomes de pessoas, estabelecimentos e detalhes que permitam identificação indireta. Código é pseudonimização, não anonimização automática.
- Prazo proposto: apagar respostas individuais e contatos até 90 dias após a avaliação final da disciplina, salvo exigência institucional comunicada previamente; conservar síntese efetivamente anonimizada.
- Informar contato institucional real do aplicador no convite e fornecer código de sessão. Permitir retirada enquanto o registro puder ser localizado; explicar que após anonimização irreversível não será possível localizar respostas individuais.

**Apresentação e consentimento, para ambos os instrumentos:**

> Somos Paulo Andre de Oliveira Hirata e Victor Merker Binda, estudantes de IHC da FEI. Queremos entender como pessoas controlam estoque e decidem reposições. Conforme o convite, a participação será em questionário de cerca de 10 minutos ou entrevista de cerca de 25 minutos. Não é avaliação do seu desempenho. Lembrar dificuldades pode gerar desconforto; você pode pular perguntas ou parar sem prejuízo. Não haverá gravação nem solicitação de dados de clientes ou valores financeiros. A equipe guardará os registros de forma restrita, pelo prazo informado acima, e apresentará somente síntese sem identificação. Não há benefício individual garantido. Você pode esclarecer dúvidas e solicitar retirada usando o contato do aplicador informado no convite e seu código, enquanto o registro puder ser localizado. Você entendeu e aceita participar?

Registrar aceita/não aceita e confirmar idade de 18 anos ou mais. Em caso de recusa, encerrar sem guardar respostas de pesquisa. O contato real precisa ser incluído no convite antes de aplicar; nenhum contato foi inventado.

## Parte B — instrumentos de coleta

### I01 — Questionário sobre decisão de reposição

**Responsável proposto:** Paulo Andre de Oliveira Hirata — 22.125.072-3.

**Objetivo:** caracterizar práticas, critérios e necessidades ligadas a T01.

**Público:** A01. **Duração estimada:** 8–12 minutos.

**Amostra planejada:** 8–12 participantes por conveniência, buscando diversidade de ferramentas e autonomia digital. Não representa estatisticamente todos os pequenos comércios.

#### Procedimento padronizado

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

**Q05. Onde registra ou consulta dados de estoque?** Múltiplas respostas: caderno/papel / planilha / sistema de vendas ou estoque / mensagens / plataforma de vendas online / não mantém registros / outro (qual?).

**Q06. Qual dispositivo mais utiliza nessa atividade?** Celular / computador ou notebook / tablet / não utiliza dispositivo digital / outro. **Q06a. Quando precisa de internet no trabalho, ela está disponível?** Sempre / na maioria das vezes / poucas vezes / nunca / não preciso / não sei.

**Q07. Como usa ferramentas digitais nessa atividade?** Sem ajuda / ajuda apenas em situações novas / ajuda frequente / outra pessoa faz essa parte / não uso.

**Q08. Com que frequência decide reposições?** Diariamente / algumas vezes por semana / semanalmente / quinzenalmente / mensalmente ou menos / quando surge necessidade, sem intervalo fixo / outra frequência.

**Q09. Pensando na última reposição, que informações utilizou para decidir?** Aberta; não fornecer exemplos antes da resposta.

**Q10. No último mês, quantas vezes interrompeu uma análise de reposição para atender outra demanda?** Nenhuma / 1–2 / 3–5 / 6 ou mais / não fiz essa análise / não lembro.

**Q11. No último mês, encontrou diferenças entre estoque registrado e disponível?** Não / sim / não mantenho registro / não sei. Se sim, **Q11a. Como lidou com a última diferença?** Aberta, sem nomes ou dados comerciais reservados.

**Q12. Como registra uma decisão de reposição para consultar depois?** Aberta; “não registro” é válido.

**Q13. Exemplo fictício: há 6 unidades, mas 2 estão reservadas para pedidos já feitos. Quantas estão livres para novas vendas?** Número livre / não sei. Não corrigir durante a aplicação.

**Q14. Exemplo fictício: “Estimativa de venda: 10 unidades nos próximos 7 dias; os valores reais podem variar”. O que isso significa para você?** Aberta. **Q14a. Que outras informações, se houver, procuraria antes de decidir uma compra?** Aberta.

**Q15. Qual a importância de cada aspecto em uma ferramenta de estoque?** Uma resposta por item: 1 nada importante / 2 pouco importante / 3 moderadamente importante / 4 importante / 5 muito importante / não se aplica. Itens: entender a origem dos valores; poder corrigir uma decisão; terminar rapidamente; consultar decisões anteriores.

**Q16. Como prefere aprender uma ferramenta nova?** Múltiplas respostas: demonstração de outra pessoa / instruções escritas / vídeo / experimentar com exemplos / outra forma / não sei.

**Q17. Qual a maior dificuldade na reposição e o que gostaria de melhorar?** Aberta; pode responder que não percebe dificuldade.

#### Análise

Apresentar contagens e denominadores válidos por pergunta, separando omissões, “não sei” e “não se aplica”. Em múltiplas respostas, a soma pode exceder o número de pessoas. Em Q15, apresentar distribuição e mediana por item; a escala mede importância declarada, não satisfação validada.

Agrupar respostas abertas por critérios comerciais, qualidade de dados, confiança, ferramentas e ajuda. Em Q13, interpretação esperada: 4 unidades. Em Q14, procurar reconhecimento de estimativa sujeita a variação, sem exigir jargão. Preservar respostas contrárias às hipóteses. Comparar modalidades e experiências somente descritivamente; opiniões não demonstram eficácia do sistema.

### I02 — Entrevista semiestruturada sobre conferência

**Responsável proposto:** Victor Merker Binda — 22.125.075-6.

**Objetivo:** compreender evidências, responsabilidades, correções e pendências em T02.

**Público:** A02. **Duração estimada:** 20–30 minutos.

**Amostra planejada:** 3–4 participantes por conveniência; buscar auxiliares e proprietários que conferem estoque, se acessíveis. Pessoas podem responder também I01, mas a sobreposição deve ser registrada e não contada como pessoas diferentes.

#### Procedimento padronizado

1. Preparar formulário online de notas com código, data, versão, papel, aceite e campos E01–E12, conforme material B, p. 21. O pesquisador registra as respostas durante a conversa. Configuração online pendente.
2. Fazer piloto, combinar local reservado e horário adequado, apresentar consentimento e confirmar conferência nos últimos três meses.
3. Seguir o roteiro; sondagens neutras permitidas: “Pode dar um exemplo?”, “O que aconteceu depois?” e “Como verificou?”. Não oferecer a solução projetada antes do relato atual.
4. Separar paráfrase de fala literal. Não solicitar acesso a sistemas reais. Em interrupção, oferecer retomada ou encerramento.
5. Ler um resumo ao participante para confirmar entendimento, aceitar correções, agradecer e fornecer código/contato. Revisar e desidentificar as notas.

#### Roteiro completo

| Pergunta | Sondagem / dado procurado |
|---|---|
| E01. Qual sua função e como participa da conferência? | Experiência; outras pessoas; proprietário sozinho ou auxiliar |
| E02. Como foi a última conferência, do começo ao fim? | Gatilho, sequência, ferramentas, duração aproximada e término |
| E03. Como identifica que dois registros tratam do mesmo produto e unidade de venda? | Código, nome, tamanho, kit e ambiguidades |
| E04. Qual foi a última diferença encontrada? Se nunca encontrou, como investigaria uma possível diferença? | Separar relato real de resposta hipotética |
| E05. Que informações verificou para entender a causa? | Fontes e evidências; não pressupor duplicidade |
| E06. Quem pode corrigir um registro e como decide o que alterar? | Responsabilidade, autorização e justificativa |
| E07. O que faz quando não consegue confirmar a causa? | Pendência e próxima verificação |
| E08. Já precisou parar uma conferência? Como soube onde continuar? | Interrupção, anotações, estratégias e perdas |
| E09. Como comunica o que resolveu e o que ainda falta conferir? | Item resolvido versus conjunto de registros |
| E10. O que faz confiar ou desconfiar do saldo? | Origem, atualização e consequências de erro, sem valores financeiros |
| E11. Que dificuldades encontra ao aprender ou usar ferramentas dessa tarefa? Como prefere ajuda? | Admitir ausência de dificuldade; vocabulário, leitura e autonomia |
| E12. Exemplo fictício: registro com 8 conjuntos e contagem de 10. O que verificaria antes de alterar? | Após resposta: se duas anotações puderem ser a mesma saída de 2 conjuntos, como confirmaria? Sem confirmação, o que faria? |

**Encerramento:** “O que não perguntamos e é importante nessa atividade?”, seguido de resumo para conferência. E12 é sondagem de raciocínio com dados fictícios; não comprova desempenho real.

#### Análise

Codificar episódios por identificação/unidade, fonte, causa, confirmação, autorização, correção, pendência, interrupção e comunicação. Paulo revisa a codificação de Victor; divergências são resolvidas consultando notas. Preservar casos contrários e distinguir relato, interpretação e proposta de design. Recorrência nesta amostra não representa prevalência nem prova saturação.

## Síntese e continuidade

| Evidência futura | Hipóteses/lacunas investigadas | Consequência |
|---|---|---|
| I01 Q01–Q12; I02 E01–E09 | Usuário prioritário, auxiliar, processo atual, registros distribuídos, vendas online, interrupções e falhas manuais | Rever personas, contexto e T01/T02 |
| I01 Q07/Q13–Q17; I02 E03/E10–E12 | Familiaridade digital, vocabulário, compreensão e confiança | Rever explicações, rótulos, ajuda e metas MU02/MU05/MU06 da E8 |
| I01 Q09/Q12/Q15; I02 E06–E10 | Controle humano e histórico | Definir revisão, rastreabilidade e retomada |
| Consulta ao orientador/documentação técnica | Escopo formal do TCC | Confirmar horizonte e eventual cálculo de reposição |

Depois da coleta, registrar por hipótese: pergunta e código da evidência, participantes que apoiam/contradizem, limitações, estado e mudança de design. Sustentada significa apoiada nesta amostra; contradições podem refutar ou refinar; ausência de dados mantém aberta. Questionários e entrevistas podem sofrer vieses de memória e desejabilidade social; observação futura poderá confrontá-los.

**Situação atual:** nenhum participante ou resultado reportado; nenhuma hipótese confirmada. Benefício real sobre falta/excesso exige acompanhamento posterior. As atribuições individuais são uma proposta de organização a ser revisada pelos integrantes.

## Checklist

- [x] Cinco categorias de dados e perfis específicos para cada integrante.
- [x] Hipóteses, tarefas e decisões relacionadas.
- [x] Ética, consentimento e análise contextualizados.
- [x] Duas técnicas distintas, incluindo questionário, com conteúdo integral.
- [ ] Configurar formulários online e contato institucional no convite.
- [ ] Realizar piloto, recrutamento e aplicação.
- [ ] Analisar respostas e atualizar hipóteses com evidências.

## Referências

- Material da disciplina, identificado como Barbosa e Silva (2010): **CC8122-Identificacao Necessidades-A.pdf**, pp. 2–13; **CC8122-Identificacao Necessidades-B.pdf**, pp. 3–9 e 20–21.
- **Planejamento Avaliacao IHC.pdf**, pp. 25–26 e 33–36: preparação, piloto e limites de interpretação.
- Entregas [1](01_conhecendo_o_problema.md), [3](03_personas_contexto_jornada.md), [4](04_cenarios_problema.md) e [5](05_analise_tarefas.md).
