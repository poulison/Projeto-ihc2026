# Entrega 3 — Personas, mapa de empatia, contexto de uso e jornada

**Data:** 02/09/2026 
**Status:** 🟨 iniciada  
**Responsabilidade:** 1 persona por integrante; 1 mapa de empatia, 1 contexto de uso consolidado e 1 jornada por equipe (salvo orientação diferente do docente).

## Objetivo da atividade

Representar grupos de usuários de forma útil para decisões de design. Persona não é personagem decorativo: suas características devem alterar requisitos, prioridades, linguagem, fluxos ou critérios de avaliação.

## Atenção a projetos técnicos

Em TCCs sem interface original, a persona pode representar um **profissional que se apropria da contribuição técnica**: DBA, analista, cientista de dados, administrador, pesquisador, técnico, operador, gestor ou especialista de domínio.

Não escolha um perfil apenas porque “parece combinar” com a tecnologia. Explique **qual objetivo esse perfil teria e qual parte da contribuição do TCC produziria valor para ele**. Se ainda for hipótese, mantenha como hipótese/proto-persona a validar.

Também considere papéis diferentes quando houver tarefas distintas, por exemplo:

- operador que executa análises;
- administrador que configura e gerencia permissões;
- especialista que interpreta resultados;
- gestor que consulta relatórios e decide;
- auditor que revisa histórico.

## Entradas da Entrega 1

Antes de criar personas, retome os tipos de usuários, características relevantes, objetivos e hipóteses registradas na Entrega 1. A persona **não deve transformar uma hipótese inicial em fato por meio de uma história fictícia**.
| Item da Entrega 1 | Status inicial | Evidência disponível agora | Como será tratado nesta entrega |
|---|---|---|---|
| **F01 — O produto deve prever a demanda e recomendar momento e quantidade de reposição.** | F | Objetivo e arquitetura definidos no artigo do TCC. | Incorporar como contribuição técnica central e como objetivo da jornada. |
| **H01 — O usuário prioritário é o proprietário ou responsável pelo estoque de um pequeno comércio digital.** | H | Delimitação do TCC, literatura sobre pequenos negócios e análise de concorrência; sem pesquisa primária. | Representar em P01 como persona de expectativa e validar posteriormente. |
| **H02 — O usuário acumula compra, venda e controle de estoque e dispõe de pouco tempo para análise.** | H | Coerente com o recorte de microempreendedores, mas ainda sem entrevista ou observação. | Incorporar como hipótese que orienta uma experiência curta e priorizada. |
| **H03 — A reposição atual pode depender de intuição, conferência visual, planilha ou dados do marketplace/PDV.** | H | Baselines do TCC simulam estratégias simples; planilha e PDV foram identificados como interfaces familiares. | Manter como hipótese e prever cadastro/importação simples. |
| **H04 — Termos estatísticos e de aprendizado de máquina podem não ser familiares ao usuário.** | H | Diferença identificada entre a linguagem dos concorrentes e a linguagem operacional do público proposto. | Traduzir métricas, explicar recomendações e oferecer detalhes técnicos apenas sob demanda. |
| **H05 — O usuário quer apoio, mas precisa manter o controle da decisão de compra.** | H | Risco financeiro da reposição e padrão de confirmação observado nas soluções analisadas; sem validação direta. | Não automatizar pedidos; permitir revisar, ajustar e confirmar recomendações. |
| **H06 — Alguns negócios contam com outra pessoa para cadastrar vendas e conferir estoque.** | ? | Papel possível no contexto de pequenos negócios, ainda sem confirmação no público real. | Representar em P02 como persona secundária de expectativa e investigar sua ocorrência. |

## 1. Personas

### Persona P01 — Mariana Alves

