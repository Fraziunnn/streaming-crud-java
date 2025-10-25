# StreamingCRUD - MongoDB e Redis

Projeto Java com integração a MongoDB Atlas e Redis, realizando operações CRUD (Create, Read, Update, Delete).

## Estrutura do Projeto

StreamingCRUD/
├─ src/br/edu/seu/streaming/
│ ├─ MongoCRUD.java
│ └─ RedisCRUD.java
├─ lib/
│ ├─ mongodb-driver-sync-4.11.0.jar
│ ├─ mongodb-driver-core-4.11.0.jar
│ ├─ bson-4.11.0.jar
│ └─ jedis-5.1.0.jar
├─ README.md


## Dependências

- Java 17+  
- Eclipse IDE  
- JARs no Build Path: mongodb-driver-sync, mongodb-driver-core, bson, jedis

## MongoDB Atlas

1. Criar cluster gratuito no MongoDB Atlas.  
2. Criar usuário e senha.  
3. Permitir acesso ao IP da sua rede (0.0.0.0/0 para testes).  
4. Substituir `<usuario>` e `<senha>` na URL de conexão no `MongoCRUD.java`.  
5. Executar como Java Application no Eclipse.

### Exemplo de Saída

Inserido: {"nome":"Carlos","idade":28,"assinatura":"Premium","generoPreferido":"Ação"}
Encontrado: {"nome":"Carlos","idade":28,"assinatura":"Premium","generoPreferido":"Ação"}
Atualizado: {"nome":"Carlos","idade":28,"assinatura":"Gold","generoPreferido":"Ação"}
Deletado. Agora buscar retorna: null


## Redis

1. Rodar Redis Server localmente.  
2. Executar `RedisCRUD.java` como Java Application.

### Exemplo de Saída

Inserido: {nome=Carlos, idade=28, assinatura=Premium, generoPreferido=Ação}
Buscar: {nome=Carlos, idade=28, assinatura=Premium, generoPreferido=Ação}
Atualizado: {nome=Carlos, idade=28, assinatura=Gold, generoPreferido=Ação}
Deletado. Existe? false


## Vídeo Demonstrativo

[Assista ao vídeo aqui](https://youtu.be/ErI4tK0HuHQ)
