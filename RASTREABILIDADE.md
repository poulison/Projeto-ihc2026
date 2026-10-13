# Matriz de rastreabilidade de IHC

**Revisão:** 13/10/2026. Esta matriz distingue o que foi registrado pela equipe, o que foi observado em fontes de mercado e o que ainda é hipótese. Nenhuma entrevista, teste com usuário ou confirmação do orientador foi realizada para esta revisão.

As hipóteses usam **descrições por extenso**, conforme a simplificação adotada pela equipe. O histórico dos códigos anteriores está na seção 6, para não apagar sua evolução. Os IDs de personas, cenários, perguntas de refinamento e recomendações permanecem. Sempre cite a entrega junto a C01/C02: em E2 são concorrentes; em E4 são cenários.

## 1. Derivação do escopo

| Elemento | Registro | Origem | Estado |
|---|---|---|---|
| Tema registrado | Previsão de estoque usando machine learning | README; E1, seção 0 | [F] Registro da equipe |
| Contribuição prevista | Prever demanda e comparar modelos | E1, seção 1 | [F] Proposta; desempenho ainda não demonstrado |
| Interface prevista | Sim, conforme documentação da equipe | README; E1, seção 0.5 | [F] Registro; fluxos obrigatórios a confirmar |
| Beneficiários possíveis | Responsável pelo estoque, proprietário, funcionários, clientes e fornecedores | E1, seção 2 | [H] Papéis e impactos a investigar |
| Usuário prioritário provisório | Responsável pelo estoque de pequeno comércio | E1, seção 2; P01 em E3 | [H] Persona não valida o público |
| Objetivo de negócio | Evitar falta e excesso ao planejar reposições | E1, seção 3 | [H] Resultado esperado |
| Recorte de IHC | Consultar dados, compreender estimativa e apoiar decisão | E1, seção 7 | Proposta da equipe |
| Recomendação calculada | Quantidade/momento dependem de regras e dados adicionais | Feedback E1; E1, seção 7.3 | [?] Confirmar no escopo formal |
| Vendas online e auxiliar | Refinamentos hipotéticos, sem pesquisa primária | E3 e E4 | [H] Não comprovados para a loja |

## 2. Hipóteses, lacunas e sua evolução

| Descrição estável | Origem | Evidência ou desenvolvimento posterior | Estado atual | Por que importa / impacto | Como investigar |
|---|---|---|---|---|---|
| Benefício das previsões para antecipar reposições | E1, 1.4 | E2 documenta recursos de mercado; E4-C01 explora decisão sob incerteza | [H] Aberta; mercado e narrativa não comprovam redução de rupturas | Sustenta valor de uso; não prometer ganho medido | Teste de conceito e acompanhamento de decisões reais |
| Compreensão dos resultados sem formação em ML | E1, 1.4 | E2-C01.1 mostra fatores com nomenclatura técnica; P01 explora pouca familiaridade digital | [H] Aberta | Orienta apresentação e ajuda; exige teste de interpretação | Testar explicações com participantes |
| Responsável pelo estoque como usuário prioritário | E1, 2.1 | P01 representa esse papel provisoriamente | [H] Aberta | Define recrutamento e tarefas | Entrevistar responsáveis e observar divisão do trabalho |
| Conhecimento comercial e familiaridade com métricas | E1, 2.4 | E2 evidencia termos de produtos; nenhum dado sobre vocabulário do público | [H] Aberta | Não presumir compreensão nem desconhecimento | Investigar exemplos, termos e experiência |
| Esforço e falhas na consolidação manual | E1, 4.2 | E4 descreve repetição e duplicidade hipotéticas | [H] Aberta | Tarefas manuais não são prova de ineficiência | Observar registros, tempos, interrupções e correções |
| Necessidade de histórico de previsões e decisões | E1, 5.5 | E3 inclui acompanhamento posterior como hipótese | [H] Aberta | Justifica histórico apenas se útil ao usuário | Investigar uso de decisões anteriores e comparação com realizado |
| Processo e dados atuais | E1, 4.1 e 10 | Apenas relatos de contagem e ruptura; demais detalhes são hipotéticos | [?] Aberta | Determina entrada de dados, qualidade e viabilidade | Examinar amostras autorizadas e responsabilidades |
| Escopo formal do TCC | E1, 0.5 e 7.3 | Referências posteriores a sete dias e recomendação não têm confirmação anexada | [?] Aberta | Condiciona fluxos e o que a interface pode afirmar | Confirmar com orientador e documento técnico |
| Acúmulo de tarefas e interrupções | Contexto E1; refinamento E3 | E4-C01/C02 exemplificam pausa e retomada | [H] Aberta | Orienta investigação de continuidade do trabalho | Observar frequência, ponto de interrupção e retomada |
| Registros distribuídos entre ferramentas | Alternativas E1; refinamento E3 | Caderno, mensagens, planilha e marketplace aparecem em E4 | [H] Aberta | Não torna integração/importação um requisito | Identificar ferramentas realmente utilizadas |
| Controle humano da decisão | Refinamento E3 | E2-RC09 é proposta própria; E4-C01 diferencia envio e resultado | [H] Necessidade; decisão provisória de design | Manter revisão e distinguir lista de pedido | Investigar responsabilidades e critérios comerciais |
| Apoio operacional de um auxiliar | Papéis possíveis E1; P02 em E3 | E4-C02 explora reconciliação de registros | [H] Aberta | P02 não deve se tornar papel obrigatório | Confirmar existência do auxiliar e casos de proprietário sozinho |
| Pouca familiaridade digital de Mariana | Construção de P01 em E3 | Narrativa e jornada hipotéticas | [H] Aberta | Idade não comprova limitação; orienta proposta a testar | Pesquisar repertório, aprendizagem e acessibilidade |
| Vendas online no pequeno comércio | Refinamento E3 | Marketplace integra E4 como recurso hipotético | [H] Aberta | Evita restringir indevidamente o público sem evidência | Confirmar canais de venda e registros |
| Percepção de incerteza e confiança | E1 revisada, seção 5.6 | Nenhum dado primário | [?] Aberta | Evita tratar previsão como garantia | Testar interpretação e critérios de rejeição da estimativa |

