[![AwesomeAPI](https://cdn.awesomeapi.com.br/awesomeapi/assets/awapi1c.png)](https://economia.awesomeapi.com.br/)

# API de Cotações
API de Cotações do Dólar (USD, USDT, CA, AUD), Euro, Libra, Peso, Iene, Franco, Yuan Chinês, Shekel Israelense, Litecoin, Bitcoin, Ethereum, Ripple, atualizado a cada 3 minutos.

### Veja toda a documentação em [https://docs.awesomeapi.com.br/](https://docs.awesomeapi.com.br/)

## Exemplo de uso
Retornar moedas selecionadas
```sh
$ curl https://economia.awesomeapi.com.br/json/all/USD-BRL,EUR-BRL
```
```js
{
    USD: {
        code: "USD",
        codein: "BRL",
        name: "Dólar Comercial",
        high: "3,8906",
        low: "3,8596",
        varBid: "-0,0138",
        pctChange: "-0,36",
        bid: "3,8660",
        ask: "3,8680",
        timestamp: "1555360069",
        create_date: "2019-04-15 17:27:50"
    },
    EUR: {
        code: "EUR",
        codein: "BRL",
        name: "Euro",
        high: "4,4006",
        low: "4,3628",
        varBid: "-0,0165",
        pctChange: "-0,38",
        bid: "4,3694",
        ask: "4,3720",
        timestamp: "1555360097",
        create_date: "2019-04-15 17:28:18"
    }
}
```

### Retorna todas as moedas
```sh
$ curl https://economia.awesomeapi.com.br/json/all
```
```js
{
    USD: {
        code: "USD",
        codein: "BRL",
        name: "Dólar Comercial",
        high: "3,8906",
        low: "3,8596",
        varBid: "-0,0138",
        pctChange: "-0,36",
        bid: "3,8660",
        ask: "3,8680",
        timestamp: "1555360069",
        create_date: "2019-04-15 17:27:50"
    },
    USDT: {
        high: "3.87",
        pctChange: "-0.741",
        bid: "3.71",
        ask: "4.02",
        timestamp: "1555358100000",
        name: "Dólar Turismo",
        low: "3.71",
        varBid: "-0.03",
        code: "USD",
        codein: "BRLT",
        create_date: "2019-04-15 17:27:00"
    },
    CAD: {
        code: "CAD",
        codein: "BRL",
        name: "Dólar Canadense",
        high: "2,9229",
        low: "2,8865",
        varBid: "-0,0204",
        pctChange: "-0,70",
        bid: "2,8909",
        ask: "2,8935",
        timestamp: "1555360097",
        create_date: "2019-04-15 17:28:19"
    },
    EUR: {
        code: "EUR",
        codein: "BRL",
        name: "Euro",
        high: "4,4006",
        low: "4,3628",
        varBid: "-0,0165",
        pctChange: "-0,38",
        bid: "4,3694",
        ask: "4,3720",
        timestamp: "1555360097",
        create_date: "2019-04-15 17:28:18"
    },
    GBP: {
        code: "GBP",
        codein: "BRL",
        name: "Libra Esterlina",
        high: "5,0991",
        low: "5,0554",
        varBid: "-0,0097",
        pctChange: "-0,19",
        bid: "5,0629",
        ask: "5,0659",
        timestamp: "1555360098",
        create_date: "2019-04-15 17:28:20"
    },
    ARS: {
        code: "ARS",
        codein: "BRL",
        name: "Peso Argentino",
        high: "0,0938",
        low: "0,0916",
        varBid: "0,0009",
        pctChange: "0,98",
        bid: "0,0928",
        ask: "0,0930",
        timestamp: "1555360069",
        create_date: "2019-04-15 17:27:50"
    },
    BTC: {
        code: "BTC",
        codein: "BRL",
        name: "Bitcoin",
        high: "20.400,0",
        low: "19.600,9",
        varBid: "-339,0",
        pctChange: "-1,68",
        bid: "19.729,0",
        ask: "19.850,0",
        timestamp: "1555360099",
        create_date: "2019-04-15 17:28:19"
    },
    LTC: {
        code: "LTC",
        codein: "BRL",
        name: "Litecoin",
        high: "337,39",
        low: "305,77",
        varBid: "-2,19",
        pctChange: "-0,70",
        bid: "309,17",
        ask: "311,98",
        timestamp: "1555360100",
        create_date: "2019-04-15 17:28:20"
    },
    JPY: {
        code: "JPY",
        codein: "BRL",
        name: "Iene Japonês",
        high: "0,03475",
        low: "0,03445",
        varBid: "-0,00010",
        pctChange: "-0,29",
        bid: "0,03451",
        ask: "0,03454",
        timestamp: "1555360102",
        create_date: "2019-04-15 17:28:22"
    },
    CHF: {
        code: "CHF",
        codein: "BRL",
        name: "Franco Suíço",
        high: "3,8788",
        low: "3,8438",
        varBid: "-0,0197",
        pctChange: "-0,51",
        bid: "3,8494",
        ask: "3,8526",
        timestamp: "1555360095",
        create_date: "2019-04-15 17:28:20"
    },
    AUD: {
        code: "AUD",
        codein: "BRL",
        name: "Dólar Australiano",
        high: "2,7925",
        low: "2,7695",
        varBid: "-0,0091",
        pctChange: "-0,33",
        bid: "2,7719",
        ask: "2,7741",
        timestamp: "1555360098",
        create_date: "2019-04-15 17:28:19"
    },
    CNY: {
        code: "CNY",
        codein: "BRL",
        name: "Yuan Chinês",
        high: "0,5800",
        low: "0,5755",
        varBid: "-0,0027",
        pctChange: "-0,46",
        bid: "0,5763",
        ask: "0,5766",
        timestamp: "1555360083",
        create_date: "2019-04-15 17:28:03"
    },
    ILS: {
        code: "ILS",
        codein: "BRL",
        name: "Novo Shekel Israelense",
        high: "1,0922",
        low: "1,0839",
        varBid: "-0,0015",
        pctChange: "-0,14",
        bid: "1,0865",
        ask: "1,0868",
        timestamp: "1555360025",
        create_date: "2019-04-15 17:27:05"
    }
}
```

> **Formatos suportados**
> - JSON
> - XML

### Legendas
Key | Tradução
-------- | ---
**bid** | Compra
**ask** | Venda
**varBid** | Variação
**pctChange** |  Porcentagem de Variação
**high** | Máximo
**low** | Mínimo
