# Laser Company Brasil — Dashboard de Tráfego Pago

Dashboard estático em HTML puro para acompanhamento de resultados de campanhas Meta Ads.

## Estrutura

```
Dashboard Forms ADS.html   → único arquivo do projeto; contém HTML, CSS e JS inline
```

## O que o dashboard faz

- Exibe métricas de 4 campanhas: QUANTA, ULTRACEL, VYDENCE e FRANQUIAS
- Tabs para filtrar por grupo (Todas / Máquinas / Franquias)
- Cards com: Total de Leads, Leads Hoje, Total Investido, Saldo Restante, CPL
- Gráfico de barras por dia (Chart.js + datalabels)
- Upload de CSV/XLSX do Business Manager para atualizar os dados
- Botão de PDF que gera 2 páginas A4 landscape: página 1 = Máquinas, página 2 = Franquias

## Deploy

- **GitHub:** https://github.com/OFerreira98/Trafego-laser-co-brasil
- **Vercel:** https://trafego-laser-co-brasil.vercel.app/

Push na branch `main` aciona redeploy automático na Vercel.

## Atualizar dados

Para atualizar investimento e leads basta clicar em **Atualizar dados** e importar o CSV exportado do Business Manager. O arquivo deve ter colunas reconhecíveis como: campanha, valor gasto, leads, data.

## Dependências (CDN, sem npm)

| Lib | Versão |
|---|---|
| Chart.js | 4.4.0 |
| chartjs-plugin-datalabels | 2.2.0 |
| xlsx (SheetJS) | 0.18.5 |
| html2pdf.js | 0.10.1 |
| Inter (Google Fonts) | — |
