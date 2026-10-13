# Entrega 1 — Conhecendo o projeto, o usuário e o problema

**Data original:** 19/08/2026  
**Revisão:** 13/10/2026 — correções após feedback do professor  
**Status:** 🟦 revisada após feedback
**Responsabilidade:** uma solução consolidada por equipe

Usamos **[F]** para fatos com origem indicada, **[H]** para hipóteses e **[?]** para lacunas. Uma decisão de recorte da equipe não comprova uma necessidade do público. As hipóteses são referenciadas por descrições; sua evolução está na [matriz de rastreabilidade](../RASTREABILIDADE.md). A revisão não utiliza evidências posteriores para afirmar que já eram conhecidas na data original.

## 0. Identificação do TCC e da equipe

### 0.1 Membros

| Nome completo | Matrícula | GitHub |
|---|---|---|
| Paulo Andre de Oliveira Hirata | 22.125.072-3 | @poulison |
| Victor Merker Binda | 22.125.075-6 | @victorrbb |

### 0.2 Título registrado nesta entrega

**Previsão de estoque usando machine learning.** Origem: identificação do projeto no [README](../README.md). A formulação ampliada utilizada posteriormente não comprova, por si só, ampliação do compromisso formal do TCC.

### 0.3 Orientador

**Fagner de Assis Moura Pimentel**, conforme identificação da equipe no README.

### 0.4 Resultado principal previsto

- [x] Sistema/aplicação interativa.
- [x] Modelo de IA/ML.
- [x] Estudo comparativo/avaliação experimental.

[F] A proposta registrada pela equipe é analisar o histórico de movimentações, prever demanda e comparar modelos. Isso descreve o resultado pretendido, não uma implementação ou desempenho já demonstrados. Origem: README e versão original desta entrega.

### 0.5 O TCC já previa interface?

[F] Sim, segundo o registro da equipe no README. [?] Fluxos obrigatórios, tecnologias, dados disponíveis e eventual cálculo de recomendação de reposição ainda precisam ser confirmados com o orientador.

## 1. Entendendo a contribuição do projeto

### 1.1 TCC em uma frase

O TCC busca prever demanda usando o histórico de movimentações e comparar modelos; a aplicação investigada em IHC é apoiar o planejamento de reposições em pequenos comércios.

### 1.2 Problema que motivou o TCC

[F] A equipe relata que um integrante observou ruptura de estoque na loja de sua família. A origem disponível é esse relato de observação direta, registrado na entrega; não foram fornecidos diário de campo, datas, frequência ou registros de vendas que permitam caracterizar a ocorrência em detalhe.

### 1.3 Contribuição central

[F] Construir e comparar previsões de demanda faz parte da proposta documentada. [?] A qualidade dessas previsões e sua utilidade em decisões reais ainda dependem de avaliação.

### 1.4 Mudança esperada

[H] **Benefício das previsões:** consultar previsões pode ajudar a antecipar reposições e reduzir faltas e excessos.  
[H] **Compreensão dos resultados:** uma apresentação adequada pode permitir que gestores sem formação em ML interpretem as estimativas.

### 1.5 Mérito técnico e aplicação

| Contribuição técnica prevista | Aplicação prática possível | Limite atual |
|---|---|---|
| Construir e comparar modelos de previsão | [H] Apoiar o planejamento de compras | Melhor desempenho preditivo não demonstra sozinho melhor decisão comercial |
| Avaliar erros das previsões | [H] Informar limites das estimativas utilizadas | Vocabulário e informação úteis ao usuário precisam ser investigados |

## 2. Pessoas envolvidas

### 2.1 Usuário direto

[H] O responsável pelo estoque de um pequeno comércio é o perfil prioritário provisório. É preciso verificar quem consulta dados, propõe compras e autoriza gastos, e se essas funções são exercidas pela mesma pessoa.

### 2.2 Perfis e responsabilidades

