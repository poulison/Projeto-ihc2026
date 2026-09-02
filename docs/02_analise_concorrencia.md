# Entrega 2 — Público-alvo e análise de concorrência

**Data:** 26/08/2026

**Status:** 🟨 em andamento

**Responsabilidade:** cada integrante analisa ao menos uma interface; a equipe produz a comparação.

Objetivo da atividade

Compreender soluções do mesmo domínio **e também interfaces familiares ao público-alvo**. O objetivo não é copiar telas, mas identificar convenções, padrões, affordances percebidas, problemas recorrentes, expectativas e oportunidades de design.

> **Concorrente não precisa ser idêntico ao produto.** Pode atuar na mesma área, resolver objetivo semelhante ou disputar a mesma necessidade. Quando não houver concorrente direto, use produtos análogos e softwares que o público já utiliza.

### Para TCCs que não previam interface

Não procure apenas um “concorrente do algoritmo”. Investigue **interfaces profissionais que materializam atividades semelhantes** às que o usuário escolhido precisaria realizar.

Exemplos:

- TCC de banco de dados → consoles de administração, ferramentas para DBA, monitoramento e análise de consultas;
- TCC de LLM/ML → painéis de experimentos, gestão de modelos/datasets, comparação de métricas, revisão de resultados;
- TCC de análise de dados → dashboards, ferramentas de BI, filtros, relatórios e exploração;
- TCC de infraestrutura/API → portais administrativos, observabilidade, logs, gestão de credenciais e uso;
- TCC de cibersegurança → consoles de alertas, triagem, histórico e auditoria.

A pergunta é: **“que convenções esse perfil já conhece para executar tarefas equivalentes?”**

## Entrada obrigatória da Entrega 1

Retome o mapa inicial de alternativas e produtos citado na Entrega 1. Aqui a equipe deixa de trabalhar apenas com impressão inicial e passa a **investigar sistematicamente** cada solução.

| Item citado na Entrega 1 | Tipo | Por que foi citado | Status inicial | Decisão nesta entrega |
|---|---|---|---|---|
| Blue Yonder Demand Planning | concorrente indireto / interface profissional análoga | É uma referência consolidada em previsão de demanda, planejamento de estoque e apoio à reposição em cadeias de suprimentos complexas | F | analisar como C01 |
| Netstock | concorrente indireto / interface profissional análoga | Oferece previsão de demanda, otimização de estoque e recomendações de reposição para pequenas e médias empresas | F | analisar como C02 |

Se uma hipótese da Entrega 1 for confirmada ou refutada durante esta análise, atualize `H01`, `H02`... em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).


## 1. Público-alvo desta análise

O público-alvo é o **responsável pelo estoque de um pequeno comércio**, muitas vezes o próprio proprietário, que acumula atividades de compra, venda e controle operacional. Ele precisa acompanhar o saldo dos produtos, identificar riscos de ruptura ou excesso e decidir o que, quando e quanto repor.

Esse usuário tende a reconhecer termos cotidianos como produto, saldo, entrada, saída, estoque mínimo, fornecedor e prazo de entrega, mas pode não dominar conceitos como erro de previsão, *machine learning*, *fill rate* ou estoque de segurança calculado. A interface deve, portanto, traduzir resultados técnicos em informações operacionais, explicar os alertas e manter o usuário no controle da decisão de reposição.

## 2. Concorrentes diretos/indiretos

### Análise C01 — Blue Yonder Demand Planning

**Autor(a):** Paulo Andre de Oliveira Hirata — 22.125.072-3  
**Tipo:** indireto / análogo  
**Link oficial:** https://blueyonder.com/solutions/supply-chain-planning/demand-planning  
**Data de acesso:** 02/09/2026

#### Contexto e proposta

O Blue Yonder Demand Planning integra uma plataforma corporativa de planejamento e execução da cadeia de suprimentos. A solução combina métodos estatísticos, aprendizado de máquina e inteligência artificial para gerar previsões, analisar fatores que afetam a demanda, apoiar planejamento colaborativo e reduzir faltas e excessos de estoque. É voltada principalmente a organizações com grande volume de dados, várias localidades e cadeias de suprimentos complexas.

