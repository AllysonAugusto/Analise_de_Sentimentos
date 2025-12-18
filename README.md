# Análise de Sentimentos em Avaliações de Produtos
Amazon e Mercado Livre

## Visão Geral
Este projeto realiza uma análise de sentimentos em avaliações de produtos
coletadas das plataformas Amazon e Mercado Livre, utilizando técnicas de
Processamento de Linguagem Natural (PLN).

## Objetivo
Classificar avaliações textuais como **positivas** ou **negativas** e extrair
insights de negócio, como:
- percentual de avaliações negativas por plataforma
- produtos com maior volume de críticas
- palavras mais frequentes em avaliações negativas

## Dataset
- Total de avaliações: **69.749**
- Fontes:
  - Amazon (`data/amazon.csv`)
  - Mercado Livre (`data/mercado_livre.csv`)

## Metodologia
1. Limpeza e normalização do texto
2. Rotulagem automática usando **SentiLex-PT**
3. Aplicação de regras linguísticas (negação e intensificadores)
4. Treinamento de modelo supervisionado:
   - TF-IDF
   - Regressão Logística

## Resultados
- Acurácia do modelo: **~97%**
- Maior volume de avaliações negativas concentrado em poucos produtos
- Diferença clara de padrão de reclamação entre plataformas

## Como Executar
```bash
pip install -r requirements.txt
```