**Autor(a):** Paulo Andre de Oliveira Hirata — matrícula a inserir  
**Tipo:** primária — persona de expectativa/proto-persona a validar  
**Base de evidências:** delimitação e literatura do TCC; análise de Blue Yonder e Netstock; hipóteses sobre o público; ainda sem entrevista, questionário ou observação  
**Hipóteses da Entrega 1 relacionadas:** H01, H02, H03, H04 e H05  
**Frase-síntese:** “Preciso saber o que comprar sem deixar dinheiro parado nem descobrir a falta quando o cliente já está esperando.”

<img width="1040" height="360" alt="image" src="https://github.com/user-attachments/assets/632327fe-9381-4c97-91fa-4b9940028b5f" />


| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | Senhora de 65 anos, idade fictícia dentro do recorte de 60 a 70 anos. Tem longa vivência no comércio e passou a incluir vendas online com apoio operacional. A baixa familiaridade digital e a rotina dividida entre atendimento e gestão são os fatores que orientam o design. **[H07]** |
| Ocupação/papel | Proprietária de um pequeno comércio que também vende pela internet. Conhece os clientes e fornecedores, define as compras e controla o orçamento. Pode contar com Rafael para registros e tarefas digitais, mas continua responsável pela decisão de reposição. **[H01/H05/H06/H07]** |
| Conhecimento do domínio | Tem experiência prática com produtos, negociação, giro de mercadorias e épocas de maior procura. Reconhece problemas pela observação das prateleiras e pelas anotações. Não costuma expressar esse conhecimento em métricas estatísticas ou relatórios analíticos. **[H03/H04/H07]** |
| Experiência tecnológica | Usa o celular principalmente para ligações, mensagens e áudios. Faz anotações em caderno e utiliza calculadora; tem pouca prática com computador, planilhas, filtros e gráficos. Precisa de orientação no primeiro uso e aprende melhor repetindo um caminho curto com instruções visíveis. **[H03/H04/H07]** |
| Objetivos | Saber o que, quando e quanto comprar; evitar faltar produto ou comprometer o caixa; consultar as recomendações com autonomia crescente; conseguir revisar e confirmar uma lista sem depender de ajuda a cada compra. **[H05/H07/F01]** |
| Necessidades | Orientação inicial passo a passo; poucas opções por vez; nomes de produtos e unidades claros; botões com rótulos como “Ver sugestão” e “Salvar lista”; explicações curtas; ajuda no ponto da dúvida; resumo antes da confirmação e retorno visível após salvar. **[H04/H05/H07]** |
| Dores/frustrações | Faltar mercadoria ou acumular itens parados; não saber por onde começar em um sistema novo; recear apagar registros ou comprar por engano; perder-se em menus e siglas; não entender um gráfico; precisar pedir ajuda para repetir tarefas simples. **[H02/H04/H07]** |
| Motivadores | Manter o negócio organizado, preservar a confiança dos clientes, proteger o dinheiro disponível e sentir que consegue usar a ferramenta sem abrir mão de sua experiência e da decisão final. **[H05/H07]** |
| Restrições/acessibilidade | Pouca familiaridade com navegação e termos digitais, insegurança ao experimentar e interrupções no atendimento. A interface deve ter texto legível, bom contraste e áreas de toque confortáveis. Não há evidência de deficiência visual, motora ou cognitiva específica; essas necessidades serão investigadas. **[H07/?]** |
| Ambiente típico de uso | Balcão ou pequena área administrativa próxima ao estoque, com caderno e calculadora à mão. Usa um celular familiar para consultas simples e pode recorrer ao computador com apoio inicial. Clientes, chamadas e recebimento de mercadorias interrompem a atividade. **[H02/H07]** |
| Comportamentos relevantes | Confere produtos fisicamente, anota vendas e faltas, pede demonstração antes de usar uma função nova e repete caminhos conhecidos. Prefere ler quantidades e frases curtas; consulta ajuda quando não entende e revisa o resultado antes de confirmar. **[H03/H05/H07]** |