| Perfil proposto | O que faria | Relação com a contribuição do TCC | Status/evidência |
|---|---|---|---|
| Responsável pelo estoque | Conferir disponibilidade e consultar previsões | Usaria a estimativa como uma informação para planejar reposições | [H] Escolha inicial da equipe; sem pesquisa de campo |
| Proprietário/gerente | Considerar caixa e aprovar compras | Confrontaria a estimativa com restrições comerciais | [H] Divisão de responsabilidades não confirmada |
| Funcionário de vendas/apoio operacional | Registrar movimentações e comunicar divergências | Poderia produzir ou conferir dados utilizados pela previsão | [H] Existência de papel separado não confirmada |
| Equipe do TCC | Desenvolver e avaliar modelos | Produz a contribuição técnica e compara resultados | [F] Responsabilidade registrada pela equipe; não representa o usuário comercial |

### 2.3 Pessoas afetadas sem uso direto necessariamente previsto

| Stakeholder | Como pode ser afetado | Uso da interface | Status/evidência |
|---|---|---|---|
| Clientes | Indisponibilidade pode impedir uma compra | Não previsto no recorte | [F] Há relato de ruptura; [H] impacto específico no atendimento não medido |
| Fornecedores | Recebem decisões de pedido do comércio | Não previsto no recorte | [H] Relação comercial presumida; canais e condições a investigar |
| Funcionários | Podem lidar com faltas, separação e divergências | [?] Depende das responsabilidades reais | [H] Perfil possível; sem observação do papel |

### 2.4 Características relevantes

[H] O usuário pode conhecer produtos e fornecedores sem dominar métricas de ML. A linguagem comercial e a explicação de incerteza são propostas a avaliar, não preferências já comprovadas.

## 3. Objetivos e atividades

### 3.1 Objetivo do usuário

[H] Evitar falta de produtos sem comprar além do necessário ou comprometer recursos de outras despesas.

### 3.2 Atividades importantes

| ID | Atividade candidata | Quem poderia realizar | Frequência/criticidade propostas | Status |
|---|---|---|---|---|
| A01 | Acompanhar disponibilidade do estoque | Responsável ou auxiliar | Frequente/alta | [H] Periodicidade e procedimento a investigar |
| A02 | Identificar risco de falta ou excesso | Responsável | Frequente/alta | [H] Critérios atuais desconhecidos |
| A03 | Planejar reposições | Responsável/proprietário | Periódica/crítica | [H] Responsabilidades e restrições a investigar |
| A04 | Interpretar uma previsão antes de decidir | Possível usuário da solução | Ligada ao ciclo de compra/crítica | [H] Atividade futura candidata, não observada na rotina atual |

### 3.3 Atividade mais frequente

[H] Acompanhar o estoque pode ser frequente por causa de entradas, saídas e ajustes. [?] A frequência relativa das atividades ainda não foi medida.

### 3.4 Atividade mais crítica

[H] Planejar reposições é potencialmente crítico por envolver risco de falta e imobilização de dinheiro. Essa prioridade precisa ser confrontada com o trabalho real.

## 4. Problema e processo atual

### 4.1 O que sabemos e o que falta conhecer

[F] A versão original registra observação de contagem manual pela equipe. Esse registro sustenta apenas a existência dessa prática em uma situação relatada, sem caracterizar todo o processo.

| Aspecto do processo | Conhecimento atual | Pergunta de investigação |
|---|---|---|
| Contagem física | [F] Relatada pela equipe, sem protocolo anexado | [?] Quem conta, quando e por qual motivo? |
| Entradas e saídas | [?] Forma de registro desconhecida | Como são registradas vendas, recebimentos, reservas, cancelamentos e devoluções? |
| Decisão de compra | [?] Responsável e gatilho desconhecidos | Quem percebe a necessidade, define quantidade e autoriza a compra? |
| Recursos utilizados | [?] Não foi confirmado uso de caderno, planilha, PDV ou mensagens | Quais ferramentas existem e como seus registros se relacionam? |
| Critérios comerciais | [?] Não documentados | Como entram prazo do fornecedor, sazonalidade, promoção, caixa, lote mínimo e estoque mínimo? |
| Divergências | [?] Procedimento desconhecido | Como a diferença entre registro e contagem é investigada e corrigida? |
| Histórico disponível | [?] Cobertura e qualidade desconhecidas | Há identificação de produto, data, quantidade e situação da movimentação? |

