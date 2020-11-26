# cypher-shell

Cypher Shell 是一个命令行工具，在 Neo4j 的默认安装里自带。可以在`$NEO_HOME/bin`目录下找到它

```bash
☁  neo4j-codelab [master] docker-compose exec neo4j sh
# cypher-shell
username: neo4j
password: ********
Connected to Neo4j 4.2.0 at neo4j://localhost:7687 as user neo4j.
Type :help for a list of available commands or :exit to exit the shell.
Note that Cypher queries must end with a semicolon.
neo4j@neo4j> match(n) return n;
```

退出 shell:

```bash
neo4j@neo4j> :exit

Bye!
```
