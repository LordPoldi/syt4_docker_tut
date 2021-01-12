# httpi

## Abfrage aller Tasks 
```console
http GET 127.0.0.1:3000/items
```

## Abfrage aller offenen Tasks 
```console
http GET http://127.0.0.1:3000/items?completed=1
```

## Setzten eines 'unerledigten' Tasks auf 'erledigt'. 
```console
http PUT 127.0.0.1:3000/items/8f9b78ac-1e16-45b6-949f-558ec6137121 completed=1 name=httpi
```

## Erstellen eines neuen Tasks 
```console
http POST 127.0.0.1:3000/items/ name=httpi
```

## Löschen eines Tasks 
```console
http DELETE 127.0.0.1:3000/items/8f9b78ac-1e16-45b6-949f-558ec6137121
```