### 4.2 Principais dificuldades propostas

[H] Consolidar registros e perceber tendências pode exigir esforço ou produzir erros. O caráter manual da atividade não demonstra ineficiência: é necessário localizar atrasos, ambiguidades, duplicidades ou retrabalho em casos reais.

### 4.3 Informações potencialmente necessárias

[H] Saldo disponível, movimentações anteriores, entradas previstas, prazo do fornecedor, estimativa de demanda, política de estoque e restrições de caixa podem participar da decisão. [?] Disponibilidade, confiabilidade e necessidade de cada informação ainda serão investigadas.

### 4.4 Consequências possíveis de erro

[H] Uma estimativa baixa pode contribuir para falta e perda de vendas; uma alta pode contribuir para excesso. Também é possível interpretar a previsão como certeza, ignorar sua atualização ou confundir estimativa de demanda com quantidade de compra. Essas são situações a investigar, não resultados medidos.

### 4.5 Situação concreta e seus limites

[F] Segundo o relato da equipe, houve ruptura na loja da família de um integrante. [?] A causa, duração, frequência e desfecho de atendimento não foram documentados. [H] Um cliente nessa situação poderia escolher outro produto ou sair sem comprar; esse desfecho ilustrativo não é apresentado como observação comprovada.

### 4.6 Evidências atuais

| Fonte identificada | Natureza | O que sustenta | Limitação |
|---|---|---|---|
| Versão original, seções 1.2 e 4.5 | Relato da equipe sobre observação de integrante | Existência relatada de ruptura | Sem registro detalhado; não estabelece causa nem frequência |
| Versão original, seção 4.1 | Relato da equipe sobre contagem manual | Existência relatada da prática | Sem descrição de responsáveis, sequência e periodicidade |
| README, relação entre TCC e IHC | Registro documental da equipe | Proposta de sistema, previsão e comparação de modelos | Não comprova implementação nem aprovação de todas as funções pelo orientador |

Artigos genéricos sem referência identificável não são utilizados como evidência específica da loja nesta revisão. Não houve nova entrevista ou observação para corrigir o documento.

## 5. Contexto de uso

### 5.1 Onde e quando?

[H] A consulta pode ocorrer no comércio, durante conferências ou planejamento de pedidos. [?] Local, momento e duração reais de uso precisam ser investigados.

### 5.2 Dispositivos

[H] Computador/notebook para registro e celular para consultas são possibilidades. [?] Equipamentos disponíveis e familiaridade do público não foram verificados.

### 5.3 Condições físicas

[H] Ruído, interrupções e pressão de tempo podem afetar a atividade; sua ocorrência e intensidade ainda são desconhecidas.

### 5.4 Fatores organizacionais

[H] Registro de movimentações e aprovação de compras podem ser distribuídos entre pessoas ou concentrados no proprietário. [?] A divisão real deve preceder a definição de permissões.

### 5.5 Histórico e rastreabilidade

[H] O usuário pode precisar consultar previsões anteriores e confrontá-las com o realizado. É preciso distinguir uma necessidade do usuário de uma informação necessária apenas à avaliação experimental do TCC.

### 5.6 Consequências de erro

[H] Dados incorretos ou interpretação equivocada podem prejudicar a decisão. [?] Como o usuário reconhece incerteza, verifica fontes e decide quando não confiar na estimativa?

## 6. Mercado e alternativas

### 6.1 Levantamento inicial

