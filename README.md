# API de Cotações
API de Cotações do Dólar (USD, USDT, CA), Euro, Libra e Peso, atualizado de 10 em 10 minutos.

## Exemplo de uso

```
curl https://economia.awesomeapi.com.br/all
```
```json
{
  "USD": {
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
  },
  "USDT": {
    "idreg": "113273",
    "code": "USD",
    "codein": "BRLT",
    "name": "Dólar Turismo",
    "high": "3.39",
    "pctChange": "-1.127",
    "open": "0",
    "bid": "3.24",
    "ask": "3.51",
    "timestamp": "1466625600000",
    "low": "3.23",
    "notFresh": "0",
    "varBid": "-0.04",
    "create_date": "2016-06-22 18:40:03"
  },
  "CAD": {
    "idreg": "113274",
    "code": "CAD",
    "codein": "BRL",
    "name": "Dólar Canadense (R$)",
    "high": "2.6747",
    "pctChange": "-1.316",
    "open": "3",
    "bid": "2.6302",
    "ask": "2.6318",
    "timestamp": "1466625540000",
    "low": "2.6276",
    "notFresh": "0",
    "varBid": "-0.0351",
    "create_date": "2016-06-22 18:40:04"
  },
  "EUR": {
    "idreg": "113275",
    "code": "EUR",
    "codein": "BRL",
    "name": "Euro (R$)",
    "high": "3.8584",
    "pctChange": "-0.609",
    "open": "4",
    "bid": "3.8161",
    "ask": "3.8189",
    "timestamp": "1466625540000",
    "low": "3.8045",
    "notFresh": "0",
    "varBid": "-0.0234",
    "create_date": "2016-06-22 18:40:06"
  },
  "GBP": {
    "idreg": "113276",
    "code": "GBP",
    "codein": "BRL",
    "name": "Libra Esterlina (R$)",
    "high": "5.0227",
    "pctChange": "-0.84",
    "open": "5",
    "bid": "4.9621",
    "ask": "4.9669",
    "timestamp": "1466625540000",
    "low": "4.9423",
    "notFresh": "0",
    "varBid": "-0.0421",
    "create_date": "2016-06-22 18:40:07"
  },
  "ARS": {
    "idreg": "113277",
    "code": "ARS",
    "codein": "BRL",
    "name": "Peso Argentino (R$)",
    "high": "0.2445",
    "pctChange": "-2.04",
    "open": "0",
    "bid": "0.24",
    "ask": "0.2401",
    "timestamp": "1466625540000",
    "low": "0.2393",
    "notFresh": "0",
    "varBid": "-0.005",
    "create_date": "2016-06-22 18:40:09"
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

## Formato de saída
```
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
