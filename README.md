[<img src="https://cdn.awesomeapi.com.br/v2/png/logo-without-slogan.png" height="40px" />](https://awesomeapi.com.br/)

# API de Cotações
API de Cotações em tempo real com mais de 150 moedas

### Veja toda a documentação em [https://docs.awesomeapi.com.br/](https://docs.awesomeapi.com.br/)

## Exemplo de uso
Retornar moedas selecionadas
```sh
$ curl https://economia.awesomeapi.com.br/json/last/USD-BRL,EUR-BRL
```
```json
{
    "USDBRL": {
        "code": "USD",
        "codein": "BRL",
        "name": "Dólar Americano/Real Brasileiro",
        "high": "5.37",
        "low": "5.2257",
        "varBid": "-0.1351",
        "pctChange": "-2.52",
        "bid": "5.2279",
        "ask": "5.2285",
        "timestamp": "1591109752",
        "create_date": "2020-06-02 11:55:53"
    },
    "EURBRL": {
        "code": "EUR",
        "codein": "BRL",
        "name": "Euro/Real Brasileiro",
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