**Retrato do cotidiano:** Mariana construiu seu conhecimento do estoque trabalhando com os produtos e conversando com clientes e fornecedores. As vendas online ampliaram sua rotina, mas ela ainda se sente mais segura com o caderno e a calculadora. Quer aprender a consultar o sistema do TCC para planejar a reposição; valoriza uma demonstração inicial e indicações claras do próximo passo. Sua autonomia comercial já está estabelecida, enquanto a autonomia no uso da ferramenta precisa ser construída. **[Narrativa hipotética — H07]**
**Decisões de design influenciadas por P01:**

- **DP01:** iniciar pela lista priorizada de riscos de ruptura e excesso, evitando exigir a revisão de todo o catálogo.
- **DP02:** organizar o fluxo como **risco → explicação → recomendação → decisão**, em vez de expor primeiro métricas técnicas.
- **DP03:** mostrar saldo atual, demanda prevista, horizonte de sete dias, quantidade sugerida e data de atualização próximos uns dos outros.
- **DP04:** explicar termos como estoque de segurança, *fill rate* e confiança da previsão em linguagem cotidiana e sob demanda.
- **DP05:** sinalizar ausência, atraso ou insuficiência dos dados antes de apresentar uma recomendação.
- **DP06:** permitir ajustar e confirmar a quantidade; o sistema não deve efetuar pedidos automaticamente.
- **DP07:** apresentar o impacto esperado da escolha, como risco de falta ou de excesso, sem prometer que a previsão é certa.
- **DP08:** manter poucos filtros operacionais: risco, produto, categoria e período.

### Persona P02 — Rafael Costa

**Autor(a):** Victor Merker Binda — 22.125.075-6 
**Tipo:** secundária — persona de expectativa/proto-persona a validar  
**Base de evidências:** tarefas previstas no módulo de cadastro operacional e hipótese de divisão de trabalho no pequeno negócio; ainda sem validação da existência ou frequência desse papel  
**Hipóteses da Entrega 1 relacionadas:** H03, H04 e H06  
**Frase-síntese:** “Se eu registrar tudo corretamente agora, a decisão de compra não será baseada em um saldo desatualizado depois.”

<img width="1040" height="360" alt="image" src="https://github.com/user-attachments/assets/5f2ec3ad-281d-4e3e-a5ee-0dfc2dbbb516" />

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | Adulto jovem, entre 20 e 35 anos, colaborador de uma operação pequena. O fator relevante é executar várias tarefas operacionais sob interrupção, não sua idade. **[H]** |
| Ocupação/papel | Auxiliar operacional ou administrativo. Registra produtos e vendas, confere estoque físico, corrige divergências e comunica itens críticos à proprietária. Não assume sozinho a decisão financeira de compra. **[H/?]** |
| Conhecimento do domínio | Conhece códigos, nomes, variações dos produtos e a rotina de entrada e saída. Pode conhecer menos sobre contratos, caixa e critérios de reposição definidos pela proprietária. **[H]** |
| Experiência tecnológica | Tem familiaridade com formulários, busca, marketplace e planilhas. Aprende fluxos operacionais com rapidez, mas não precisa conhecer o funcionamento do modelo preditivo. **[H]** |
| Objetivos | Registrar dados sem retrabalho; localizar produtos rapidamente; corrigir erros; terminar a conferência do estoque; informar situações críticas com dados confiáveis. **[H]** |
| Necessidades | Busca sempre visível; cadastro curto; importação de planilha quando disponível; validação de campos; mensagens de erro que indiquem como corrigir; confirmação de salvamento; histórico de alterações e permissões adequadas ao papel. **[H]** |
| Dores/frustrações | Digitação repetitiva, produtos duplicados, códigos inconsistentes, tela que perde dados após interrupção, erro informado somente no final e dúvida sobre se uma venda alterou o saldo. **[H]** |
| Motivadores | Manter a operação organizada, evitar cobranças por divergência de estoque e fornecer uma base confiável para a proprietária decidir. **[H]** |
| Restrições/acessibilidade | Pode usar computador compartilhado, realizar a tarefa em blocos curtos e sofrer interrupções por separação de pedidos ou atendimento. Necessidades específicas de acessibilidade ainda são desconhecidas. **[H/?]** |
| Ambiente típico de uso | Bancada administrativa ou área próxima ao armazenamento de produtos, com alternância entre contagem física, embalagem, computador e comunicação por celular. **[H]** |
| Comportamentos relevantes | Pesquisa pelo nome ou código, registra atividades em sequência, deixa uma tarefa incompleta quando surge um pedido urgente e precisa retomar do ponto anterior. Confere totais antes de encerrar. **[H]** |

