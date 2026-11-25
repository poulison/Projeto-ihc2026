# Matriz de rastreabilidade de IHC

**Revisão:** 25/11/2026. A seção 3.1 incorpora a cadeia completa até MoLIC, Figma e avaliação. Esta matriz distingue o que foi registrado pela equipe, o que foi observado em fontes de mercado e o que ainda é hipótese. Ainda não houve entrevista, resposta ao questionário publicado (E7), teste de usabilidade com usuários nem confirmação do orientador. A única observação com pessoa externa é o walkthrough formativo da E6 (W01, 24/11/2026), com uma pessoa que já conhecia o projeto. Por isso, ele não muda o estado de nenhuma hipótese.

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

| ID | Descrição estável | Origem | Evidência ou desenvolvimento posterior | Estado atual | Por que importa / impacto | Como investigar |
|---|---|---|---|---|---|---|
| HP01 | Benefício das previsões para antecipar reposições | E1, 1.4 | E2 documenta recursos de mercado; E4-C01 explora decisão sob incerteza | [H] Aberta; mercado e narrativa não comprovam redução de rupturas | Sustenta valor de uso; não prometer ganho medido | Teste de conceito e acompanhamento de decisões reais |
| HP02 | Compreensão dos resultados sem formação em ML | E1, 1.4 | E2-C01.1 mostra fatores com nomenclatura técnica; P01 explora pouca familiaridade digital. No walkthrough da E6, W01 relatou dúvida sobre o significado de alguns dados e não conhecia o termo “SKU” (evidência formativa de uma pessoa). Na E14, dois participantes sem experiência com estoque explicaram disponibilidade, previsão e saldo sem ajuda (participantes aproximados, sem generalização) | [H] Aberta | Orienta apresentação e ajuda; exige teste de interpretação | Testar explicações com participantes |
| HP03 | Responsável pelo estoque como usuário prioritário | E1, 2.1 | P01 representa esse papel provisoriamente | [H] Aberta | Define recrutamento e tarefas | Entrevistar responsáveis e observar divisão do trabalho |
| HP04 | Conhecimento comercial e familiaridade com métricas | E1, 2.4 | E2 evidencia termos de produtos; nenhum dado sobre vocabulário do público | [H] Aberta | Não presumir compreensão nem desconhecimento | Investigar exemplos, termos e experiência |
| HP05 | Esforço e falhas na consolidação manual | E1, 4.2 | E4 descreve repetição e duplicidade hipotéticas | [H] Aberta | Tarefas manuais não são prova de ineficiência | Observar registros, tempos, interrupções e correções |
| HP06 | Necessidade de histórico de previsões e decisões | E1, 5.5 | E3 inclui acompanhamento posterior como hipótese | [H] Aberta | Justifica histórico apenas se útil ao usuário | Investigar uso de decisões anteriores e comparação com realizado |
| HP07 | Processo e dados atuais | E1, 4.1 e 10 | Apenas relatos de contagem e ruptura; demais detalhes são hipotéticos | [?] Aberta | Determina entrada de dados, qualidade e viabilidade | Examinar amostras autorizadas e responsabilidades |
| HP08 | Escopo formal do TCC | E1, 0.5 e 7.3 | Referências posteriores a sete dias e recomendação não têm confirmação anexada | [?] Aberta | Condiciona fluxos e o que a interface pode afirmar | Confirmar com orientador e documento técnico |
| HP09 | Acúmulo de tarefas e interrupções | Contexto E1; refinamento E3 | E4-C01/C02 exemplificam pausa e retomada | [H] Aberta | Orienta investigação de continuidade do trabalho | Observar frequência, ponto de interrupção e retomada |
| HP10 | Registros distribuídos entre ferramentas | Alternativas E1; refinamento E3 | Caderno, mensagens, planilha e marketplace aparecem em E4 | [H] Aberta | Não torna integração/importação um requisito | Identificar ferramentas realmente utilizadas |
| HP11 | Controle humano da decisão | Refinamento E3 | E2-RC09 é proposta própria; E4-C01 diferencia envio e resultado | [H] Necessidade; decisão provisória de design | Manter revisão e distinguir lista de pedido | Investigar responsabilidades e critérios comerciais |
| HP12 | Apoio operacional de um auxiliar | Papéis possíveis E1; P02 em E3 | E4-C02 explora reconciliação de registros | [H] Aberta | P02 não deve se tornar papel obrigatório | Confirmar existência do auxiliar e casos de proprietário sozinho |
| HP13 | Pouca familiaridade digital de Mariana | Construção de P01 em E3 | Narrativa e jornada hipotéticas | [H] Aberta | Idade não comprova limitação; orienta proposta a testar | Pesquisar repertório, aprendizagem e acessibilidade |
| HP14 | Vendas online no pequeno comércio | Refinamento E3 | Marketplace integra E4 como recurso hipotético | [H] Aberta | Evita restringir indevidamente o público sem evidência | Confirmar canais de venda e registros |
| HP15 | Percepção de incerteza e confiança | E1 revisada, seção 5.6 | Nenhum dado primário | [?] Aberta | Evita tratar previsão como garantia | Testar interpretação e critérios de rejeição da estimativa |

