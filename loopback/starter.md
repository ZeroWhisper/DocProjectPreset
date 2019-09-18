font: https://www.youtube.com/watch?v=jQ6abvNmQiA

### Instalar o Loopback 4

yarn global add @loopback/cli

- Depois de instalado, todos os comandos vão partir de `lb4`
- Para um inicio rápido, basta digitar `yarn start`

### Conexão com o Banco de Dados

`yarn add loopback-connector-mongodb`

`lb4 dabasource mongoDS --concector mongoDB`

- Depois do comando acima, basta selecionar o driver e colar o endereço do Banco

### Criando models

`lb4 model <name>`

### Criando repositórios

`lb4 repository <name>`

### Criando controller

`lb4 controller <name>`

- Tanto o model, repository e controller serão questionados via terminal

### Extra

Para usar o loopback 4 com graphql

`https://loopback.io/openapi-to-graphql.html`