**Decisões de design influenciadas por P02:**

- **DP09:** oferecer busca por nome, código e categoria e reduzir campos obrigatórios ao mínimo necessário.
- **DP10:** validar formato, duplicidade e consistência durante o preenchimento, mostrando como corrigir o problema.
- **DP11:** confirmar salvamento e atualização do saldo, além de permitir corrigir um registro sem recriar toda a operação.
- **DP12:** preservar rascunhos ou estado do formulário quando houver interrupção.
- **DP13:** separar permissões de cadastro das permissões de confirmação de reposição.
- **DP14:** registrar autor, data e alteração para que divergências possam ser rastreadas.
- **DP15:** permitir importação simples de arquivo, mas manter cadastro manual para negócios sem ERP ou integração com marketplace.

### Síntese das personas

P01 e P02 compartilham a necessidade de uma interface clara, porém não são duplicadas. **Mariana (P01)** usa a informação para assumir uma decisão financeira: precisa comparar risco, previsão e quantidade sugerida antes de confirmar a compra. **Rafael (P02)** produz e corrige os dados que sustentam essa análise: precisa de velocidade, prevenção de erros, retomada e rastreabilidade.

A persona prioritária é **P01**, porque o objetivo central do TCC é apoiar a decisão de reposição do microempreendedor. P02 é secundária e somente deverá permanecer no projeto se a existência desse papel for confirmada no público pesquisado. Mesmo sendo secundária, sua experiência afeta diretamente a qualidade da previsão: dados incompletos ou incorretos podem gerar recomendações inadequadas.

## 2. Mapa de empatia — equipe

**Persona escolhida:** P01 — Mariana Alves  
**Justificativa:** é a principal beneficiária da contribuição do TCC, toma a decisão de compra e sofre diretamente os efeitos de ruptura, excesso e capital imobilizado. O mapa aprofunda sua relação cotidiana com o problema, mas continua sendo hipotético até a validação com pessoas reais.

<img width="3600" height="2780" alt="image" src="https://github.com/user-attachments/assets/851d7c11-ffb8-41fd-9166-827cb163319d" />

| Dimensão | Descrição | Natureza da informação | Consequência para o design |
|---|---|---|---|
| O que vê | Pedidos chegando pelo marketplace, produtos com ritmos diferentes de venda, espaço limitado, preços de fornecedores e saldo distribuído entre registros. | Hipótese H02/H03. | Consolidar os itens prioritários e permitir aprofundar apenas quando necessário. |
| O que ouve | Clientes perguntando se ainda há produto, fornecedores informando prazo ou reajuste e colaboradores alertando sobre divergências. | Hipótese H02/H06. | Mostrar urgência, prazo e responsável pela última atualização sem criar alarmes genéricos. |
| O que diz e faz | “Esse produto costuma vender mais nesta época”; confere saldo, consulta vendas, calcula mentalmente ou em planilha e negocia o pedido. | Hipótese H03. | Permitir comparar a recomendação com histórico e ajustar a quantidade antes da decisão. |
| O que pensa e sente | Receio de perder uma venda por falta e, ao mesmo tempo, de comprometer o caixa com mercadoria parada; desconfia de números sem explicação. | Problema do domínio documentado; reação emocional ainda hipotética. | Explicar motivo, incerteza, período e dados utilizados; evitar apresentar previsão como certeza. |
| Dores | Falta descoberta tarde, compra emergencial, excesso, capital imobilizado, dados dispersos, conferência demorada e recomendação pouco transparente. | Ruptura e excesso são fatos do domínio; vivência e intensidade devem ser validadas. | Priorizar exceções, validar dados e encurtar o caminho entre alerta e ação. |
| Ganhos/necessidades | Saber onde agir primeiro, entender a sugestão, decidir com antecedência, manter o controle e verificar depois se a decisão teve bom resultado. | Hipótese de valor do produto. | Oferecer ranking de risco, lista sugerida revisável, explicação e acompanhamento posterior. |

