# Estações

## Obtendo todas as estações

```shell
curl "http://dev.labmet.com.br/v1/stations"
  -H "X-Api-Key: meowmeowmeow"
```

> O comando acima retorna uma estrutura JSON parecida com isso, onde **total** é a quantidade de estações e **size** é a quantidade total de cada resposta:

```json
{"total": 1532,
 "size": 25,
 "cursor": "DXF1ZXJ5QW5kRmV0Y2gBAAAAAACB-eoWaFJjV0FrTS1UMXlxTmRMYVJyZ3hKQQ==",
 "stations": [{"id": "dHhwwWUBFst_hbbgnWGN",
   "type": "labmet",
   "model": "automatic",
   "city": "guaraci",
   "state": "sp",
   "code": "lmt0013",
   "latitude": -20.1906228183,
   "longitude": -49.0471931786},
  {"id": "dXhwwWUBFst_hbbgnWGN",
   "type": "labmet",
   "model": "automatic",
   "city": "pitangueiras",
   "state": "sp",
   "code": "lmt0017",
   "latitude": -21.0521195365,
   "longitude": -48.2647871106}
 ]
}
```

Esse endpoint retorna todas as estações meteorológicas.

### HTTP Request

`GET https://api.labmet.com.br/v1/stations`

### Parâmetros URL

Parametro | Padrão | Descrição
--------- | ------- | -----------
cursor | null | cursor utilizado em caso de paginação
city | null | caso seja passado o nome de uma cidade serão retornado as estações de uma cidade.

<aside class="success">
Relembre - para todos os acessos é necessário enviar o cabeçalho com a chave de acesso!
</aside>
