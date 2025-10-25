# StreamingCRUD - MongoDB e Redis

Projeto de integração Java com MongoDB Atlas e Redis.

## Estrutura do Projeto

- src/br/edu/seu/streaming/
    - MongoCRUD.java
    - RedisCRUD.java
- lib/
    - mongodb-driver-sync-4.11.0.jar
    - mongodb-driver-core-4.11.0.jar
    - bson-4.11.0.jar
    - jedis-5.1.0.jar

## MongoDB Atlas

1. Criar cluster gratuito no MongoDB Atlas.
2. Criar usuário e senha.
3. Permitir IP da sua rede (0.0.0.0/0 para testes).
4. Copiar URL de conexão (com `<usuario>` e `<senha>`).

### Rodar MongoCRUD
```bash
- Adicione os jars no Build Path do Eclipse.
- Substitua <usuario> e <senha> na string de conexão.
- Execute como Java Application.

### Link do vídeo

https://youtu.be/ErI4tK0HuHQ