## 3. Contexto de uso — consolidação

| Dimensão | Descrição | Implicação de design |
|---|---|---|
| Usuários | P01, proprietária e decisora da reposição; P02, possível auxiliar responsável por cadastros e conferências. Ambos são personas de expectativa. | Priorizar P01 no painel decisório e disponibilizar a P02 um fluxo operacional com permissões específicas. |
| Tarefas | Registrar ou importar produtos e vendas; conferir saldo; identificar ruptura/excesso; examinar previsão; revisar quantidade sugerida; confirmar decisão; registrar chegada da reposição e acompanhar resultado. | Conectar dados, análise e ação em um fluxo rastreável e permitir retomada após interrupções. |
| Equipamentos | Computador ou notebook para análise e cadastro; celular usado paralelamente para marketplace, mensagens e contato com fornecedor; possível planilha/CSV como fonte inicial. **[H]** | Criar aplicação web responsiva, interação por teclado, importação simples e informações essenciais legíveis sem telas excessivamente densas. |
| Ambiente físico | Casa, escritório pequeno ou área administrativa junto ao estoque, com ruído, circulação, separação de pedidos e interrupções. **[H]** | Salvar progresso, confirmar ações, manter o estado da análise e evitar tarefas longas sem retorno intermediário. |
| Ambiente social/organizacional | A proprietária alterna atendimento, operação e gestão; pode receber informações de colaborador, cliente e fornecedor. A urgência aumenta em períodos promocionais. **[H]** | Indicar responsável e data dos dados, permitir compartilhamento/exportação da lista e destacar prazos sem excesso de notificações. |
| Papéis/permissões/governança | P01 pode cadastrar, analisar, ajustar e confirmar a reposição. P02 pode cadastrar e corrigir registros, mas a confirmação financeira permanece com P01. **[H]** | Implementar controle de acesso simples, histórico de alterações e confirmação explícita para decisões de compra. |
| Volume de dados/histórico | Catálogo com diversos produtos, ritmos de venda diferentes e possibilidade de itens com menos de 30 dias ou histórico esparso. O modelo usa histórico temporal e prevê os próximos sete dias. | Priorizar por exceção, permitir busca/filtros, informar insuficiência do histórico e não ocultar a maior incerteza dos itens novos ou irregulares. |

### Narrativa consolidada do contexto

No início ou no final de um período de trabalho, Mariana reserva alguns minutos entre o atendimento de pedidos e o contato com fornecedores para planejar o estoque. Ela pode estar em casa ou em um pequeno espaço administrativo próximo às mercadorias. Enquanto analisa os dados no computador, recebe notificações do marketplace e mensagens no celular. Se houver um auxiliar, parte dos registros pode ter sido inserida por ele, de modo que Mariana precisa saber quando os dados foram atualizados e se existem inconsistências.

O sistema do TCC deve caber nesse cotidiano fragmentado. Mariana não inicia a atividade com o objetivo abstrato de “usar inteligência artificial”; ela chega ao produto porque precisa evitar uma falta, decidir um pedido antes do prazo do fornecedor ou impedir uma compra excessiva. A aplicação organiza o histórico, indica os produtos com maior risco e apresenta uma quantidade sugerida. Mariana confronta a informação com seu conhecimento sobre promoções, fornecedor e caixa, ajusta se necessário e confirma sua decisão. Depois, ela registra ou acompanha a chegada dos itens e verifica se o produto permaneceu disponível sem gerar excesso. Toda essa narrativa é uma hipótese de contexto a ser validada.

## 4. Jornada do usuário — equipe

