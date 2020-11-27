introspect the data that is returned from this end point.

```cypher
WITH "https://api.stackexchange.com/2.2/questions?pagesize=100&order=desc&sort=creation&tagged=neo4j&site=stackoverflow&filter=!5-i6Zw8Y)4W7vpy91PMYsKM-k9yzEsSC1_Uxlf" AS url
CALL apoc.load.json(url) YIELD value
UNWIND value.items AS item
RETURN item.title, item.owner, item.creation_date, keys(item)
LIMIT 5;
```

https://neo4j.com/labs/apoc/4.1/import/load-json/#load-json-examples-stackoverflow
