# 🍔 Análise de Cancelamento em Delivery de Comida

## 📌 Visão Geral
Este projeto analisa **3.000 pedidos** de um aplicativo de delivery para identificar os fatores que mais influenciam o cancelamento de pedidos.

**Objetivo:** Entender o perfil dos pedidos cancelados e gerar insights acionáveis para o time operacional.

## 🔍 Principais Descobertas
| Insight | Conclusão |
|---------|-----------|
| ⏱️ **Tempo de espera** | Cancelados esperam **85 min** vs 75 min (entregues) |
| 💰 **Valor do pedido** | **Não influencia** cancelamento |
| 🕒 **Horário crítico** | **23h** tem maior taxa (28% de cancelamento) |
| 📊 **Feature mais importante** | Tempo de espera responde por **71%** do modelo |

## 🛠️ Ferramentas Utilizadas
- Python 3.9+
- Pandas (manipulação de dados)
- Matplotlib / Seaborn (visualizações)
- Scikit-learn (RandomForest, SMOTE)
- Imbalanced-learn (balanceamento de classes)

## 📊 Resultados do Modelo

### Sem balanceamento (escolhido)
- Acurácia: 67%
- Feature mais importante: tempo_espera_min

### Com balanceamento (SMOTE)
- Acurácia: 65%
- Conclusão: Balanceamento não trouxe ganho

## 📈 Visualizações
| Gráfico | O que mostra |
|---------|--------------|
| Boxplot tempo vs cancelado | Cancelados esperam mais |
| Heatmap de correlação | Tempo de espera é mais correlacionado |
| Feature importance | Tempo de espera = 71% da importância |

## ▶️ Como Reproduzir

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/analise-cancelamento-delivery.git