**Persona:** P01 — Mariana Alves  
**Objetivo da jornada:** decidir, dentro da rotina do pequeno comércio digital, quais produtos devem ser repostos, em que momento e em qual quantidade, mantendo o controle financeiro e entendendo as limitações da recomendação.  
**Início e fim da jornada:** começa **antes do uso**, quando vendas, mensagens de clientes ou o prazo do fornecedor despertam a preocupação com falta ou excesso; termina **depois do uso**, quando Mariana acompanha a chegada e as vendas posteriores para avaliar o resultado da decisão.

| Etapa | Situação/ação | Objetivo | Pensamento/emoção | Dor | Oportunidade de design | Evidência |
|---|---|---|---|---|---|---|
| 1 — Rotina anterior ao uso | Durante o dia, Mariana atende pedidos, acompanha mensagens e percebe que alguns produtos saem mais rápido do que outros. Nem sempre consegue analisar o catálogo naquele momento. | Manter a operação funcionando e reconhecer sinais de que será necessário planejar uma compra. | “Depois preciso conferir se isso ainda dura até a próxima entrega.” Atenção dividida e leve preocupação. | O sinal de risco aparece disperso entre vendas, memória, planilha e contagem física. | Consolidar dados ao longo da rotina e apresentar pendências quando ela tiver tempo de decidir. | **H02/H03 — hipótese a validar.** |
| 2 — Motivação e gatilho | Um cliente procura um item quase esgotado, aproxima-se o dia habitual de pedido ou o fornecedor informa um prazo. Mariana decide revisar o estoque. | Evitar descobrir a falta somente quando já não houver tempo para repor. | “Se eu pedir pouco, posso perder vendas; se pedir demais, comprometo o caixa.” Ansiedade e senso de urgência. | Conflito entre disponibilidade e capital imobilizado; decisão baseada em informação incompleta. | Alertar com antecedência, indicar prazo e separar risco de ruptura de risco de excesso. | Ruptura e excesso são **fatos do domínio**; gatilhos e emoção são **H**. |
| 3 — Preparação dos dados | Antes da análise, Mariana ou Rafael verifica se vendas, saldo e prazos estão registrados; quando necessário, importa uma planilha ou corrige uma divergência. | Garantir que a recomendação seja calculada sobre dados recentes e coerentes. | “Posso confiar nessa análise ou ficou alguma venda de fora?” Cautela. | Dados espalhados, digitação repetitiva, histórico curto e dúvida sobre a atualização. | Exibir data da última atualização, validar dados, mostrar pendências e permitir importação/correção simples. | **F01/H03/H06.** |
| 4 — Visão geral no produto do TCC | Mariana abre o painel e encontra os produtos ordenados por risco, com destaque para ruptura, excesso e histórico insuficiente. | Saber onde precisa concentrar atenção sem conferir todos os itens. | “Quais produtos realmente exigem uma ação hoje?” Busca por rapidez e alívio ao ver prioridades claras. | Painéis densos ou alertas sem prioridade aumentam a carga de trabalho. | Aplicar gestão por exceção, poucos indicadores e filtros por risco, produto, categoria e período. | Requisito derivado do escopo do TCC e da análise de Blue Yonder/Netstock; utilidade para P01 ainda é **H**. |
| 5 — Compreensão da recomendação | Ela seleciona um produto crítico e compara saldo, vendas recentes, previsão para sete dias, prazo de reposição e quantidade sugerida. Consulta a explicação da recomendação. | Entender por que o item foi priorizado e verificar se a sugestão faz sentido. | “Esse aumento combina com o que estou vendo nas vendas?” Curiosidade, mas possível desconfiança. | Termos técnicos, gráfico sem contexto e previsão apresentada como certeza. | Usar unidades e linguagem comercial, comparar realizado e previsto, explicar fatores e sinalizar incerteza ou pouco histórico. | **F01/H04.** |
| 6 — Decisão e ação | Mariana considera promoção, caixa e informação do fornecedor, ajusta a quantidade quando necessário, confirma a decisão e usa a lista para negociar ou fazer o pedido. | Realizar uma compra consciente sem entregar a decisão integralmente ao algoritmo. | “A sugestão ajuda, mas a decisão final precisa considerar o que sei do negócio.” Maior segurança quando mantém o controle. | Recomendação automática pode ignorar eventos que ainda não estão nos dados; um erro gera custo real. | Permitir editar, justificar e confirmar; nunca enviar pedido automaticamente; deixar claro o impacto provável da alteração. | **H05 — hipótese a validar; confirmação humana é decisão de design.** |
| 7 — Continuidade da rotina | Após decidir, Mariana volta a atender clientes. A lista fica salva, com produtos, quantidades, responsável e estado do pedido, para consulta posterior. | Não perder o trabalho realizado e acompanhar o que ainda está pendente. | “Preciso voltar ao atendimento sem esquecer o que combinei.” Sensação de organização. | Interrupções e informações mantidas apenas em mensagens ou memória. | Salvar estado, registrar histórico e permitir exportar ou compartilhar uma lista curta com fornecedor/colaborador. | **H02/H06.** |
| 8 — Resultado posterior | Quando os itens chegam, a entrada é registrada. Nos dias seguintes, Mariana acompanha se houve ruptura, se sobrou estoque e como o previsto se comparou às vendas reais. | Avaliar se a decisão ajudou e melhorar as próximas reposições. | “Funcionou melhor do que minha estimativa anterior? Em quais produtos ainda preciso ter cuidado?” Confiança gradual, não automática. | Sem retorno posterior, a recomendação parece uma caixa-preta e erros podem se repetir. | Mostrar resultado da decisão, diferença entre previsto e realizado, dias em ruptura e possíveis excessos; manter o histórico por produto. | Métricas são parte do **escopo do TCC**; redução efetiva de ruptura/excesso é **resultado esperado, ainda não comprovado**. |

