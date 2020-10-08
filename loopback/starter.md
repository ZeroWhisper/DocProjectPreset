# This is a test

Fonts:
https://www.youtube.com/watch?v=jQ6abvNmQiA
https://www.youtube.com/watch?v=3zK0tdZsKPU

Banco de Dados:
https://www.elephantsql.com/

### Instalar o Loopback 4

`yarn global add @loopback/cli`

- Depois de instalado, todos os comandos vão partir de `lb4`
- Para um inicio rápido, basta digitar `yarn start`

### Criando a API (https://loopback.io/doc/en/lb4/Application-generator.html)

`lb app <name>`

- Exemplo
  `lb app project`

### Conexão com o Banco de Dados

`yarn add loopback-connector-mongodb`

`lb dabasource mongoDS --concector mongoDB`

- Depois do comando acima, basta selecionar o driver e colar o endereço do Banco

### Criando models (https://loopback.io/doc/en/lb4/Model-generator.html)

`lb4 model <name>`

- Exemplo
  `lb4 model user -y` // -y confirma todas as opcoes pre-definidas

# Extra:

Procurar com base no banco de dados. Apenas alguns suportados
https://loopback.io/doc/en/lb4/Discovering-models.html
`lb4 discover`

### Criando repositórios

`lb4 repository <name>`

### Criando controller (https://loopback.io/doc/en/lb4/Controller-generator.html)

`lb4 controller <name>`

- Inline
  `lb4 controller [options] [<name>]`
- Exemplo
  `lb4 controller --controllerType=REST user`

- Tanto o model, repository e controller serão questionados via terminal

### Criando relação entre tabelas (https://loopback.io/doc/en/lb4/Relation-generator.html)

`lb4 relation`

- Inline

```sh
lb4 relation
--sourceModel=<sourceModel>
--destinationModel=<destinationModel>
--foreignKeyName=<foreignKeyName>
--relationType=<hasMany|belongsTo>
[--relationName=<relationName>]
[--format]
```

relationType - Type of the relation that will be created between the source and target models.

sourceModel - Name of the model to create the relationship from.

destinationModel - Name of the model to create a relationship with.

foreignKeyName - Property that references the primary key property of the destination model.

relationName - Name of the relation that will be created.

Relations (https://loopback.io/doc/en/lb4/Relations.html)

### Extra

Para usar o loopback 4 com graphql

`https://loopback.io/openapi-to-graphql.html`
