[![AwesomeAPI](https://cdn.awesomeapi.com.br/awesomeapi/assets/awapi1c.png)](https://economia.awesomeapi.com.br/)

# API de Cotações
API de Cotações do Dólar (USD, USDT, CA, AUD), Euro, Libra, Peso, Iene, Franco, Yuan Chinês, Shekel Israelense, Litecoin, Bitcoin, Ethereum, Ripple, atualizado a cada 3 minutos.

### Veja toda a documentação em [https://docs.awesomeapi.com.br/](https://docs.awesomeapi.com.br/)

## Exemplo de uso
Retornar moedas selecionadas
```sh
$ curl https://economia.awesomeapi.com.br/json/all/USD-BRL,EUR-BRL
```
```json
{
    "USD": {
        "code": "USD",
        "codein": "BRL",
        "name": "Dólar Comercial",
        "high": "5.37",
        "low": "5.2257",
        "varBid": "-0.1351",
        "pctChange": "-2.52",
        "bid": "5.2279",
        "ask": "5.2285",
        "timestamp": "1591109752",
        "create_date": "2020-06-02 11:55:53"
    },
    "EUR": {
        "code": "EUR",
        "codein": "BRL",
        "name": "Euro",
        "high": "6.0046",
        "low": "5.844",
        "varBid": "-0.1235",
        "pctChange": "-2.07",
        "bid": "5.8462",
        "ask": "5.8497",
        "timestamp": "1591109753",
        "create_date": "2020-06-02 11:55:56"
    }
}
```

### Retorna todas as moedas
```sh
$ curl https://economia.awesomeapi.com.br/json/all
```
```json
{
    "USD": {
        "code": "USD",
        "codein": "BRL",
        "name": "Dólar Comercial",
        "high": "5.37",
        "low": "5.2126",
        "varBid": "-0.1498",
        "pctChange": "-2.79",
        "bid": "5.2127",
        "ask": "5.2144",
        "timestamp": "1591110126",
        "create_date": "2020-06-02 12:02:09"
    },
    "USDT": {
        "code": "USD",
        "codein": "BRLT",
        "name": "Dólar Turismo",
        "high": "5.3",
        "low": "5.21",
        "varBid": "-0.14",
        "pctChange": "-2.469",
        "bid": "5.21",
        "ask": "5.53",
        "timestamp": "1591109580000",
        "create_date": "2020-06-02 12:00:00"
    },
    "CAD": {
        "code": "CAD",
        "codein": "BRL",
        "name": "Dólar Canadense",
        "high": "3.9779",
        "low": "3.8655",
        "varBid": "-0.0854",
        "pctChange": "-2.16",
        "bid": "3.8641",
        "ask": "3.8668",
        "timestamp": "1591110125",
        "create_date": "2020-06-02 12:02:08"
    },
    "EUR": {
        "code": "EUR",
        "codein": "BRL",
        "name": "Euro",
        "high": "6.0046",
        "low": "5.8274",
        "varBid": "-0.1406",
        "pctChange": "-2.35",
        "bid": "5.8289",
        "ask": "5.8329",
        "timestamp": "1591110123",
        "create_date": "2020-06-02 12:02:06"
    },
    "GBP": {
        "code": "GBP",
        "codein": "BRL",
        "name": "Libra Esterlina",
        "high": "6.7495",
        "low": "6.5454",
        "varBid": "-0.1514",
        "pctChange": "-2.26",
        "bid": "6.5468",
        "ask": "6.55",
        "timestamp": "1591110125",
        "create_date": "2020-06-02 12:02:07"
    },
    "ARS": {
        "code": "ARS",
        "codein": "BRL",
        "name": "Peso Argentino",
        "high": "0.0783",
        "low": "0.0759",
        "varBid": "-0.0023",
        "pctChange": "-2.94",
        "bid": "0.0759",
        "ask": "0.0759",
        "timestamp": "1591110126",
        "create_date": "2020-06-02 12:02:09"
    },
    "BTC": {
        "code": "BTC",
        "codein": "BRL",
        "name": "Bitcoin",
        "high": "54998",
        "low": "50001",
        "varBid": "-663",
        "pctChange": "-1.29",
        "bid": "50359",
        "ask": "50787.1",
        "timestamp": "1591110127",
        "create_date": "2020-06-02 12:02:08"
    },
    "LTC": {
        "code": "LTC",
        "codein": "BRL",
        "name": "Litecoin",
        "high": "260",
        "low": "246.9",
        "varBid": "-6.4",
        "pctChange": "-2.53",
        "bid": "246.9",
        "ask": "250.28",
        "timestamp": "1591110126",
        "create_date": "2020-06-02 12:02:07"
    },
    "JPY": {
        "code": "JPY",
        "codein": "BRL",
        "name": "Iene Japonês",
        "high": "0.04992",
        "low": "0.04803",
        "varBid": "-0.0018",
        "pctChange": "-3.61",
        "bid": "0.048",
        "ask": "0.04806",
        "timestamp": "1591110127",
        "create_date": "2020-06-02 12:02:08"
    },
    "CHF": {
        "code": "CHF",
        "codein": "BRL",
        "name": "Franco Suíço",
        "high": "5.6058",
        "low": "5.4268",
        "varBid": "-0.1536",
        "pctChange": "-2.75",
        "bid": "5.4248",
        "ask": "5.4288",
        "timestamp": "1591110126",
        "create_date": "2020-06-02 12:02:08"
    },
    "AUD": {
        "code": "AUD",
        "codein": "BRL",
        "name": "Dólar Australiano",
        "high": "3.6869",
        "low": "3.5918",
        "varBid": "-0.0518",
        "pctChange": "-1.42",
        "bid": "3.5926",
        "ask": "3.5945",
        "timestamp": "1591110124",
        "create_date": "2020-06-02 12:02:07"
    },
    "CNY": {
        "code": "CNY",
        "codein": "BRL",
        "name": "Yuan Chinês",
        "high": "0.7559",
        "low": "0.7345",
        "varBid": "-0.0179",
        "pctChange": "-2.38",
        "bid": "0.7344",
        "ask": "0.7346",
        "timestamp": "1591110124",
        "create_date": "2020-06-02 12:02:05"
    },
    "ILS": {
        "code": "ILS",
        "codein": "BRL",
        "name": "Novo Shekel Israelense",
        "high": "1.5423",
        "low": "1.5015",
        "varBid": "-0.0332",
        "pctChange": "-2.17",
        "bid": "1.5013",
        "ask": "1.5018",
        "timestamp": "1591110127",
        "create_date": "2020-06-02 12:02:08"
    },
    "ETH": {
        "code": "ETH",
        "codein": "BRL",
        "name": "Ethereum",
        "high": "1198",
        "low": "1198",
        "varBid": "0",
        "pctChange": "0",
        "bid": "203.04",
        "ask": "6498.97",
        "timestamp": "1591087287",
        "create_date": "2020-06-02 05:41:28"
    },
    "XRP": {
        "code": "XRP",
        "codein": "BRL",
        "name": "Ripple",
        "high": "1.13",
        "low": "1.08",
        "varBid": "-0.03",
        "pctChange": "-2.69",
        "bid": "1.08",
        "ask": "1.08",
        "timestamp": "1591110127",
        "create_date": "2020-06-02 12:02:08"
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
