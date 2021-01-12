# SQL

## Abfrage aller Tasks 
```sql
SELECT * FROM todos.todo_items;
```

## Abfrage aller offenen Tasks 
```sql
SELECT * FROM todos.todo_items
WHERE completed = 0;
```

## Setzten eines 'unerledigten' Tasks auf 'erledigt'. 
```sql
UPDATE todos.todo_items
SET completed = 0
WHERE id = "333dcf2d-f84d-4fc3-86d3-d345572eb9dc";
```

## Erstellen eines neuen Tasks 
```sql
INSERT INTO todos.todo_items
VALUES("8b55bbb6-3ee7-4e0e-80c7-d9ae5878107b", "test-item-wb", 0)
```

## Löschen eines Tasks 
```sql
DELETE FROM todos.todo_items
WHERE id = "333dcf2d-f84d-4fc3-86d3-d345572eb9dc";
```