## 3. Necessidades, personas e cenários

Os identificadores locais da Entrega 4 foram incorporados sem criar uma segunda numeração.

| Necessidade | Capacidade relacionada | Persona | Cenário | Objetivo/tarefa candidata | Modelagem e interface | Validação |
|---|---|---|---|---|---|---|
| R04-01 — decidir reposição considerando disponibilidade, procura, prazo e recursos | Previsão como apoio; recomendação calculada condicional | P01 — Mariana | [E4-C01](docs/04_cenarios_problema.md) | Apurar disponibilidade, comparar informações e alternativas, decidir e avaliar resultado | HTA/GOMS/CTT e telas: PENDENTES; não produzidos nesta revisão | Necessidade e cenário hipotéticos |
| R04-02 — manter saldo e histórico explicáveis e comunicar pendências | Qualidade dos dados utilizados na previsão; capacidade operacional a delimitar | P02 — Rafael; P01 depende do resultado | [E4-C02](docs/04_cenarios_problema.md) | Investigar divergência, confirmar fonte, corrigir com justificativa e distinguir pendências | HTA/GOMS/CTT e telas: PENDENTES | Papel auxiliar e procedimento a investigar |

MoLIC, Figma, heurísticas e tarefas de teste ainda não foram ligados a esses cenários. Campos futuros não são tratados como artefatos já existentes.

## 4. Rastreabilidade dos padrões e recomendações

| Proposta | Objetivo candidato | Evidência/hipótese | Artefatos e recomendações | Condição |
|---|---|---|---|---|
| Resumo com acesso ao detalhe | Localizar informação para decidir | E2-C02.1/C02.2; hipótese de benefício das previsões | RC01/RC04/RC12; P01; R04-01 | Conteúdo prioritário depende da tarefa real |
| Consulta com filtros | Localizar produto/período | E2-C01.1/C02.2; volume real desconhecido | RC02/RC06; P01/P02 | Filtros e familiaridade a validar |
| Explicação da previsão | Compreender estimativa e limites | E2-C01.1; hipóteses de compreensão e vocabulário | RC03/RC05/RC07/RC08; P01 | Não prometer explicação que o modelo não produz |
| Registro revisável de decisão | Recuperar e conferir escolha | Controle humano e histórico são hipóteses | RC09; E4-C01; R04-01 | Não observado como confirmação de compra nos concorrentes |
| Estado comunicado em texto | Interpretar situação e erro | Texto/cor em E2-C02.2; princípio de acessibilidade | RC10; P01/P02 | Não representa conformidade de acessibilidade verificada |
| Preparação/conferência dos dados | Sustentar disponibilidade confiável | Lacuna sobre processo; E4-C02 hipotético | RC08/RC11; P02; R04-02 | Cadastro/importação e permissões dependem da pesquisa |
| Comparação com realizado | Avaliar utilidade após a compra | Hipótese de histórico em E1; jornada E3 | RC05; P01 | Não comprovada apenas pela existência de gráficos de previsões e ajustes |