| Alternativa | Quem utiliza ou utilizaria | Uso possível | Status/evidência nesta etapa |
|---|---|---|---|
| Contagem física manual | Pessoa que conferiu o estoque; papel específico não registrado | Apurar unidades presentes | [F] Relato da equipe; sequência e abrangência desconhecidas |
| Planilha ou anotações | [H] Responsável ou auxiliar | Registrar e conferir movimentações | [H] Uso na loja não confirmado |
| Experiência do responsável | [H] Pessoa que decide compras | Estimar procura e definir pedido | [H] Critérios e importância não investigados |
| Sistema de vendas/PDV | [?] Usuário e existência do sistema desconhecidos | Possível fonte de vendas e saldos | [?] Alternativa a investigar; não é prática atribuída à loja |

### 6.2 Produtos a investigar

Blue Yonder e Netstock foram citados inicialmente pela equipe como candidatos à análise. [?] A versão original não identificava as fontes consultadas nessa etapa. Sua caracterização e as evidências de mercado ficam na [Entrega 2](02_analise_concorrencia.md), com as respectivas datas, sem validação retroativa da Entrega 1.

### 6.3 Interfaces possivelmente conhecidas

[H] Planilhas, sistemas de vendas e aplicativos de mensagens podem fazer parte da rotina. [?] É necessário verificar quais são usados e por quem. A existência dessas interfaces no mercado não comprova familiaridade do público.

### 6.4 Pontos positivos a investigar

[H] Organização de saldos, movimentações e avisos pode facilitar consultas. Nesta etapa não há evidência visual identificada suficiente para atribuir esse benefício a um concorrente específico ou ao público do projeto.

### 6.5 Limitações a investigar

[H] Amplitude funcional e configuração complexa podem dificultar o uso por pequenos negócios. Custo, esforço e compreensão precisam de evidência própria.

### 6.6 Padrões familiares a investigar

[H] Busca, tabelas, filtros e avisos de estoque são candidatos. Sua adoção dependerá de familiaridade e tarefa, e não apenas de presença em produtos concorrentes.

## 7. Escopo de IHC

### 7.1 Caminho escolhido

**Caminho A — a equipe registra que o TCC já prevê interface.** O recorte proposto é consultar informações de estoque, interpretar previsões e apoiar o planejamento de reposição. ERP completo permanece fora do escopo.

### 7.2 Perfil priorizado

[H] Responsável pelo estoque de pequeno comércio, provisoriamente escolhido por sua possível relação com a decisão de compra. A investigação deverá confirmar ou rever essa escolha.

### 7.3 Objetivo priorizado e limite técnico

[H] O objetivo de negócio é decidir o que, quanto e quando repor. A interface proposta pretende **apoiar essa decisão com previsões compreensíveis e informações disponíveis**. Previsão de demanda não equivale, por si só, a recomendação de compra.

[?] Calcular quantidade ou momento recomendado pode exigir prazo de entrega, saldo disponível, pedidos em trânsito, política de estoque, lote mínimo e restrições financeiras. A inclusão dessa capacidade permanece pendente de confirmação com o orientador; não é atribuída automaticamente ao modelo de ML.

### 7.4 Interface explorada

> Para a disciplina, propõe-se uma interface que ajude um possível responsável pelo estoque a interpretar previsões de demanda e confrontá-las com informações comerciais para planejar reposições. Público, dados e fluxos serão refinados pela investigação.

### 7.5 Relação com o TCC

A interface é prevista no registro da equipe, e IHC aprofunda seu uso. A incorporação dos detalhes ao TCC depende da equipe e do orientador; o protótipo acadêmico não amplia automaticamente o escopo formal.

## 8. Possibilidades de interação