> A jornada descreve a atividade cotidiana completa e não uma sequência de telas. O produto do TCC aparece como apoio no centro da jornada; a motivação surge antes da abertura do sistema e o resultado somente pode ser avaliado depois da decisão e da reposição.

## Síntese

Os cenários e tarefas seguintes deverão preservar obrigatoriamente:

- o objetivo de identificar **o que, quando e quanto repor**;
- a motivação anterior ao uso, ligada a risco de falta, excesso, prazo do fornecedor e limitação de caixa;
- a priorização de poucos produtos críticos, sem obrigar a revisão de todo o catálogo;
- a verificação da qualidade, suficiência e data de atualização dos dados;
- a explicação da previsão em linguagem operacional, sem apresentar o modelo como infalível;
- a comparação entre saldo, histórico, demanda prevista e quantidade recomendada;
- a revisão e confirmação humana antes de transformar a recomendação em compra;
- a retomada após interrupções e a rastreabilidade de cadastros e decisões;
- o acompanhamento posterior do resultado, comparando previsto e realizado e observando ruptura e excesso;
- a validação futura de P01, P02, mapa de empatia, contexto e jornada com microempreendedores reais.
## Checklist

- [ ] Existe pelo menos uma persona por integrante.
- [ ] As personas não são apenas diferenças demográficas superficiais.
- [ ] Está claro o que é dado real e o que é hipótese/proto-persona.
- [ ] A persona não “validou por ficção” uma hipótese da Entrega 1; afirmações continuam marcadas como hipótese quando não há evidência.
- [ ] Objetivos e dores têm consequência para o design.
- [ ] Contexto de uso está coerente com a Entrega 1.
- [ ] Em TCC sem interface original, a persona possui relação explícita com a contribuição técnica.
- [ ] Papéis administrativos, técnicos e decisórios só foram criados quando possuem objetivos/tarefas diferentes.
- [ ] Jornada possui etapas, dores e oportunidades e não é apenas wireflow.
- [ ] IDs das personas foram adicionados à rastreabilidade.