Não foram atribuídos IDs de telas antes de existir um modelo de interação. F01–F06 na Entrega 1 identificam ações candidatas, não telas implementadas.

## 5. Registro de mudanças

| Data | Mudança | Motivo/evidência | Artefatos afetados |
|---|---|---|---|
| 13/10/2026 | Completar tabelas, qualificar fatos e explicitar lacunas | Feedback do professor da E1 | E1; README; matriz |
| 13/10/2026 | Tratar recomendação calculada e horizonte como pendências | Feedback E1; ausência de confirmação técnica anexada | E1, E2, E3, E4 |
| 13/10/2026 | Manter Blue Yonder e Netstock como conjunto atual | Escolha da equipe durante a revisão; coerência com texto das entregas | E2; fontes de imagens; matriz |
| 13/10/2026 | Retirar Odoo/Zoho do conjunto ativo sem apagar arquivos | Divergência identificada no feedback E2 | Arquivos preservados em historico/2026-10-13 |
| 13/10/2026 | Usar figuras oficiais com legendas e limites | Conferência visual e documental nesta revisão | E2-C01.1–C01.3; E2-C02.1–C02.2 |
| 13/10/2026 | Corrigir origem de RC09/RC10 e demais inferências | Feedback E2 e inspeção das figuras | E2; padrões nesta matriz |
| 13/10/2026 | Substituir códigos de hipóteses por descrições | Simplificação solicitada pela equipe; conflito de significados entre E1/E3 | E1–E4; matriz; histórico abaixo |
| 13/10/2026 | Integrar P01/P02 e R04-01/R04-02 | Continuidade com cenários enviados | E3, E4 e seção 3 desta matriz |
| 13/10/2026 | Padronizar matrícula de Victor como 22.125.075-6 | Concordância entre README, E1 e E3 | E2 |

## 6. Histórico de correspondência dos identificadores retirados

Este registro é **histórico**, não o esquema ativo de referência. O professor recomendou IDs estáveis; a equipe optou por descrições para simplificar a leitura. A aceitação acadêmica dessa mudança de formato não foi confirmada. Origem, estado e evolução continuam documentados.

| Código antigo | Sentido na Entrega 1 | Sentido utilizado na Entrega 3 anterior | Tratamento atual |
|---|---|---|---|
| H01 | Benefício das previsões | Usuário prioritário | Duas hipóteses distintas preservadas por descrição |
| H02 | Compreensão sem formação em ML | Acúmulo de tarefas/pouco tempo | Distinção preservada; nenhuma confirmada |
| H03 | Usuário prioritário | Registros distribuídos | Distinção preservada; conferir processos reais |
| H04 | Conhecimento comercial sem métricas de ML | Familiaridade com termos técnicos | Tema equivalente; permanece hipótese |
| H05 | Esforço e erros manuais | Controle humano da compra | Distinção preservada; controle humano é refinamento |
| H06 | Histórico de previsões | Participação de auxiliar | Distinção preservada; auxiliar não substitui histórico |
| H07 | Não existia | Pouca familiaridade digital de Mariana | Registrada como hipótese acrescentada em E3 |
| Q01/Q02 | Processo/dados; escopo formal | Não preservados como referências centrais | Lacunas mantidas por descrição |
| F01 em E3 | Em E1 era ação candidata de identificar riscos | Foi usado como fato sobre previsão e recomendação | Referência ambígua retirada de E3; previsão é proposta registrada e recomendação é pendência |


## Como atualizar

- Referenciar hipóteses pelo nome descritivo desta matriz e seção de origem.
- Registrar nova evidência com fonte, data, limite e impacto; narrativa fictícia não valida hipótese.
- Usar prefixo de entrega em C01/C02 para distinguir concorrentes de cenários.
- Manter P01/P02, perguntas Cxx-Qn, RC01–RC12 e DP01–DP18 nos artefatos correspondentes.
- Acrescentar modelos, telas e testes somente quando existirem; registrar mudanças no histórico.