| Possibilidade | Avaliação inicial | Objetivo/tarefa que justificaria | Evidência atual e dependência |
|---|---|---|---|
| Visão geral/alertas | Candidata | Identificar itens que exigem atenção | [H] Benefício das previsões; risco e critérios ainda não validados |
| Entrada/importação de dados | Candidata | Fornecer dados para análise | [F] A proposta depende de histórico; [?] origem e formato disponíveis |
| Consulta da previsão | Candidata central | Interpretar estimativa antes de decidir | [F] Previsão integra a proposta; [H] forma de consulta útil ao usuário |
| Histórico e filtros | Candidata | Localizar registros e comparar períodos | [H] Necessidade de histórico; depende de volume e prática real |
| Explicação do resultado | Candidata | Compreender incerteza e limites | [H] Compreensão e vocabulário do público |
| Cadastro de produtos | Condicional | Identificar produtos e dados essenciais | [?] Depende das fontes já existentes |
| Usuários/permissões | Condicional | Respeitar responsabilidades distintas | [?] Divisão do trabalho não confirmada |
| Administração completa | Fora do recorte | Não há tarefa justificadora nesta etapa | Decisão de escopo da equipe |

## 9. Benefícios e ações iniciais

### 9.1 Benefícios esperados

| Benefício possível | Necessidade proposta | Possível beneficiário | Status |
|---|---|---|---|
| Antecipar rupturas | Planejar disponibilidade | Responsável pela compra | [H] Não medido |
| Facilitar interpretação do histórico | Reunir informação para decidir | Responsável/auxiliar | [H] Esforço atual não medido |
| Compreender previsões | Avaliar estimativa sem formação em ML | Responsável pela decisão | [H] A validar com usuários |

### 9.2 Ações candidatas

As prioridades abaixo são **provisórias de investigação/prototipação**, não requisitos confirmados ou compromissos de implementação.

| ID | O usuário poderia precisar conseguir... | Para alcançar... | Prioridade provisória | Sustentação/dependência |
|---|---|---|---|---|
| F01 | Identificar itens com possível risco | Direcionar a análise da reposição | Alta | [H] Benefício das previsões; critérios de risco a definir |
| F02 | Consultar saldo, histórico e estimativa | Confrontar informações antes de decidir | Alta | [H] Compreensão; [?] disponibilidade dos dados |
| F03 | Buscar e filtrar produtos | Localizar o item necessário | A definir | [?] Volume do catálogo e estratégia de busca |
| F04 | Revisar dados, atualização e limitações | Evitar interpretação indevida | Alta | [H] Vocabulário e percepção de incerteza |
| F05 | Registrar uma decisão de reposição | Recuperar o que decidiu e acompanhar o resultado | A definir | [?] Forma atual de registro e limite do TCC |
| F06 | Comparar previsto e realizado | Avaliar a utilidade da estimativa | A definir | [H] Necessidade comercial de histórico; distinta da avaliação dos modelos |

### 9.3 Tecnologias e restrições

| Item previsto | Motivo | Implicação proposta |
|---|---|---|
| Aprendizado de máquina | Parte da contribuição técnica | Explicar estimativa e limites, sem prometer certeza |
| Histórico temporal | Entrada da previsão | Investigar qualidade, suficiência e atualização |
| Comparação de modelos | Avaliação técnica | Não exigir que o comerciante escolha algoritmos ou interprete métricas técnicas |
| Dados/regras de reposição | Capacidade adicional ainda não confirmada | Não apresentar previsão como quantidade automaticamente recomendada |

## 10. Hipóteses e dúvidas prioritárias

| Hipótese/dúvida | Tipo | Por que importa | Como investigar |
|---|---|---|---|
| Benefício das previsões para antecipar reposições | [H] | Sustenta o valor de uso | Entrevista e teste de conceito; avaliar decisões e resultados |
| Compreensão dos resultados por gestores sem formação em ML | [H] | Orienta apresentação e explicação | Teste de interpretação com participantes reais |
| Responsável pelo estoque como usuário prioritário | [H] | Define quem participará do projeto e da avaliação | Entrevistar e observar papéis; persona organiza hipóteses, não as valida |
| Conhecimento comercial sem domínio de métricas de ML | [H] | Orienta vocabulário | Investigar termos, exemplos e interpretações |
| Esforço e falhas na consolidação manual | [H] | Pode justificar apoio ao processo | Observar casos, interrupções, retrabalho e correções |
| Necessidade de histórico de previsões | [H] | Pode justificar consulta posterior | Investigar decisões reais e necessidade de comparação |
| Processo e dados atuais | [?] | Define viabilidade e entrada de dados | Examinar registros autorizados, ferramentas, responsáveis e periodicidade |
| Escopo formal do TCC | [?] | Evita prometer cálculo de reposição sem suporte | Confirmar fluxos, dados, horizonte e regras com o orientador |
| Percepção de incerteza e confiança na previsão | [?] | Evita decisão apoiada em falsa certeza | Pedir interpretação de exemplos e critérios para aceitar ou rejeitar estimativas |

