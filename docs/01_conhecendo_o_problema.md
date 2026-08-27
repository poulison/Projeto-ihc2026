# Entrega 1 — Conhecendo o projeto, o usuário e o problema

**Data:** 19/08/2026

**Status:** 🟨 em andamento

**Responsabilidade:** 1 solução consolidada por equipe

As respostas usam **[F]** para fatos, **[H]** para hipóteses e **[?]** para informações que ainda precisamos descobrir.

---

# 0. Identificação do TCC e da equipe

## 0.1 Membros

| Nome completo | Matrícula | GitHub |
|---|---:|---|
| Paulo Andre de Oliveira Hirata | 22.125.072-3 | @poulison |
| Victor Merker Binda | **[?] A preencher** | @victorrbb |

## 0.2 Título atual do TCC

**Previsão de estoque usando machine learning**

## 0.3 Orientador

**Fagner de Assis Moura Pimentel**

## 0.4 Resultado principal previsto

- [x] sistema/aplicação interativa;
- [x] modelo de IA/ML;
- [x] estudo comparativo/avaliação experimental.

**Descrição:** [F] Sistema que utiliza o histórico do estoque para prever demanda e comparar modelos de aprendizado de máquina.

## 0.5 O TCC já previa interface?

- [x] Sim, a interface já faz parte do TCC.

[F] O README prevê um sistema com interface. [?] Os fluxos obrigatórios e as tecnologias ainda serão confirmados com o orientador.

---

# 1. Entendendo a contribuição do projeto

## 1.1 TCC em uma frase

O TCC busca prever a demanda usando o histórico do estoque para ajudar pequenos comércios a planejar reposições.

## 1.2 Problema que motivou o TCC

[F] Um dos integrantes observou situações de ruptura de estoque na loja de sua família. **Fonte:** relato da equipe.

## 1.3 Contribuição central

[F] Analisar movimentações do estoque, gerar previsões de demanda e comparar modelos para entender qual apresenta melhor resultado no contexto estudado.

## 1.4 Mudança esperada

[H] **H01 —** As previsões podem ajudar o responsável a antecipar reposições e reduzir faltas e excessos.

[H] **H02 —** Uma interface simples pode tornar esse tipo de análise acessível a gestores sem conhecimento de ML.

## 1.5 Mérito técnico e aplicação

| Contribuição técnica | Aplicação prática possível |
|---|---|
| Construir e comparar modelos de previsão | Apoiar o planejamento de compras |
| Avaliar o desempenho dos modelos | Escolher previsões mais adequadas ao contexto |

---

# 2. Pessoas envolvidas

## 2.1 Usuário direto

[H] **H03 —** O usuário principal será o responsável pelo estoque de um pequeno comércio, que consultará previsões e planejará reposições.

## 2.2 Perfis e responsabilidades

| Perfil | O que faria | Status |
|---|---|---|
| Responsável pelo estoque | Consulta produtos, previsões e planeja reposições | [H] H03 |
| Proprietário/gerente | Aprova compras e acompanha resultados | [H] |
| Funcionário de vendas | Registra movimentações e informa divergências | [H] |
| Equipe do TCC | Desenvolve e avalia os modelos | [F] |

## 2.3 Pessoas afetadas sem uso direto

| Stakeholder | Como é afetado | Usa a interface? |
|---|---|---:|
| Clientes | Podem encontrar ou não o produto desejado | Não |
| Fornecedores | Recebem os pedidos de reposição | Não |
| Funcionários | Lidam com faltas e reclamações | Talvez |

## 2.4 Características relevantes

[H] **H04 —** O usuário conhece produtos e fornecedores, mas pode não entender métricas de ML. A interface deve usar linguagem comercial e explicar as previsões.

[?] Ainda precisamos conhecer sua experiência tecnológica e necessidades de acessibilidade.

---

# 3. Objetivos e atividades

## 3.1 Objetivo do usuário

[H] Evitar a falta de produtos sem comprar mais do que o necessário.

## 3.2 Atividades importantes

| ID | Atividade | Quem realiza | Frequência/criticidade | Status |
|---|---|---|---|---|
| A01 | Acompanhar o estoque | Responsável | Frequente/alta | [H] |
| A02 | Identificar risco de falta ou excesso | Responsável | Frequente/alta | [H] H01 |
| A03 | Planejar reposições | Responsável/gerente | Periódica/crítica | [H] H01 |
| A04 | Conferir a previsão antes de decidir | Responsável | Periódica/crítica | [H] H04 |

## 3.3 Atividade mais frequente

[H] A01, pois vendas, entradas e ajustes mudam o saldo do estoque constantemente.

## 3.4 Atividade mais crítica

[H] A03. Comprar pouco pode causar ruptura; comprar demais ocupa espaço e imobiliza dinheiro.

