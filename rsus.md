# Tributação sobre Restricted Stock Units no exterior

### Disclaimer: Não sou contador. Esse é um compilado de informações que achei na internet.


### Introdução


Algumas empresas ofereçam planos de remuneração atrelados a ações dessa empresa. Existem muitas maneiras de formatar esse plano:
- Restricted stock units
- Stock options
- Stock units

Cada plano oferece caracteristicas diferentes que podem impactar na tributação. Por exemplo, se o plano oferece risco financeiro ao funcionário, ele pode não ser categorizado como "salário" e sim "investimento" o que muda a tributação.

Nesse artigo falaremos de Restricted Stock Units que são oferecidas ao empregado como forma de retenção.
- O funcionário não paga nada para obter esse plano (sem risco financeiro)
- Existe um calendário indicando as datas em que as RSUs são convertidas em ações na posse do funcionário (vesting)
- A empresa considera as ações (na data do vestimento) na base de cálculo do FGTS e INSS

Essas caracteristicas indicam uma relação de natureza remuneratória (salário), portanto incidindo tributação da tabela progressiva de imposto de renda de pessoa física.

Em geral, o imposto de renda sobre pessoa fisica (IRPF) é recolhido na fonte (a empresa pagadora) e o funcionário só recebe o salário liquído. Entretanto, quando esse valor é pago no exterior, fica a cargo do empregado recolher o imposto de renda.


## Tributação no Recebimento

A tributação no recebimento dessas ações acontece apenas quando elas são disponibilizadas ao funcionário (vesting date ou release date), de acordo com o calendário do plano de RSUs.

A corretora emite uma nota indicando que X ações foram disponibilizadas na conta por um valor $Y de mercado.

O funcionário que recebe essas ações deve fazer o cálculo do imposto de renda devido, e pagar até o último dia útil do mês seguinte ao recebimento.

Exemplo: Se você recebeu ações no dia 20/10, tem até o dia 30/11 para pagar o imposto relativo a esse recebimento.

O imposto pode ser calculado utilizando a aplicação "Carnê-Leão" que pode ser baixada ou utilizar a versão Web disponibilizada no gov.br na aba de imposto de renda.

O primeiro passo é calcular o valor em reais recebido:
1. Converta o valor das ações para dólar utilizando a cotação informada pela corretora no recibo de "release".
2. Converta o valor em dólar para reais utilizando a cotação de compra último dia util da primeira quinzena do mês anterior ao recebimento. Essa cotação deve ser obtida no site do Banco Central.

Exemplo: Se voce recebeu ações no dia 22/01/2023, deve utilizar a cotação do dia 15/12/2022.

No carnê leão, informe um novo recebimento, vindo do exterior e indique o valor total em reais calculado acima. Na descrição informe onde estão localizadas as açoes, por qual preço em dolares e qual a cotação utilizada.
Feito isso para todos os recebimentos do mês, você pode gerar a DARF e pagar o imposto.

Durante a declaração anual é possivel importar os dados do carnê-leão.


## Declaração de bens e direitos

É importante declarar as ações como bens na declaração anual de renda. Ela deve conter os seguintes dados:
- Ticker da ação
- Bolsa em que ela é negociada
- Corretora + numero identificador
- Número de ações
- Preço médio de recebimento em reais. Atenção: Não coloque o valor de mercado.


### Cálculo do preço médio

A cada novo recebimento o preço médio por ação será alterado. Ele não se altera em vendas.

Ele pode ser calculado iterativamente por:

```
NA = Número de ações antes do recebimento de novas ações
PM = Preço médio antes do recebimento de novas ações

NR = Número de ações recebidas
VM = Valor de mercado de cada ação recebida
PM' = Preço médio após recebimento

PM' = (NA*PM + NR*VM) / (NA + NR)
```


## Tributação na Venda

Na venda dessa ações você poderá realizar um lucro ou prejuízo, alterando assim o valor total do seu patrimônio. Este eventual lucro deve ser tributado como "Ganho de capital".

O imposto sobre ganho de capital é de 15% sobre o lucro em vendas de até 5 milhões de reais.

É importante saber que se o total de vendas no mês foi menor que R$35.000,00, o lucro fica *isento de tributação*!

Para calcular o lucro, utilize o preço médio calculado anteriormente:

```
N = Número de ações vendidas
PV = Preço de venda
PM = Preço médio
Lucro = N*(PV - PM)
```

Para pagar o imposto sobre o lucro, você deve baixar o aplicativo "GCAP" (Ganho de CAPital).
Ele irá pedir os seguintes dados:


#### Aba Identificação / Aquisição
```
Onde o bem foi adquirido: Exterior
Data de aquisição: Utilize a data do primeiro recebimento de ações
Origem dos Rendimentos: Rendimentos auferidos em moeda nacional (isso porque foi fruto do trabalho no Brasil)
Cotação do dólar na data de aquisição: Aqui você deve colocar o dolár médio de aquisição. Para isso calcule o preço médio em dolares e divida o preço em reais pelo preço em dolar.
Custo de aquisição (U$): Preço médio vezes o número de ações vendidas
```


#### Aba Operação
```
Natureza: Alienação de Ações em Bolsa de Valores
Alienação a prazo: Não
Data de alienação: Data da venda
Cotação do dolar na data de alienação: Cotação de venda do dolar no dia da venda obtido no site to Banco Central.
```
Nessa aba haverá uma pergunta se o valor do conjunto de vendas no mês é maior que R$35.000,00 exatamente para que a receita zere o tributo caso seja menor.


Tendo registrado essas vendas do mês, é possivel gerar a DARF e pagar o imposto sobre o lucro.

Você pode utilizar (e me dar feedback) o site [https://brenoguim.github.io/stonks/lion.html](Lion) para fazer todos os cálculos de preço médio, preço médio de dolar.


## Regularizando atrasos

TBD