Origem, evolução e impacto são preservados por descrição na [matriz](../RASTREABILIDADE.md).

## 11. Síntese da equipe

| Pergunta | Resposta atual |
|---|---|
| Contribuição do TCC | [F] Proposta registrada de prever demanda e comparar modelos |
| O TCC previa interface? | [F] Sim, conforme registro da equipe no README |
| Usuário prioritário | [H] Responsável pelo estoque de pequeno comércio |
| Objetivo | [H] Evitar falta e excesso ao planejar reposições |
| Processo atual | [F] Há relato de contagem manual e ruptura; [?] processo completo desconhecido |
| Contexto | [H] Conferência e planejamento de compras na rotina do comércio |
| Recorte de IHC | Proposta: informação de estoque → interpretação da previsão → apoio à decisão |
| Recomendação automática de quantidade/momento | [?] Não confirmada no escopo formal |

**Dentro do recorte proposto:** consulta, interpretação e apoio ao planejamento.  
**Fora do escopo:** ERP completo, emissão fiscal, pagamentos, logística e compra automática.  
**Pendências principais:** investigar público/processo/dados e confirmar capacidades com o orientador.

## 12. Próximas entregas

Concorrência, personas, cenários e tarefas aprofundam esta base. Prototipação, coleta de dados e avaliação deverão confrontar hipóteses com evidência, mantendo explícita a diferença entre proposta de interface e função implementada no TCC.

## 13. Comunicação do projeto

1. **Problema inicial:** a equipe relata ruptura em um comércio; causas e frequência ainda precisam ser investigadas.
2. **Contribuição prevista:** prever demanda e comparar modelos a partir de histórico disponível.
3. **Uso proposto:** [H] apoiar um possível responsável pelo estoque a compreender estimativas e planejar reposições.


# Checklist

- [ ] Está clara a diferença entre tema do TCC, escopo formal do TCC e escopo de IHC.
- [ ] A equipe declarou se o TCC já previa interface.
- [ ] Se não previa, foi derivado um usuário plausível e um objetivo de uso.
- [ ] A interface de IHC não foi apresentada como obrigação automática do TCC.
- [ ] A contribuição do TCC foi descrita sem começar por tecnologias de implementação.
- [ ] Usuários diretos e stakeholders foram diferenciados.
- [ ] Foram considerados profissionais que configuram, administram, interpretam ou decidem, quando pertinente.
- [ ] Objetivo do usuário não foi confundido com objetivo do projeto.
- [ ] Processo/problema atual foi descrito antes da solução.
- [ ] Existe situação concreta de uso/problema.
- [ ] Contexto físico, social/organizacional, dispositivos e consequências de erro foram considerados.
- [ ] Mercado/alternativas existentes foram levantados inicialmente.
- [ ] Possibilidades como dashboard, relatório, histórico, filtros e CRUD foram tratadas como hipóteses de solução, não como requisitos automáticos.
- [ ] Cada possibilidade de interface tem um objetivo/tarefa que poderia justificá-la.
- [ ] Afirmações relevantes estão marcadas `[F]`, `[H]` ou `[?]`.
- [ ] Hipóteses prioritárias receberam IDs e foram para a rastreabilidade.
- [ ] O recorte de IHC é viável para modelar, prototipar e avaliar no semestre.
- [ ] A equipe consegue explicar problema humano → contribuição computacional → forma de uso.
