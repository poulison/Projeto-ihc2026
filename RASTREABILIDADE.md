# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Previsão de estoque usando machine learning | Título do TCC e README | definido |
| Resultado técnico esperado | Sistema interativo com modelos de previsão e comparação experimental | README e Entrega 1 | definido; detalhes pendentes |
| O TCC previa interface? | Sim | README do projeto | definido |
| Capacidade/contribuição central | Analisar o histórico do estoque, prever demanda e comparar modelos | Entrega 1, seções 1.3 e 1.5 | definido |
| Possíveis beneficiários/stakeholders | Responsável pelo estoque, gerente, proprietário, clientes, funcionários e fornecedores | Relato da equipe e hipóteses H01/H03 | H |
| Usuário escolhido para IHC | Responsável pelo estoque de pequeno comércio | Perfil mais próximo da ruptura observada e da decisão de reposição | H — H03 |
| Objetivo principal do usuário | Antecipar reposições e equilibrar falta e excesso | Hipótese H01 | H |
| Contexto de uso adotado | Rotina de conferência e compra de mercadorias em pequeno comércio | Hipóteses de contexto da Entrega 1 | H |
| Interface/recorte de IHC | Consulta de risco, interpretação da previsão e planejamento de reposição | Deriva da capacidade do TCC e do problema de ruptura | proposta |
| Relação com o TCC | Parte prevista e aprofundamento de IHC | A interface já constava no escopo registrado, mas o recorte detalha seu uso | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Previsões e alertas ajudarão a antecipar reposições e reduzir faltas/excessos | H | Define o valor central da solução | Entregas 3, 4 e 7 | Entrega 2: Odoo e Zoho materializam previsão/reposição; avaliações públicas relatam apoio ao controle, mas não validam nosso público | refinada | Mantém o fluxo principal; exige teste com usuários |
| H02 | A análise preditiva pode ser apresentada de modo compreensível a gestores sem formação em ML | H | Orienta linguagem, explicações e visualizações | Entregas 2, 3 e 7 | Entrega 2: C01 explica composição do previsto e C02 usa indicadores familiares; compreensão de ML não foi testada | refinada | Adotar explicação progressiva e validar terminologia |
| H03 | O responsável pelo estoque é o usuário direto prioritário | H | Sustenta personas, tarefas e avaliação | Entrega 3 | PENDENTE | aberta | Define o público do projeto |
| H04 | O usuário conhece o domínio, mas não métricas de ML | H | Afeta vocabulário e prevenção de erros | Entregas 3, 7 e 8 | PENDENTE | aberta | Exige tradução da informação técnica |
| H05 | Consolidar dados e perceber tendências manualmente é trabalhoso e sujeito a falhas | H | Justifica alertas, busca e filtros | Entregas 3, 4 e 7 | Entrega 2: concorrentes consolidam saldo, movimentos, previsões e exceções; processo atual da loja segue desconhecido | refinada | Justifica investigar esforço atual antes de fechar requisitos |
| H06 | É necessário consultar histórico de previsões, decisões e resultados | H | Justifica rastreabilidade e avaliação de confiança | Entregas 3, 5 e 7 | PENDENTE | aberta | Pode gerar fluxo de histórico |
| Q01 | Como a loja controla estoque e quais dados históricos estão disponíveis? | ? | Determina integração, qualidade e viabilidade | Entregas 3 e 7 | PENDENTE | aberta | Pode alterar entrada de dados |
| Q02 | Quais fluxos e tecnologias são obrigatórios no escopo formal do TCC? | ? | Evita divergência entre TCC e IHC | Reunião com orientador | PENDENTE | aberta | Pode alterar a delimitação |

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | {{ex.: recomendação de otimização}} | {{...}} | {{P01}} | {{C01}} | {{T01}} | {{links}} | {{...}} | {{M01}} | {{F01...}} | {{V01 ou —}} | {{UT01}} | {{...}} |
| R02 |  |  |  |  |  |  |  |  |  |  |  |  |

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| F01 | Dashboard focado em exceções | A02 — identificar risco de falta/excesso | Produtos em risco, motivo e acesso ao detalhe | H01; C01 e C02 da Entrega 2 | RC01, RC03; demais artefatos PENDENTES |
| F02 | Histórico com busca e filtros | A01/A04 — acompanhar movimentos e conferir previsão | Produto, período, movimentos, previsto e realizado | H05/H06; C01 e C02 | RC02, RC04; demais artefatos PENDENTES |
| F03 | Detalhe/explicabilidade da previsão | A04 — compreender antes de decidir | Saldo, entradas, saídas, horizonte, confiança e limitações | H02/H04; Figura C01.2 | RC02, RC05; demais artefatos PENDENTES |
| F04 | Registro revisável de reposição | A03 — planejar reposição | Quantidade sugerida, justificativa, impacto e confirmação | H01; painel de reposição C01 | RC06; demais artefatos PENDENTES |
| F05 | Importação com validação | Atualizar movimentações | Arquivo, erros por linha/campo e correção | Q01; avaliações públicas de C02 | RC06; demais artefatos PENDENTES |

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
