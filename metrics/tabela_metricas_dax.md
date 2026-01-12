# 📊 Tabela de Métricas DAX

Este projeto utiliza um modelo tabular com as seguintes entidades:

## 🟦 Fato_Respostas
- DATA
- LOCAL
- ORIGEM
- ∑ VOL. ENTRADA
- ∑ VOL. RESPOSTA

> Tabela de volumetria de respostas por canal e data.

## 🟨 Fato_Pesquisas
- ano
- Área
- Fonte
- Tipo
- Pilar
- BU
- BU Classificação
- ∑ Código
- ∑ Contagem

> Tabela principal de pesquisas de satisfação e categorização.

## 🟧 Medidas
- ∑ Column
- % Acumulado Por tipo Reclamado
- % BOOKING
- % Google
- % Hoteis
- % NPS
- % Por pilar
- Amplitude estatística
- Speech analytics para especificidades: Carne, Bolo, pão

> Métricas derivadas para análise de canais e tipos de reclamação.

## 🟩 Parâmetro
- Parâmetro
- Parâmetro Campos
- ∑ Parâmetro Pedido

> Tabela auxiliar para filtros e segmentações dinâmicas.

## 🟥 Desvio Padrão
- ∑ Column
- 90
- 95
- 99
- 99.5

> Tabela estatística para controle de variabilidade e alertas.

