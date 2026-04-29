# Laser Company Brasil — Plano do Projeto

## Visão Geral

Dashboard de tráfego pago para a Laser Company Brasil, desenvolvido para apresentar resultados de campanhas Meta Ads (Facebook/Instagram) de forma visual e profissional ao cliente.

---

## Objetivo

Substituir relatórios manuais por um dashboard interativo e atualizável, que o gestor de tráfego entrega ao cliente com um link. O cliente acessa pelo celular ou computador e visualiza os dados em tempo real.

---

## Campanhas Ativas

| Campanha | Grupo | Cor |
|---|---|---|
| QUANTA | Máquinas | Azul `#4f6af0` |
| ULTRACEL | Máquinas | Roxo `#7c3aed` |
| VYDENCE | Máquinas | Laranja `#f97316` |
| FRANQUIAS | Franquias | Verde `#059669` |

---

## Funcionalidades Entregues

### Dashboard (tela)
- [x] Header com nome da empresa e data do último lead
- [x] Tabs para filtrar: Todas as campanhas / Máquinas / Franquias
- [x] 5 cards de métricas: Total de Leads, Leads Hoje, Total Investido, Saldo Restante, CPL
- [x] Gráfico de barras por dia com datalabels (Chart.js)
- [x] Legenda interativa na aba Máquinas (clique para mostrar/ocultar campanha)
- [x] Upload de CSV ou XLSX exportado do Business Manager para atualizar dados
- [x] Notificações de sucesso/erro no upload

### PDF
- [x] Botão "Baixar em PDF" gera arquivo com 2 páginas A4 landscape
- [x] Página 1: Máquinas (QUANTA / ULTRACEL / VYDENCE)
- [x] Página 2: Franquias
- [x] Cada página tem: header, 5 cards e gráfico compacto

### Deploy
- [x] Repositório no GitHub
- [x] Publicado na Vercel com redeploy automático a cada push

---

## Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML + CSS + JS puro | Sem frameworks, arquivo único |
| Chart.js 4.4.0 | Gráfico de barras |
| chartjs-plugin-datalabels | Labels nas barras |
| SheetJS (xlsx) 0.18.5 | Leitura de arquivos Excel/CSV |
| html2pdf.js 0.10.1 | Geração do PDF |
| Inter (Google Fonts) | Tipografia |
| Vercel | Hospedagem estática |

---

## Links

| | |
|---|---|
| GitHub | https://github.com/OFerreira98/Trafego-laser-co-brasil |
| Dashboard ao vivo | https://trafego-laser-co-brasil.vercel.app/ |

---

## Como Atualizar os Dados

1. Exportar relatório de campanhas do Business Manager (CSV ou XLSX)
2. Acessar o dashboard no link da Vercel
3. Clicar em **Atualizar dados**
4. Selecionar o arquivo exportado
5. Os dados atualizam automaticamente na tela

> O arquivo deve ter colunas com: nome da campanha, valor gasto, leads e data.

---

## Próximos Passos (ideias)

- [ ] Conectar direto ao Google Sheets para atualização automática dos leads
- [ ] Adicionar período de datas com filtro por semana/mês
- [ ] Logo da Laser Company no header
- [ ] Envio automático do PDF por WhatsApp ou e-mail
