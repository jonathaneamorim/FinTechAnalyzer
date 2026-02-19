# FinTechAnalyzer
Projeto para análise, controle e cálculo financeiro.

## Ideias
### Tela inicial - Gráficos (Principal)
- Criar um loading personalizado enquanto carrega as informações iniciais, e um load especifico para cada gráfico ainda não atualizado
- Indicador de quanto em quanto tempo o gráfico precisa ser atualizado (pegar a ultima atualização do gráfico), e salvar a ultima atualização do gráfico

- Monitoramento da Taxa Selic atual dinâmico. Salvar em cache para evitar reconsultas. Talvez fazer uma especie de objeto monitorador que guardará informações e atualizará automaticamente. (Selic muda a cada 45 dias (A taxa Selic é atualizada a cada 45 dias pelo Comitê de Política Monetária (Copom) do Banco Central.))
    - Selic atual + projeções (Focus, curva de juros)
    - CDI do dia
    - IPCA acumulado + expectativas futuras

- Monitoramento de Bolsas (Americana, Ibovespa, Chinesa, Russa, Europeia etc)
    - Bolsa (Ibovespa, mini-índices básicos)

- Monitoramento da inflação (IPCA e INPC), capturar dados de mês em mês. A sigla INPC corresponde ao Índice Nacional de Preços ao Consumidor. A sigla IPCA corresponde ao Índice Nacional de Preços ao Consumidor Amplo.
    - Inflação é o nome dado ao aumento dos preços de produtos e serviços. Ela é calculada pelos índices de preços, comumente chamados de índices de inflação.
    - O IPCA engloba uma parcela maior da população. Ele aponta a variação do custo de vida médio de famílias com renda mensal de 1 e 40 salários mínimos.
    - O INPC verifica a variação do custo de vida médio apenas de famílias com renda mensal de 1 a 5 salários mínimos. Esses grupos são mais sensíveis às variações de preços, pois tendem a gastar todo o seu rendimento em itens básicos, como alimentação, medicamentos, transporte etc.
    - Inflação aberta por grupo (Alimentos, Habitação etc.)

- Monitoramento do preço de moedas (Dolar, euro, Real, BTC, Etherium, Rublo, Yene e Yuan) - Comparativo com outras moedas (moeda padrão é o real).
    - Taxa de câmbio (USD/BRL e EUR/BRL)

- Curva DI futura (resumo)
- Previsões de inflação e juros para 12, 24 e 36 meses
- Cenários afetados
    - Preços de renda fixa
    - Descontos de títulos prefixados
    - Atratividade de IPCA+

- Monitor de renda fixa
- Comparador de CDBs:
    - CDB 100% CDI vs 110%, 120%, etc.
    - Melhores prazos e liquidez
    - Tributação automática


- Simulador de Tesouro Direto:
    - Prefixados vs IPCA+
    - Impacto da Selic em cada título
    - Marcação a mercado simulada

### Calculadoras
- Realizar calculos baseados nos dados capturados
- Calculo de juros compostos
- Calculos de rendimentos em CDB de acordo com o valor atual da selic ou valor personalizado
- Projeção de CDB vs Tesouro Selic vs fundo DI
- Simulador de IPCA no longo prazo
- Compensação de IR versus rentabilidade real
- Meta financeira: “quanto aportar para chegar em X em Y anos”
- Renda passiva futura com aportes mensais


## V2.0
### Alertas acionáveis
- “Selic alterada — veja impacto nos títulos prefixados”
- “IPCA divulgado — carteira real valorizou X%”
- “CDB acima de 115% CDI disponível em novos bancos”
- “Curva de juros sofreu inclinação forte — confira impacto na renda fixa longa”

### Gráficos comparativos
- Selic x IPCA (10 anos)
- CDI vs Poupança
- Prefixados vs IPCA+ no tempo
- Força do real vs dólar ao longo do tempo
- Inflação por categoria

### Se possivel
- Monitoramento de fundos de investimentos - https://developers.anbima.com.br/pt/ 

## V3.0
### Ferramentas de decisão
“Compro prefixado agora?”
Com base na curva atual.

“Trocar Tesouro Selic por CDB faz sentido?”
Comparação automática considerando liquidez e impostos.

Calculadora de aposentadoria real (descontada pela inflação)
Poucos apps fazem isso corretamente.


## Links
- https://dadosabertos.bcb.gov.br/dataset/dolar-americano-usd-todos-os-boletins-diarios
- https://dadosabertos.bcb.gov.br/dataset/?tags=indicadores+de+cr%C3%A9dito
- https://dadosabertos.bcb.gov.br/dataset/20716-taxa-media-de-juros-das-operacoes-de-credito---pessoas-fisicas---total
- https://openbanking-brasil.github.io/areadesenvolvedor/versions/v1.0.0-rc/index.html#introducao-extensibilidade
- https://www.bcb.gov.br/resultadobusca?termo=api&source=
- https://api.bcb.gov.br/dados/serie/bcdata.sgs.11/dados?formato=json&dataInicial=18/02/2016&dataFinal=18/02/2026
- https://dadosabertos.bcb.gov.br/dataset/11-taxa-de-juros---selic
- https://api.bcb.gov.br/dados/serie/bcdata.sgs.11/dados/ultimos/10?formato=json
- https://dadosabertos.bcb.gov.br/dataset/11-taxa-de-juros---selic/resource/b73edc07-bbac-430c-a2cb-b1639e605fa8#:~:text=Banco%20Central%20do%20Brasil%20*%20BCB/Demab.%20*%20Taxa%20de%20juros%20%2D%20Selic.%20*%20json_serie%2Dsgs%2D11. 
- https://economia.awesomeapi.com.br/last/USD-BRL,EUR-BRL,BTC-BRL
- https://awesomeapi.com.br/