O produto é indireto em relação ao projeto porque possui escopo, custo e complexidade superiores à realidade do microempreendedor brasileiro. Mesmo assim, funciona como referência de como transformar previsões em informações explicáveis, alertas e ações de planejamento.

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| Previsão de demanda | Combina métodos estatísticos, ML, IA e sinais internos ou externos para estimar a demanda | [`assets/02_concorrencia/blue_yonder_interface.webp`](assets/02_concorrencia/blue_yonder_interface.webp) | A automação reduz trabalho repetitivo, mas a origem e a atualização dos dados precisam estar visíveis para gerar confiança |
| Explicação dos fatores | A abordagem divulgada como *glass box* apresenta fatores causais associados às previsões | [Página oficial de Demand Planning](https://blueyonder.com/solutions/supply-chain-planning/demand-planning) | Explicar por que o valor mudou permite avaliar a recomendação sem exigir conhecimento do algoritmo |
| Alertas e recomendações | A experiência pública destaca acontecimentos, riscos, indicadores e ações possíveis | [`assets/02_concorrencia/blue_yonder_interface.webp`](assets/02_concorrencia/blue_yonder_interface.webp) | O encadeamento “o que aconteceu → por que importa → o que fazer” reduz a distância entre informação e ação |
| Planejamento de cenários | Permite comparar alternativas e avaliar impactos antes da decisão | [Página oficial de Demand Planning](https://blueyonder.com/solutions/supply-chain-planning/demand-planning) | O cenário ativo e as diferenças entre alternativas devem estar claramente identificados |
| Visão multidimensional | Organiza a análise por produto, local, cliente e período | [Página oficial de Demand Planning](https://blueyonder.com/solutions/supply-chain-planning/demand-planning) | É útil para catálogos complexos, mas dimensões demais podem aumentar a carga cognitiva |

#### Experiência do usuário e opiniões

Na data da consulta, o G2 apresentava nota geral de **4,1/5 em 30 avaliações** para o Blue Yonder Demand Planning. Há relatos favoráveis sobre economia de tempo, possibilidade de ajustar dados e facilidade depois do aprendizado inicial. Também aparecem relatos de curva de aprendizagem, necessidade de treinamento e dificuldade em alguns procedimentos de grande escala. Parte das avaliações é antiga e menciona a marca anterior do produto, devendo ser interpretada com cautela.

O Gartner Peer Insights apresentava **4,6/5 em 224 avaliações** para o Blue Yonder Supply Chain Planning. Esse resultado se refere ao conjunto mais amplo de planejamento da cadeia de suprimentos, e não apenas ao módulo de previsão. As opiniões públicas ajudam a identificar padrões percebidos, mas não substituem um teste de usabilidade com o público do projeto.

#### Preço/modelo de negócio

O Blue Yonder opera como plataforma SaaS corporativa. O fabricante não divulga um preço fixo nas páginas consultadas e direciona o interessado ao contato comercial. O valor tende a depender dos módulos, integrações, quantidade de usuários e escala de implantação. Esse modelo reforça seu posicionamento corporativo e dificulta a adoção por pequenos negócios.

#### Padrões e tendências percebidos

- Visão inicial orientada a riscos, oportunidades e indicadores relevantes.
- Explicação dos fatores que influenciam a previsão para aumentar confiança.
- Automação de tarefas repetitivas com manutenção do controle humano.
- Uso de detalhamento progressivo: primeiro o resumo, depois causas e dados.
- Integração entre planejamento de demanda, oferta e execução.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Alertas são associados a contexto e indicadores | Imagem oficial de experiência e descrição de recomendações acionáveis | Mostrar risco, impacto e próxima ação na mesma sequência |
| A previsão pode apresentar seus fatores | Descrição oficial da abordagem *glass box* | Explicar a recomendação em linguagem simples, sem expor complexidade técnica desnecessária |
| A plataforma possui grande amplitude funcional | Vários módulos, dimensões e fluxos de planejamento descritos pelo fabricante | Evitar reproduzir a densidade de uma plataforma corporativa; manter apenas o necessário para reposição |
| O aprendizado pode exigir treinamento | Relatos públicos no G2 | Usar terminologia cotidiana, ajuda contextual e fluxo curto |
| Preço e implantação não são transparentes ao pequeno negócio | Ausência de preço fixo e direcionamento ao contato comercial | Priorizar ferramentas abertas, baixo custo operacional e configuração simples |

### Análise C02 — Netstock

**Autor(a):** Victor Merker Binda  
**Tipo:** indireto / análogo  
**Link oficial:** https://www.netstock.com/solutions/inventory-optimization/  
**Data de acesso:** 02/09/2026

#### Contexto e proposta

O Netstock é uma plataforma SaaS de previsão de demanda, otimização de estoque e reposição integrada a sistemas ERP. A solução reúne indicadores em painéis, classifica itens por importância e risco, calcula estoque de segurança e gera pedidos recomendados. Seu princípio de “gestão por exceção” procura mostrar primeiro os itens que exigem atenção, em vez de obrigar o usuário a verificar todo o catálogo.

Entre os dois produtos analisados, o Netstock é o mais próximo da proposta do TCC porque atende pequenas e médias empresas e aproxima previsão, risco e decisão de compra. Ainda assim, é uma solução proprietária, voltada ao mercado internacional e normalmente dependente de integração com um sistema de gestão.

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| Painel de exceções | Resume indicadores e prioriza produtos com risco de ruptura, excesso ou outros desvios | [`assets/02_concorrencia/netstock_interface.png`](assets/02_concorrencia/netstock_interface.png) | Direciona a atenção, mas o motivo da prioridade precisa estar explícito |
| Classificação de produtos | Agrupa itens por valor de vendas, velocidade e perfil de risco | [Página oficial de Inventory Optimization](https://www.netstock.com/solutions/inventory-optimization/) | A classificação facilita a priorização, desde que siglas e categorias tenham explicação |
| Previsão de demanda | Gera previsões por produto, grupo, canal ou cliente, considerando tendências e sazonalidade | [Página oficial de Inventory Optimization](https://www.netstock.com/solutions/inventory-optimization/) | A previsão deve ser comparável às vendas realizadas e apresentada em linguagem operacional |
| Estoque de segurança | Calcula proteção contra riscos de oferta e demanda e considera o nível de serviço desejado | [Página oficial de Inventory Optimization](https://www.netstock.com/solutions/inventory-optimization/) | O valor precisa ter explicação, parâmetros visíveis e possibilidade de conferência |
| Reposição recomendada | Calcula e prioriza pedidos conforme previsão, política de estoque e prazo de entrega | [Página oficial de Inventory Ordering](https://www.netstock.com/solutions/inventory-ordering/) | A quantidade sugerida deve ficar próxima do produto e exigir confirmação antes do registro |
| Integração com ERP | Processa dados do sistema de gestão e pode devolver pedidos ou recomendações | [Página oficial de Inventory Optimization](https://www.netstock.com/solutions/inventory-optimization/) | O projeto não deve tornar um ERP obrigatório, pois parte do público pode depender de cadastro próprio ou planilha |


#### Experiência do usuário e opiniões

Na data da consulta, o Capterra apresentava nota geral de **4,8/5 em 75 avaliações**, com **4,7/5 em facilidade de uso**. Usuários destacavam a interface intuitiva, a visibilidade dos níveis de estoque, a identificação rápida de problemas e o apoio à reposição. Entre as limitações relatadas estavam o esforço inicial de configuração, a dependência da qualidade dos dados e restrições de personalização em relatórios e painéis. Algumas avaliações foram incentivadas ou encaminhadas pelo fornecedor, aspecto que deve ser considerado na interpretação.

No G2, o Netstock apresentava **4,6/5 em 171 avaliações**. A síntese pública destacava facilidade de uso e transformação de dados complexos em informações acionáveis, mas também registrava pedidos por maior flexibilidade de relatórios e funcionalidades.

#### Preço/modelo de negócio

O Netstock funciona como plataforma SaaS proprietária e oferece diferentes pacotes. O site apresenta a opção “Get Pricing”, mas não exibe um valor único nas páginas analisadas. O custo depende do pacote e do contexto da organização. Assim, embora o produto esteja mais próximo de pequenas e médias empresas do que o Blue Yonder, as fontes públicas não permitem concluir que seja financeiramente acessível ao microempreendedor brasileiro.

#### Padrões e tendências percebidos

- Gestão por exceção, priorizando produtos que exigem ação.
- Painel com indicadores operacionais e financeiros de estoque.
- Navegação do resumo geral para detalhes do produto e do pedido.
- Recomendação prescritiva, informando o que e quanto repor.
- Integração entre dados do ERP, previsão e geração de pedidos.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| O painel prioriza problemas de estoque | Imagem e descrição oficial do *Executive Dashboard* | Organizar a tela inicial por risco, evitando exigir revisão manual de todos os produtos |
| A recomendação é aproximada da ação de compra | Descrição oficial de pedidos recomendados | Levar o usuário do alerta ao produto e à confirmação da reposição em poucos passos |
| A interface é considerada intuitiva por parte dos usuários | Avaliações públicas no Capterra e G2 | Manter hierarquia clara, indicadores resumidos e detalhamento progressivo |
| Configuração e qualidade dos dados afetam a experiência | Limitações recorrentes relatadas nas avaliações | Validar entradas e avisar quando o histórico for insuficiente ou inconsistente |
| Relatórios podem ter personalização limitada | Relatos públicos no Capterra e G2 | Oferecer filtros essenciais sem criar um construtor complexo de relatórios |
| A integração com ERP é central ao produto | Descrição oficial da plataforma | Disponibilizar cadastro e importação simples para usuários sem ERP |

## 3. Softwares que o público-alvo usa no cotidiano

Analise interfaces que moldam a expectativa do público, mesmo que não sejam concorrentes.

| Software | Por que o público usa | Padrões relevantes | Prints | O que aprender |
|---|---|---|---|---|
| Planilha eletrônica | Registrar produtos, compras, vendas e contagens de estoque | Tabela, linha e coluna, ordenação, filtros e importação de arquivo | Não coletado; uso ainda deve ser validado com o público | Oferecer importação simples e apresentar listas em uma estrutura familiar |
| Sistema de vendas/PDV | Registrar vendas, localizar produtos e atualizar o saldo | Busca por produto, código, quantidade e confirmação da operação | Não coletado; depende do sistema utilizado por cada participante | Reduzir digitação, manter busca visível e confirmar alterações importantes |
| Aplicativo de mensagens | Comunicar faltas, pedidos e informações a funcionários ou fornecedores | Avisos curtos, indicador de pendência e acesso direto à conversa | Não coletado; uso ainda deve ser validado com o público | Escrever alertas curtos, indicar urgência e deixar a próxima ação evidente |

## 3.1 Padrões de interface relevantes ao escopo de IHC

Registre somente padrões encontrados nas soluções analisadas e que possam ter relação com objetivos reais da equipe.

| Padrão observado | Produto(s) | Para qual tarefa serve | Vantagem percebida | Risco/limitação | Aplicável ao nosso escopo? |
|---|---|---|---|---|---|
| dashboard | Blue Yonder e Netstock | Identificar riscos e acompanhar indicadores | Reúne o estado geral e direciona a atenção | Muitos indicadores podem esconder o que exige ação | sim, com poucos indicadores operacionais |
| relatório | Netstock | Conferir estoque, pedidos e desempenho | Permite aprofundar a análise sem sobrecarregar a visão inicial | Relatórios extensos ou rígidos dificultam a interpretação | sim, limitado às informações necessárias à reposição |
| histórico + filtros | Blue Yonder e Netstock | Analisar produto, local e período | Facilita localizar dados e comparar comportamentos | Excesso de filtros aumenta a carga cognitiva | sim, com produto, categoria, risco e período |
| administração/CRUD | Não confirmado nas telas públicas analisadas | Manter produtos, vendas e parâmetros | Evita dependência de intervenção técnica | Cadastro longo ou técnico pode afastar o usuário | sim, somente para dados essenciais do projeto |
| comparação de resultados | Blue Yonder e Netstock | Comparar demanda prevista, realizada e cenários | Ajuda a compreender variações e avaliar recomendações | Comparações sem período ou legenda podem induzir a erro | sim |
| alerta acionável | Blue Yonder e Netstock | Identificar um risco e decidir a próxima ação | Aproxima informação, explicação e decisão | Automação sem confirmação pode causar compra incorreta | sim, com explicação e confirmação humana |

> O objetivo não é concluir “todo concorrente tem dashboard, então teremos um”. O padrão só será adotado se apoiar uma tarefa rastreável.

## 4. Síntese comparativa da equipe

| Critério | C01 — Blue Yonder | C02 — Netstock | Oportunidade para o projeto |
|---|---|---|---|
| Navegação | Plataforma ampla, multidimensional e voltada a diferentes papéis | Painéis focados em indicadores, exceções e pedidos | Criar fluxo curto: risco → detalhe → decisão |
| Feedback/estado | Expõe fatores da demanda, riscos, oportunidades e indicadores | Mostra classificação, situação do estoque e pedidos recomendados | Informar motivo do risco, período analisado e data de atualização |
| Prevenção/recuperação de erro | A transparência favorece a conferência, mas a complexidade exige treinamento | As recomendações dependem de configuração e dados corretos | Validar entradas, sinalizar histórico insuficiente e pedir confirmação antes da reposição |
| Terminologia | Técnica e corporativa | Mais operacional, mas ainda utiliza métricas de planejamento | Usar linguagem cotidiana e explicar termos sob demanda |
| Acessibilidade | O fabricante declara acessibilidade como princípio, mas a conformidade específica não foi verificada | Não foi encontrada comprovação suficiente nas páginas analisadas | Não depender somente de cor; combinar texto, ícone, contraste e ordem de prioridade |
| Eficiência | Automatiza análises, cenários e recomendações em escala corporativa | Aplica gestão por exceção e prioriza pedidos | Mostrar primeiro poucos alertas acionáveis e oferecer busca simples |

## 5. Recomendações derivadas

Liste recomendações com origem explícita.

- **RC01:** Organizar a navegação no fluxo visão de riscos → detalhe do produto e da previsão → decisão de reposição — derivada de C01/C02.
- **RC02:** Exibir saldo atual, demanda prevista, período analisado, data de atualização e quantidade recomendada — derivada de C01/C02.
- **RC03:** Explicar cada alerta no formato “o que ocorreu, por que importa e qual ação é sugerida” — derivada de C01.
- **RC04:** Priorizar produtos por risco de ruptura ou excesso, aplicando gestão por exceção — derivada de C02.
- **RC05:** Permitir comparar vendas realizadas e previstas e consultar os principais fatores considerados — derivada de C01/C02.
- **RC06:** Oferecer poucos filtros úteis, como risco, produto, categoria e período — derivada de C01/C02.
- **RC07:** Traduzir métricas técnicas para linguagem comercial e fornecer explicações adicionais sob demanda — derivada de C01/C02 e do perfil do público.
- **RC08:** Validar os dados de entrada, avisar quando o histórico for insuficiente e não apresentar a previsão como certeza — derivada das avaliações de C01/C02.
- **RC09:** Exigir confirmação antes de registrar uma reposição e permitir revisar a quantidade sugerida — derivada de C02.
- **RC10:** Combinar cor com texto, ícone e prioridade para comunicar estados — derivada da análise de acessibilidade de C01/C02.
- **RC11:** Permitir cadastro próprio e importação simples, sem tornar um ERP obrigatório — derivada da limitação identificada em C02.
- **RC12:** Manter apenas as informações necessárias à decisão do pequeno comerciante — derivada da diferença de escala entre C01 e o público do projeto.

## Referências

- BLUE YONDER. [Demand Planning](https://blueyonder.com/solutions/supply-chain-planning/demand-planning). Acesso em: 02 set. 2026.
- BLUE YONDER. [User Experience Strategy](https://blueyonder.com/why-blue-yonder/user-experience). Acesso em: 02 set. 2026.
- G2. [Blue Yonder Demand Planning Reviews](https://www.g2.com/products/blue-yonder-demand-planning/reviews). Acesso em: 02 set. 2026.
- GARTNER PEER INSIGHTS. [Blue Yonder Supply Chain Planning Reviews and Ratings](https://www.gartner.com/reviews/market/supply-chain-planning-solutions/vendor/blue-yonder/product/blue-yonder-supply-chain-planning/likes-dislikes). Acesso em: 02 set. 2026.
- NETSTOCK. [Inventory Optimization](https://www.netstock.com/solutions/inventory-optimization/). Acesso em: 02 set. 2026.
- NETSTOCK. [Executive Dashboard](https://www.netstock.com/executive-dashboard/). Acesso em: 02 set. 2026.
- NETSTOCK. [Inventory Ordering](https://www.netstock.com/solutions/inventory-ordering/). Acesso em: 02 set. 2026.
- CAPTERRA. [Netstock Software Reviews](https://www.capterra.com/p/152724/NETSTOCK/). Acesso em: 02 set. 2026.
- G2. [Netstock Reviews](https://www.g2.com/products/netstock/reviews). Acesso em: 02 set. 2026.

---

# Checklist
- [ ] O mapa inicial de alternativas da Entrega 1 foi revisitado e aprofundado.
- [ ] Hipóteses relevantes sobre mercado/padrões foram atualizadas na rastreabilidade quando surgiram evidências.
- [ ] Há pelo menos uma análise completa por integrante.
- [ ] Cada análise contém prints legíveis da interface.
- [ ] Prints mostram telas/estados relevantes, não apenas logos/homepage.
- [ ] Foram analisados concorrentes e/ou interfaces representativas ao público.
- [ ] Em TCC sem interface original, foram investigadas ferramentas profissionais análogas às atividades do usuário escolhido.
- [ ] Padrões como dashboard, relatório, filtros e CRUD foram analisados como soluções para tarefas, não como requisitos automáticos.
- [ ] Opiniões de UX têm fonte.
- [ ] A síntese compara critérios comuns e produz recomendações.
- [ ] Não há “copiar porque o concorrente faz”; há justificativa de adequação ao público/contexto.


