# 📊 Superstore Marketing Campaign

> **Objetivo:** Ajudar o time de marketing a obter maior resultado na próxima campanha, identificando o perfil dos clientes mais rentáveis e os padrões de aceitação.

---

## 📁 Sobre o Dataset

| | |
|---|---|
| **Arquivo** | `trab.xlsx` — aba `marketing_campaign` |
| **Registros** | 2.240 clientes |
| **Período** | Jul/2012 a Jun/2014 |
| **Colunas** | 29 variáveis (perfil, produtos, canais, campanhas) |
| **Valores nulos** | 24 em `Income` (1,07%) |

### Dicionário de Variáveis

**Perfil do Cliente**

| Coluna | Descrição |
|---|---|
| `ID` | Identificador único do cliente |
| `Year_Birth` | Ano de nascimento |
| `Education` | Nível de escolaridade |
| `Marital_Status` | Estado civil |
| `Income` | Renda anual familiar |
| `Kidhome` | Número de crianças em casa |
| `Teenhome` | Número de adolescentes em casa |
| `Dt_Customer` | Data de cadastro na empresa |

**Engajamento**

| Coluna | Descrição |
|---|---|
| `Recency` | Dias desde a última compra |
| `NumWebVisitsMonth` | Visitas ao site no último mês |

**Gasto por Produto (últimos 2 anos)**

| Coluna | Descrição |
|---|---|
| `MntWines` | Gasto em vinhos |
| `MntFruits` | Gasto em frutas |
| `MntMeatProducts` | Gasto em carnes |
| `MntFishProducts` | Gasto em pescados |
| `MntSweetProducts` | Gasto em doces |
| `MntGoldProds` | Gasto em produtos gold/premium |

**Canais de Compra**

| Coluna | Descrição |
|---|---|
| `NumDealsPurchases` | Compras via promoção/deal |
| `NumWebPurchases` | Compras pelo site |
| `NumCatalogPurchases` | Compras por catálogo |
| `NumStorePurchases` | Compras em loja física |

**Campanhas**

| Coluna | Descrição |
|---|---|
| `AcceptedCmp1` a `AcceptedCmp5` | 1 = aceitou a campanha, 0 = não aceitou |
| `Response` | Aceitação da campanha mais recente (variável-alvo) |
| `Complain` | 1 = fez reclamação nos últimos 2 anos |

---

## 🎯 Análise de Pareto

**Os 20% de clientes com maior gasto respondem por 52,2% da receita total ($1.356.988).**

Isso confirma o princípio de Pareto aplicado à base. A estratégia de marketing deve priorizar a retenção e upsell desse grupo antes de tentar adquirir novos clientes.

---

## 🔍 Principais Insights

### 1. Vinhos e Carnes dominam o faturamento

| Categoria | Total | % do Gasto |
|---|---|---|
| 🍷 Vinhos | $680.816 | 50,2% |
| 🥩 Carnes | $373.968 | 27,6% |
| 🥇 Gold | $98.609 | 7,3% |
| 🐟 Pescados | $84.057 | 6,2% |
| 🍬 Doces | $60.621 | 4,5% |
| 🍎 Frutas | $58.917 | 4,3% |

Apenas 2 categorias concentram **77,8% do faturamento** — outro Pareto dentro do mix de produtos.

---

### 2. Loja física lidera, mas Web cresce

| Canal | Compras | % do Total |
|---|---|---|
| 🏪 Loja Física | 12.970 | 39,0% |
| 🌐 Web | 9.150 | 27,5% |
| 📖 Catálogo | 5.963 | 17,9% |
| 🏷️ Deals/Promoção | 5.208 | 15,6% |

Clientes que visitam muito o site tendem a gastar menos (correlação = −0,50) — sinal de "vitrine virtual" sem conversão.

---


<img width="682" height="667" alt="Captura de tela 2026-05-19 172327" src="https://github.com/user-attachments/assets/823a279c-d047-4b2c-b036-463500ff8413" />