---

# 4. Problema e processo atual

## 4.1 Como é feito hoje?

[F] A equipe já observou uma ruptura na loja. [?] Ainda não sabemos se o controle atual usa sistema, planilha, papel ou contagem manual.

## 4.2 Principais dificuldades

[H] **H05 —** Consolidar movimentações e perceber tendências manualmente pode ser demorado e sujeito a erros.

## 4.3 Informações necessárias

[H] Saldo atual, vendas anteriores, entradas previstas, prazo do fornecedor, demanda prevista, estoque mínimo e custo do produto.

## 4.4 Consequências de erro

[H] Uma estimativa baixa pode causar falta e perda de vendas; uma estimativa alta pode gerar excesso e desperdício.

## 4.5 Situação concreta

[F/H] Um cliente procura um produto na loja da família de um integrante, mas o item acabou antes da reposição. A ruptura foi observada, porém sua causa ainda não foi identificada. O cliente precisa escolher outra opção ou sair sem comprar.

## 4.6 Evidências atuais

| Fonte | O que sustenta | Limitação |
|---|---|---|
| Relato da equipe | Existência da ruptura | Não informa frequência ou causa |
| README e título do TCC | Previsão com ML e sistema com interface | Fluxos ainda pouco definidos |
| [Sebrae](https://sebrae.com.br/Sebrae/Portal%20Sebrae/UFs/PE/Anexos/-controles-financeiros-.pdf) | Importância de evitar falta e excesso | Fonte geral |

---

# 5. Contexto de uso

## 5.1 Onde e quando?

[H] Na loja, durante a conferência do estoque ou o planejamento de pedidos.

## 5.2 Dispositivos

[H] Computador ou notebook; celular para consultas rápidas. [?] Precisamos verificar os equipamentos disponíveis.

## 5.3 Condições físicas

[H] O uso pode acontecer com ruído, interrupções e pressão de tempo.

## 5.4 Fatores organizacionais

[H] Funcionários podem registrar movimentações, enquanto gerente ou proprietário aprova compras.

## 5.5 Histórico e rastreabilidade

[H] **H06 —** O usuário pode precisar rever previsões anteriores e comparar o previsto com o realizado.

## 5.6 Consequências de erro

[H] Dados incorretos podem gerar previsões ruins e decisões de compra inadequadas.

---

# 6. Mercado e alternativas

## 6.1 Alternativas atuais

| Alternativa | Uso | Status |
|---|---|---|
| Planilhas/anotações | Registrar e conferir saldos | [H] para a loja estudada |
| Experiência do responsável | Estimar procura e compras | [H] |
| Odoo Inventory | Controle, previsão e reposição | [F] documentação oficial |
| Zoho Inventory | Dashboard, relatórios e reposição | [F] documentação oficial |

## 6.2 Produtos da mesma área

[F] O [Odoo Inventory](https://www.odoo.com/app/inventory-features) oferece previsão e reposição. O [Zoho Inventory](https://www.zoho.com/us/inventory/help/reports/inventory-reports.html) oferece dashboard e relatórios de estoque.

## 6.3 Interfaces conhecidas

[H] Planilhas, sistemas de vendas e painéis administrativos podem ser familiares. [?] Isso será validado com o público.

## 6.4 Pontos positivos

[F] As soluções encontradas organizam saldos, movimentações, filtros, alertas e relatórios.

## 6.5 Limitações

[H] Sistemas muito amplos podem ser difíceis de configurar e apresentar informações demais para pequenos comerciantes.

## 6.6 Padrões familiares

[H] Busca, filtros, tabelas de produtos, saldo, entradas, saídas e alertas de estoque baixo.

---

# 7. Escopo de IHC

## 7.1 Caminho escolhido

**Caminho A — o TCC já possui interface.**

O recorte será identificar risco de falta ou excesso, entender a previsão e planejar uma reposição. Não pretendemos criar um ERP completo.

## 7.2 Perfil priorizado

**Responsável pelo estoque de um pequeno comércio**, pois é quem transforma a previsão em decisão de reposição.

## 7.3 Objetivo priorizado

Decidir o que repor, em qual quantidade e em qual momento.

## 7.4 Interface explorada

> Para fins da disciplina de IHC, será projetada uma interface que permita ao responsável pelo estoque usar previsões de demanda para identificar riscos e planejar reposições na rotina de um pequeno comércio.

## 7.5 Relação com o TCC

- [x] A interface já fazia parte do TCC.
- [x] O recorte é um aprofundamento de IHC.

Os detalhes projetados só entrarão no TCC após decisão da equipe e do orientador.

---

# 8. Possibilidades de interação

| Possibilidade | Faz sentido? | Justificativa |
|---|---|---|
| Visão geral/alertas | Sim | Identificar produtos que exigem atenção |
| Entrada de dados | Sim | Fornecer o histórico para a previsão |
| Relatório de previsão | Sim | Entender o resultado antes de decidir |
| Histórico e filtros | Sim | Rever produtos, períodos e previsões |
| Explicação do resultado | Sim | Evitar interpretação incorreta |
| Cadastro de produtos | Talvez | Manter apenas dados essenciais |
| Usuários e permissões | Talvez | Depende da divisão real de responsabilidades |
| Administração completa | Não | Está fora do recorte inicial |

---

# 9. Benefícios e ações iniciais

## 9.1 Benefícios

| Benefício | Necessidade | Usuário | Status |
|---|---|---|---|
| Antecipar rupturas | Evitar falta de produtos | Responsável | [H] H01 |
| Facilitar a interpretação do histórico | Reduzir esforço manual | Responsável | [H] H05 |
| Explicar previsões | Apoiar quem não conhece ML | Responsável | [H] H02/H04 |

## 9.2 Ações necessárias

| ID | O usuário precisa conseguir... | Prioridade |
|---|---|---|
| F01 | Ver produtos com risco de falta ou excesso | Alta |
| F02 | Consultar saldo, histórico e previsão | Alta |
| F03 | Buscar e filtrar produtos | Alta |
| F04 | Revisar dados e avisos antes de decidir | Alta |
| F05 | Registrar uma decisão de reposição | Alta |
| F06 | Comparar previsão e demanda realizada | Média |

## 9.3 Tecnologias e restrições

| Item | Motivo | Impacto na interação |
|---|---|---|
| Aprendizado de máquina | Parte central do TCC | Explicar incerteza e limites |
| Histórico do estoque | Entrada da previsão | Validar dados ausentes ou incorretos |
| Comparação de modelos | Mérito técnico | Não sobrecarregar o gestor com métricas |

---

# 10. Hipóteses e dúvidas prioritárias

| ID | Hipótese/dúvida | Como investigar |
|---|---|---|
| H01 | Previsões ajudarão a antecipar reposições | Entrevista e teste de conceito |
| H02 | Gestores sem formação em ML entenderão os resultados | Teste com usuários |
| H03 | O responsável pelo estoque é o usuário prioritário | Entrevista/persona |
| H04 | O usuário conhece o negócio, mas não métricas de ML | Entrevista |
| H05 | O processo manual é trabalhoso e sujeito a erros | Observação/entrevista |
| H06 | Histórico de previsões é necessário | Entrevista e análise de tarefas |
| Q01 | Como a loja controla o estoque e quais dados possui? | Observação/entrevista |
| Q02 | Quais fluxos são obrigatórios no TCC? | Reunião com o orientador |

As hipóteses também estão em [RASTREABILIDADE.md](../RASTREABILIDADE.md).

---

# 11. Síntese da equipe

| Pergunta | Resposta atual |
|---|---|
| Contribuição do TCC | Prever demanda e comparar modelos usando o histórico do estoque |
| O TCC previa interface? | Sim |
| Usuário prioritário | Responsável pelo estoque de pequeno comércio |
| Objetivo | Evitar falta e excesso ao planejar reposições |
| Processo atual | Ainda precisa ser investigado |
| Contexto | Conferência e compra de mercadorias na loja |
| Recorte de IHC | Risco → previsão → decisão de reposição |
| Relação com o TCC | Interface prevista, aprofundada pela disciplina |
| Hipóteses principais | H01 a H06; dúvidas Q01 e Q02 |

**Dentro do escopo de IHC:** consulta, interpretação da previsão e planejamento de reposição.

**Fora do escopo:** ERP completo, emissão fiscal, pagamentos, logística e compra automática.

**Implementação no TCC:** ainda não definida; será discutida com o orientador.

---

# 12. Próximas entregas

As próximas etapas irão validar o público e o processo atual, detalhar tarefas, criar o protótipo e avaliar a interface. Esta entrega poderá ser revisada quando novas evidências aparecerem.

---

# 13. Comunicação do projeto

1. **Problema:** pequenos comércios precisam evitar falta e excesso de produtos.
2. **Contribuição:** o TCC compara modelos que preveem demanda usando o histórico do estoque.
3. **Forma de uso:** o responsável consulta riscos e previsões para planejar compras.

---

# Checklist

- [x] TCC e escopo de IHC estão diferenciados.
- [x] Usuário, objetivo, problema e contexto foram definidos.
- [x] Fatos, hipóteses e dúvidas foram identificados.
- [x] Mercado e alternativas foram levantados inicialmente.
- [x] O recorte é viável para o semestre.

## Pendências

- [?] Matrícula de Victor Merker Binda.
- [?] Processo atual de controle da loja.
- [?] Confirmação do escopo formal com o orientador.