## 3. Necessidades, personas e cenários

Os identificadores locais da Entrega 4 foram incorporados sem criar uma segunda numeração.

| Necessidade | Capacidade relacionada | Persona | Cenário | Objetivo/tarefa candidata | Modelagem e interface | Validação |
|---|---|---|---|---|---|---|
| R04-01 — decidir reposição considerando disponibilidade, procura, prazo e recursos | Previsão como apoio; recomendação calculada condicional | P01 — Mariana | [E4-C01](docs/04_cenarios_problema.md) | Apurar disponibilidade, comparar informações e alternativas, decidir e avaliar resultado | [T01 — HTA](docs/05_analise_tarefas.md#t01-hta), [GOMS](docs/05_analise_tarefas.md#t01-goms) e [CTT](docs/05_analise_tarefas.md#t01-ctt) produzidos; autoria: Paulo. Interface: cartões P07–P14 (E6), [M01](docs/10_molic.md) e F01–F06R (E11) | Necessidade e cenário hipotéticos. PF01 percorrido no walkthrough W01 (E6) |
| R04-02 — manter saldo e histórico explicáveis e comunicar pendências | Qualidade dos dados utilizados na previsão; capacidade operacional a delimitar | P02 — Rafael; P01 depende do resultado | [E4-C02](docs/04_cenarios_problema.md) | Investigar divergência, confirmar fonte, corrigir com justificativa e distinguir pendências | [T02 — HTA](docs/05_analise_tarefas.md#t02-hta), [GOMS](docs/05_analise_tarefas.md#t02-goms) e [CTT](docs/05_analise_tarefas.md#t02-ctt) produzidos; autoria: Victor. Interface: cartões P15–P17P (E6), [M02](docs/10_molic.md) e F10–F14N (E11) | Papel auxiliar e procedimento a investigar. PF02 não foi percorrido no walkthrough W01 |

### 3.1 Cadeia completa: da persona à avaliação

A matriz abaixo reflete o estado do repositório em 25/11/2026. Ela permite interpretar um problema observado numa tela sabendo qual cena do MoLIC o originou, qual objetivo é apoiado, quais signos estão envolvidos e qual tarefa é afetada. As Entregas 12 e 13 estão em andamento e a 14 ainda não tem sessões. Nessas colunas, o que é **previsto** está separado do que já foi **registrado**.

| Persona | Cenário de problema | Cenário de interação | Objetivo final | MoLIC | Fluxo principal no Figma | Metas (E8) | Tarefas de teste (E12/E14) | Inspeção (E13) |
|---|---|---|---|---|---|---|---|---|
| P01 — Mariana (autoria Paulo) | [E4-C01](docs/04_cenarios_problema.md) · R04-01 · T01 | [CI01](docs/09_modelo_conceitual.md#ci01--decidir-a-reposição-da-garrafa-antes-do-prazo-do-fornecedor) | **O01** — Tomar uma decisão de reposição fundamentada e recuperável | [M01](docs/10_molic.md#m01--decidir-a-reposição-de-um-item) | F01 → F02 → F03 → F04 → F05 → F05S | MU01–MU07 (MU06 não avaliada nesta versão) | UT01 (T01-A), UT02 (T01-B), UT05/M01 — previstas | A02-V01, A02-V03 a A02-V07, A02-V09, A02-V11 a A02-V14 → C01, C02, C05–C13. Observação (E14): AU01, AU02, AU03 |
| P02 — Rafael (autoria Victor) | [E4-C02](docs/04_cenarios_problema.md) · R04-02 · T02 | [CI02](docs/09_modelo_conceitual.md#ci02--explicar-a-diferença-no-saldo-dos-conjuntos-de-potes) | **O02** — Tornar o saldo do item confiável e explicável | [M02](docs/10_molic.md#m02--explicar-a-diferença-no-saldo-de-um-item) | F01 → F10 → F11 → F12 → F13 | MU01, MU03–MU07 (MU06 não avaliada nesta versão) | UT03 (T02-A), UT04 (T02-B), UT05/M02 — previstas | A01-V01, A01-V02; A02-V02, A02-V05, A02-V08, A02-V10, A02-V11, A02-V13 → C02, C03, C04, C06, C11, C13. Observação (E14): AU01 |

#### Objetivo → signos → cena do MoLIC → estados do Figma → avaliação

| Objetivo (E9) | Tipo | Signos principais | Cena do MoLIC | Estados no Figma | Meta/tarefa/inspeção |
|---|---|---|---|---|---|
| O01 | Final | desfecho da reposição; estado do registro | M01: `gco` na abertura; `gcc` após O08 ou abandono | F01 → F05S; abandono em F05 (“Descartar rascunho”) | MU01; UT01, UT02 |
| O02 | Final | desfecho da conferência; saldo registrado | M02: `gco` na abertura; `gcc` após O08 ou abandono | F01 → F13 ou F14/F14N | MU01; UT03, UT04 |
| O03 | Instrumental direto | produto; unidade de venda | M01 e M02 · O03 | F01; identificação em F02 e F10 | MU04 (produto ou unidade errados = erro crítico) |
| O04 | Instrumental direto | contagem física; quantidade comprometida/disponível; vendas confirmadas; atualização da base; previsão de demanda; horizonte; prazo do fornecedor; [sugestão de reposição, condicional] | M01 · O04 | F02; F02B | MU02, MU03; UT01, UT02; A02-V09, A02-V11, A02-V14; E14: AU02 |
| O05 | Instrumental direto | desfecho da reposição; quantidade planejada; motivo; próxima verificação | M01 · O05 e revisão | F03, F04, F04Q, F04E, F05/F05Q/F05A/F05P | MU04; UT01, UT02; A02-V01, A02-V03, A02-V04, A02-V06, A02-V07; E14: AU02, AU03; walkthrough W01: hesitação na escolha do desfecho (E6) |
| O06 | Instrumental direto | evidência de origem; situação da evidência | M02 · O06 | F10, F11, F11P | MU03; UT03, UT04; A01-V02, A02-V02, A02-V08, A02-V10 |
| O07 | Instrumental direto | correção da transcrição; desfecho da conferência; motivo; próxima verificação | M02 · O07 e revisão | F12, F12N, F12P | MU04; UT03, UT04; A01-V01, A02-V11 |
| O08 | Instrumental direto | estado do registro; responsável e data | M01/M02 · O08 e gravação incerta | F05S…F05PS, F06E, F06R, F12E, F12F, F13, F14/F14N | MU01, MU04; A02-V05, A02-V12, A02-V13 |
| O09 | Instrumental direto (com pausa) | ponto de retomada; atualização da base; estado do registro | M01/M02 · O09 | F02P, F10P, F11P | MU07; UT05; A01-V02, A02-V10; E14: AU01 |
| O10 | Instrumental indireto de O01 | alcance da conferência | M02 · O10 (opcional, após `gcc` de O02) | F13 | UT03 (“diga a ela como ficou esse item”); MU04 (declaração indevida de conferência total) |

Os detalhes de cada ligação estão no [mapa e no dicionário de objetivos (E9)](docs/09_modelo_conceitual.md#3-mapa-de-objetivos), na [consolidação do MoLIC (E10)](docs/10_molic.md#consolidação-da-equipe), na [cobertura MoLIC → Figma (E11)](docs/11_figma.md#cobertura-molic--figma), no [plano DECIDE (E12)](docs/12_planejamento_avaliacao.md) e nas fichas da [E13](docs/13_avaliacao_heuristica.md). Quando a E14 produzir resultados, a última coluna receberá os achados observados, a decisão de revisão e a nova verificação.

### Metas de usabilidade da Entrega 8

R04-01 fundamenta T01, a decisão de reposição de Mariana. R04-02 fundamenta T02, a investigação de divergências por Rafael. Os casos A e B e os limites de cada meta estão definidos na [Entrega 8](docs/08_engenharia_usabilidade.md). As telas abaixo constam da [Entrega 11](docs/11_figma.md). A última coluna descreve o registro a produzir na avaliação.

| Necessidade e tarefa | Decisão de interface | Meta da E8 | Evidência prevista |
|---|---|---|---|
| R04-01/T01 e R04-02/T02 · concluir o trabalho do item | Mostrar o desfecho salvo da reposição ou da conferência em F05S ou F13 | MU01 · Eficácia | Classificação da primeira tentativa de cada caso A, com ajuda recebida e conferência do resultado final. |
| R04-01/T01 · interpretar disponibilidade e previsão | Separar físico, comprometido e disponível em F02, identificar ausência de estimativa em F02B e explicitar o que foi salvo | MU02 · Compreensão | Explicação, nas palavras da pessoa, dos quatro pontos dos casos T01-A e T01-B. |
| R04-01/T01 e R04-02/T02 · decidir ou conferir durante o expediente | Reunir a base da decisão em F02 e as fontes da divergência em F11 antes da revisão | MU03 · Eficiência | Tempo ativo por caso A concluído sem ajuda, com espera, pausa e tentativas interrompidas registradas separadamente. |
| R04-01/T01 e R04-02/T02 · evitar registro indevido | Revisar produto e quantidade antes de salvar. Em F12P e F12N, preservar o saldo quando faltar evidência ou autorização. | MU04 · Segurança | Contagem e descrição dos erros críticos por tentativa, incluindo os casos B, e registro à parte dos desvios recuperados. |
| R04-01/T01 e R04-02/T02 · entender o resultado da própria ação | Mostrar um resumo da decisão em F05S e do saldo corrigido em F13 | MU05 · Satisfação | Nota pós-tarefa de 1 a 5 e motivo declarado, registrados por participante e tarefa. |
| R04-01/T01 e R04-02/T02 · ganhar autonomia | Manter as etapas de identificar, revisar e confirmar reconhecíveis ao mudar o item | MU06 · Aprendizagem | Comparação de ajuda, conclusão e erros críticos entre duas execuções equivalentes na mesma sessão. |
| R04-01/T01 e R04-02/T02 · retomar após atendimento | Reapresentar contexto e próxima ação em F02P ou F10P | MU07 · Retomada | Após a pausa, tempo para identificar o contexto e a próxima ação, com verificação de duplicação. |

O [DECIDE da E12](docs/12_planejamento_avaliacao.md) orienta a coleta. A [E13](docs/13_avaliacao_heuristica.md) pode apontar problemas para revisão antes das sessões. A [E14](docs/14_observacao_usuario.md) é a referência para a observação com participantes. Ao dispor de dados, registrar versão, caso, evidência, decisão de revisão e nova verificação. A definição destas metas preserva o estado das hipóteses da seção 2.

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

F01–F06 na Entrega 1 identificam ações candidatas, não telas. Os IDs Fxx de telas e estados usados a partir da seção 3.1 são os quadros do protótipo da [Entrega 11](docs/11_figma.md), derivados do MoLIC da Entrega 10.

## 5. Registro de mudanças

| Data | Mudança | Motivo/evidência | Artefatos afetados |
|---|---|---|---|
| 13/10/2026 | Completar tabelas, qualificar fatos e explicitar lacunas | Feedback do professor da E1 | E1; README; matriz |
| 13/10/2026 | Tratar recomendação calculada e horizonte como pendências | Feedback E1; ausência de confirmação técnica anexada | E1, E2, E3, E4 |
| 13/10/2026 | Manter Blue Yonder e Netstock como conjunto atual | Escolha da equipe durante a revisão; coerência com texto das entregas | E2; fontes de imagens; matriz |
| 13/10/2026 | Retirar Odoo/Zoho do conjunto ativo sem apagar arquivos | Divergência identificada no feedback E2 | Arquivos preservados em `assets/historico/2026-10-13_concorrencia/` (movidos da pasta ativa em 25/11/2026) |
| 13/10/2026 | Usar figuras oficiais com legendas e limites | Conferência visual e documental nesta revisão | E2-C01.1–C01.3; E2-C02.1–C02.2 |
| 13/10/2026 | Corrigir origem de RC09/RC10 e demais inferências | Feedback E2 e inspeção das figuras | E2; padrões nesta matriz |
| 13/10/2026 | Substituir códigos de hipóteses por descrições | Simplificação solicitada pela equipe; conflito de significados entre E1/E3 | E1–E4; matriz; histórico abaixo |
| 13/10/2026 | Integrar P01/P02 e R04-01/R04-02 | Continuidade com cenários enviados | E3, E4 e seção 3 desta matriz |
| 13/10/2026 | Padronizar matrícula de Victor como 22.125.075-6 | Concordância entre README, E1 e E3 | E2 |
| 24/11/2026 | Refazer os cartões da E6 (P07-0 a P17P) e o mapa dos percursos PF01, PF02 e PF03 | Revisão da equipe na E6 | E6; `assets/06_prototipos/`; seção 3 desta matriz (cartões P07–P14 e P15–P17P) |
| 24/11/2026 | Revisar a coleta de dados da E7 e a engenharia de usabilidade da E8, ligando R04-01/R04-02, T01/T02 e as metas MU01–MU07 | Revisão da equipe nas E7 e E8 | E7, E8; seção “Metas de usabilidade da Entrega 8” desta matriz |
| 25/11/2026 | Reformular O01/O02 como objetivos finais e classificar O03–O10 como instrumentais diretos/indireto | Feedback das Entregas 9 e 10 | E9 (mapas, dicionário e DCC), E10, E11, E13 |
| 25/11/2026 | Encerrar O02 em O08 e tornar O10 uma consulta opcional do alcance | Feedback E10: a comunicação a Mariana ocorre fora do sistema | M02; E10; E11 (F13) |
| 25/11/2026 | Alinhar as cenas do MoLIC aos nomes dos signos e restringir `d+u:` | Feedback E10 | M01, M02 |
| 25/11/2026 | Registrar a divergência de rótulos entre E9 e Figma e os estados a preservar | Feedback E11 | E11 |
| 25/11/2026 | Ligar personas, cenários, objetivos, MoLIC, Figma, metas, tarefas de teste e inspeção | Feedback E9, E10 e E11: matriz desatualizada | Seção 3.1 desta matriz |
| 25/11/2026 | Arquivar placeholders `f01.svg`, `v01.svg` e `fluxograma_avaliacao.svg`; substituir `mapa_objetivos.svg` pela fonte real | Feedback E11 | `assets/historico/2026-11-25_placeholders/` |
| 25/11/2026 | Registrar a sessão de 23/11 (W01) como não documentada e acrescentar um walkthrough cognitivo simulado, sem participante | Feedback E6. As decisões foram só ajustes de texto e de estado, a maioria já presente na E11 | E6, seção 4 |
| 25/11/2026 | Registrar as observações da sessão W01 de 23/11 (PF01 e PF03) e as decisões correspondentes | Feedback E6. Sem mudanças estruturais | E6, seções 4 e 5 |
| 25/11/2026 | Retirar o walkthrough cognitivo simulado da E6, mantendo só a sessão com W01; retirar do repositório o script do I01 e a ficha do I02 | Decisão da equipe. O formulário segue publicado e o roteiro da entrevista continua na E7 | E6, E7, `instrumentos/` |
| 25/11/2026 | Atualizar o cabeçalho, a cobertura de interface de R04-01/R04-02 e a hipótese de compreensão com o walkthrough W01, sem mudar estados | Revisão final da matriz | Seções 2, 3 e 3.1 |
| 25/11/2026 | Publicar o questionário I01 e registrar o link, com acesso sem login e saltos verificados | Feedback E7. A publicação não é evidência sobre as hipóteses, que continuam abertas | E7, instrumento I01 |
| 25/11/2026 | Mapear as etapas do ciclo de Mayhew para os artefatos e indicar a etapa atual | Feedback E8 | E8, seção 4 |
| 25/11/2026 | Alinhar mais rótulos do Figma aos signos da E9 (F01, F02B, F02P, F03, F05P, F05PS, F06E, F06R, F12E, F12N, F12P) e verificar as 57 ligações no modo de apresentação | Revisão final das E9–E11 | E11; capturas f01.png e f13.png |
| 25/11/2026 | Concluir o plano DECIDE da E12 com registro por fichas e cronômetro, sem gravação, e alinhar o termo e a E14 | Decisão da equipe na E12 | E12, E14 (passo 3), termo de consentimento |
| 25/11/2026 | Registrar as fichas individuais da E13 e trocar os IDs antigos (PRE-01 a PRE-03 e a numeração anterior de A01) pelos IDs atuais das fichas | Inspeções de Paulo (A01) e Victor (A02) em 25/11/2026 | E13, seção 3.1 desta matriz, E11 |
| 25/11/2026 | Consolidar os 16 achados da E13 em 13 problemas únicos (C01–C13), com grau final, prioridade e responsável; C01–C05 a corrigir antes da E14 | Consolidação da dupla na E13 | E13 (seções 7 e 8), E14 (versão a registrar após as correções) |
| 25/11/2026 | Preencher a comparação da E14 com a heurística usando os IDs C01–C13 | Consolidação da E13 | E14, seção F |
| 25/11/2026 | Aplicar no Figma as correções C01–C05 e parte de C06: novo F04Q (edição preserva 4 unidades), novo F11P (pausa durante a comparação), controles da simulação movidos para pontos de início do moderador, unidade dos potes explícita e área de clique maior em F03 | Consolidação da E13 | Figma; E11 (correções), E12 (versão), E13 (seção 8), E14 (versão e preparação) |
| 25/11/2026 | Retirar o teste piloto do plano e trocá-lo por uma conferência do protótipo e dos materiais antes da primeira sessão; registrar que os dois participantes já foram identificados | Decisão da equipe | E8 (limites das metas), E11, E12, E14 (passos 2 e 4, fluxograma, conclusão e checklist) |
| 25/11/2026 | Registrar as sessões da E14 (U01 e U02) e os achados AU01–AU03; ligar AU02 e AU03 a O04/O05 e AU01 a O09 | Sessões com dois participantes aproximados, sem termo assinado; UT05 e pós-teste em conjunto | E14 (seções C–G), seções 2 e 3.1 desta matriz |
| 25/11/2026 | Registrar o aceite dos dois participantes, obtido depois da sessão e gravado em vídeo | Vídeos conferidos pela equipe e guardados fora do repositório | E14 (passo 3, conclusão e checklist) |
| 25/11/2026 | Registrar o termo escrito assinado pelos dois participantes | Confirmação por mensagem; vias guardadas fora do repositório | E14 (passo 3, conclusão e checklist) |
| 25/11/2026 | Dar IDs estáveis HP01–HP15 às hipóteses e lacunas, com correspondência aos códigos antigos | Recomendação do professor (IDs estáveis); checklist da E1 | Seções 2 e 6 desta matriz; E1, seção 10 |
| 25/11/2026 | Revisão final contra os feedbacks E1–E11: mover as capturas de Odoo e Zoho para o histórico, completar a tabela da equipe no README e anotar os itens abertos da E8 | Feedback E1 (identificação) e E2 (divergência de imagens) | E2, README, E8, `assets/historico/2026-10-13_concorrencia/` |
| 25/11/2026 | Alinhar o fim da T02 na E5: a tarefa termina quando Rafael comunica o alcance a Mariana, fora do sistema; a verificação do recebimento deixa de ser critério de conclusão (HTA 4.3, GOMS G4 e nó U4 do CTT) | Inconsistência entre E5 e E9/E10/E14 apontada na revisão final | E5 (HTA, GOMS, CTT e diagrama `ctt_t02`) |
| 25/11/2026 | Corrigir a data do walkthrough W01 de 23/11 para 24/11/2026; a sessão ocorreu depois da revisão dos cartões do mesmo dia. As linhas anteriores deste histórico mantêm a data com que foram escritas | Confirmação da equipe | E6 (status e seções 4 e 5), E8, cabeçalho desta matriz |
| 25/11/2026 | Identificar as versões do Figma: E13 inspecionou o estado com 28 quadros, antes das correções; E14 usou o estado com 30 quadros, salvo no histórico de versões como “E14 · estado das sessões de 25/11/2026” | O link do Figma é mutável | E11, E12, E13 e E14 |
| 25/11/2026 | Corrigir o perfil de U01 e U02: nenhum dos dois conhecia o projeto antes da sessão; a menção a contato prévio sai dos perfis, do pré-teste e das limitações | Correção da equipe | E14 (passo 2, seção C e conclusão) |

**Revisão de 12/11/2026:** P02 classificada como persona primária do recorte operacional, por objetivo e uso direto previstos; existência/recorrência continuam hipóteses. E3 passa a preservar visuais locais e a separar contexto de solução. C02 deixa de antecipar duplicidade no título; ambas as tabelas de perguntas explicitam os sete elementos. E5 inclui Input/Feedback/Plano na tarefa zero, GOMS indentado, CTT com gatilho inicial e fechamento da comunicação; modelagem concluída, pesquisa futura não realizada.

## 6. Histórico de correspondência dos identificadores retirados

Este registro é **histórico**. O professor recomendou IDs estáveis. Em 13/10/2026 a equipe trocou os códigos antigos por descrições; em 25/11/2026 as hipóteses voltaram a ter IDs estáveis, **HP01–HP15** (seção 2). O prefixo HP evita repetir H01–H07, que tinham sentidos diferentes na E1 e na E3. A última coluna indica o ID atual de cada sentido antigo.

| Código antigo | Sentido na Entrega 1 | Sentido utilizado na Entrega 3 anterior | Tratamento atual |
|---|---|---|---|
| H01 | Benefício das previsões | Usuário prioritário | Duas hipóteses distintas: HP01 (E1) e HP03 (E3) |
| H02 | Compreensão sem formação em ML | Acúmulo de tarefas/pouco tempo | HP02 (E1) e HP09 (E3); nenhuma confirmada |
| H03 | Usuário prioritário | Registros distribuídos | HP03 (E1) e HP10 (E3); conferir processos reais |
| H04 | Conhecimento comercial sem métricas de ML | Familiaridade com termos técnicos | Tema equivalente: HP04; permanece hipótese |
| H05 | Esforço e erros manuais | Controle humano da compra | HP05 (E1) e HP11 (E3); controle humano é refinamento |
| H06 | Histórico de previsões | Participação de auxiliar | HP06 (E1) e HP12 (E3) |
| H07 | Não existia | Pouca familiaridade digital de Mariana | HP13, acrescentada em E3 |
| Q01/Q02 | Processo/dados; escopo formal | Não preservados como referências centrais | HP07 e HP08 |
| F01 em E3 | Em E1 era ação candidata de identificar riscos | Foi usado como fato sobre previsão e recomendação | Referência ambígua retirada de E3; previsão é proposta registrada e recomendação é pendência |


## Como atualizar

- Referenciar hipóteses pelo nome descritivo desta matriz e seção de origem.
- Registrar nova evidência com fonte, data, limite e impacto; narrativa fictícia não valida hipótese.
- Usar prefixo de entrega em C01/C02 para distinguir concorrentes de cenários.
- Manter P01/P02, perguntas Cxx-Qn, RC01–RC12 e DP01–DP18 nos artefatos correspondentes.
- Ao alterar um objetivo, signo, cena ou estado do Figma, atualizar a seção 3.1 e registrar a mudança na seção 5. Na seção 3.1, mover os resultados de avaliação de “previstos” para “registrados” somente quando houver evidência.
