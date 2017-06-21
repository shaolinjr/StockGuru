# Endpoints for the Google Finance API

## Getting currencies

http://finance.google.com/finance/info\?client\=ig\&q\=CURRENCY:[currency_base+currency_to_compare]

For example if I want to know the value of one dollar in Brazillian Real :

http://finance.google.com/finance/info\?client\=ig\&q\=CURRENCY:USDBRL

## Getting stockPrices
http://finance.google.com/finance/info\?client\=ig\&q\=[company_market_symbol]

## Request return structure
```
[
{
"id": "-2001","t" : "BTCUSD",
"e" : "CURRENCY","l" :"2,753.5500",
"l_fix":"","l_cur" : "",
"s": "0","ltt":"",
"lt" : "Jun 20, 9:35PM GMT",
"lt_dts" : "2017-06-20T21:35:44Z",
"c" : "+159.56000","c_fix" : "",
"cp" : "6.151","cp_fix" : "",
"ccol" : "chg","pcls_fix" : ""
}
]
```

### Attributes meaning of the returned request

| Attribute | Meaning     |
| :------------- | :------------- |
|t |Ticker
|e	|Exchange (eg: NASDAQ, NYSE,BMF) or Request type (eg.CURRENCY)
|l	|Last Price
|ltt	|Last Trade Time
|l	|Price
|lt	|Last Trade Time Formatted
|lt_dts	|Last Trade Date/Time
|c	|Change
|cp	|Change Percentage
|el	|After Hours Last Price
|elt	|After Hours Last Trade Time Formatted
|div	|Dividend
|yld	|Dividend Yield
```


```
