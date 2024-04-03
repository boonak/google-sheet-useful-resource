## Google Sheet Formula

**Stacking Tables from different sheets**
-  ranges in each IMPORTRANGE must be equal
```
=Query({
IMPORTRANGE("<google sheet url 1>", "SheetA!A2:I");
IMPORTRANGE("<google sheet url 2>", "SheetB!A2:I");
IMPORTRANGE("<google sheet url 3>", "SheetC!A2:I")
},
"Select * Where Col3 IS NOT NULL", 1)
```
