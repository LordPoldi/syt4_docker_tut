# Curl

## Abfrage aller Tasks 
```console
curl 127.0.0.1:3000/items
```

## Abfrage aller offenen Tasks 
```console
curl http://127.0.0.1:3000/items?completed=1
```

## Setzten eines 'unerledigten' Tasks auf 'erledigt'. 
```console
curl -X PUT -H "Content-Type: application/json" "JSON" -d '{"name":"curl-test", "completed":true}' 127.0.0.1:3000/items/e06639d8-743c-42d7-b07d-7d472f0bebfe
```

## Erstellen eines neuen Tasks 
```console
curl -X POST -H "Content-Type: application/json" -d '{"name":"curl-test"}' 127.0.0.1:3000/items/
```

## Löschen eines Tasks 
```console
curl -X DELETE 127.0.0.1:3000/items/e06639d8-743c-42d7-b07d-7d472f0bebfe
```