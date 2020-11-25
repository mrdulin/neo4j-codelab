PROFILE MATCH (tom)-[:ACTED_IN]->(tomHanksMovies) RETURN tom,tomHanksMovies


AllNodesScan运算符开头的。这意味着数据库中所有的节点都会被遍历，以查看它们是否满足查询条件。我们注意到数据库命中数更高了，并且在第一个和第二个节点后连接线也更粗了。
这意味着查询的效率低下，因此我们最好把标签放回去。