[![AwesomeAPI](https://cdn.awesomeapi.com.br/awesomeapi/assets/awapi1c.png)](https://economia.awesomeapi.com.br/)

# API de Cotações
API de Cotações do Dólar (USD, USDT, CA), Euro, Libra, Peso e Bitcoin, atualizado de 10 em 10 minutos.

# DOCUMENTAÇÃO DESATUALIZADA
Veja a documentação atualizada em [https://docs.awesomeapi.com.br/](https://docs.awesomeapi.com.br/)

## Exemplo de uso
```
curl https://economia.awesomeapi.com.br/all
```
```json
{
  "USD": {
    "code": "USD",
    "codein": "BRL",
    "name": "Dólar Comercial",
    "high": "3.279",
    "low": "3.2489",
    "pctChange": "-0.455",
    "open": "0",
    "bid": "3.2552",
    "ask": "3.2567",
    "varBid": "-0.0149",
    "timestamp": "1512154740000",
    "create_date": "2017-12-03 22:40:01"
  },
  "USDT": {
    "code": "USD",
    "codein": "BRLT",
    "name": "Dólar Turismo",
    "high": "3.26",
    "low": "3.12",
    "pctChange": "0.587",
    "open": "0",
    "bid": "3.24",
    "ask": "3.43",
    "varBid": "0.02",
    "timestamp": "1512153900000",
    "create_date": "2017-12-03 22:40:02"
  },
  "CAD": {
    "code": "CAD",
    "codein": "BRL",
    "name": "Dólar Canadense (R$)",
    "high": "2.569",
    "low": "2.5639",
    "pctChange": "0.027",
    "open": "3",
    "bid": "2.5654",
    "ask": "2.5663",
    "varBid": "0.0007",
    "timestamp": "1512326220000",
    "create_date": "2017-12-03 22:40:04"
  },
  "EUR": {
    "code": "EUR",
    "codein": "BRL",
    "name": "Euro (R$)",
    "high": "3.8731",
    "low": "3.8624",
    "pctChange": "-0.253",
    "open": "4",
    "bid": "3.865",
    "ask": "3.8659",
    "varBid": "-0.0098",
    "timestamp": "1512327540000",
    "create_date": "2017-12-03 22:40:05"
  },
  "GBP": {
    "code": "GBP",
    "codein": "BRL",
    "name": "Libra Esterlina (R$)",
    "high": "4.3928",
    "low": "4.3745",
    "pctChange": "-0.264",
    "open": "4",
    "bid": "4.3774",
    "ask": "4.3793",
    "varBid": "-0.0116",
    "timestamp": "1512327540000",
    "create_date": "2017-12-03 22:40:06"
  },
  "ARS": {
    "code": "ARS",
    "codein": "BRL",
    "name": "Peso Argentino (R$)",
    "high": "0.1895",
    "low": "0.1878",
    "pctChange": "-0.106",
    "open": "0",
    "bid": "0.1889",
    "ask": "0.1892",
    "varBid": "-0.0002",
    "timestamp": "1512154740000",
    "create_date": "2017-12-03 22:40:07"
  },
  "BTC": {
    "code": "BTC",
    "codein": "BRL",
    "name": "Bitcoin",
    "high": "43123",
    "low": "41300",
    "pctChange": "0",
    "open": "0",
    "bid": "42505.08789",
    "ask": "42800",
    "varBid": "0",
    "timestamp": "1512347394",
    "create_date": "2017-12-03 22:40:08"
  }
}
```

## Uma única moeda
```
https://economia.awesomeapi.com.br/{MOEDA}/{Numero de resultados}
```
```
curl http://economia.awesomeapi.com.br/USD-BRL/1
```
```json
[
  {
    "idreg": "113272",
    "code": "USD",
    "codein": "BRL",
    "name": "Dólar Comercial",
    "high": "3.3994",
    "pctChange": "-0.834",
    "open": "0",
    "bid": "3.3763",
    "ask": "3.3778",
    "timestamp": "1466625540000",
    "low": "3.3685",
    "notFresh": "0",
    "varBid": "-0.0284",
    "create_date": "2016-06-22 18:40:01"
  }
]
```
> **Códigos disponíveis**
> - USD-BRL (Dólar Comercial)
> - USD-BRLT (Dólar Turismo)
> - CAD-BRL (Dólar Canadense)
> - EUR-BRL (Euro)
> - GBP-BRL (Libra Esterlina)
> - ARS-BRL (Peso Argentino)
> - BTC-BRL (Bitcoin)

## Formato de saída
```
curl http://economia.awesomeapi.com.br/jsonp/USD-BRL/1?callback=jsonp_callback
curl http://economia.awesomeapi.com.br/xml/USD-BRL/1
curl http://economia.awesomeapi.com.br/USD-BRL/1?format=xml
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<xml>
	<item>
		<idreg>428446</idreg>
		<codein>BRL</codein>
		<high>3.206</high><pctChange>-0.726</pctChange>
		<bid>3.1839</bid>
		<timestamp>1500062400000</timestamp>
		<notFresh>1</notFresh>
		<create_date>2017-07-15 12:30:02</create_date>
	</item>
</xml>

```
> **Formatos suportados**
> - JSON
> - JSONP
> - XML
> - HTML
> - CSV
> - SERIALIZED

### Legendas
Key | Tradução
-------- | ---
**bid** | Compra
**ask** | Venda
**varBid** | Variação
**pctChange** |  Porcentagem de Variação
**high** | Máximo
**low** | Mínimo
