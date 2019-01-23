# Iniciar um projeto em NodeJS

yarn init -y
npm init -y

Exemplo de uso:
Remover: yarn remove <package_name>
Instalar na versão específica: npm install -g pg@6.4.2
Instalar de forma global: 
 npm install -g <package_name>
 yarn add global <package_name>


# Exemplo para dep de Desenvolvimento
npm install NOME -D
yarn add NOME -D

# Instalando ESLint no seu projeto
npx eslint --init

Configuração padrão: 
1 - Use a popular style guide
2 - Standard (https://github.com/standard/standard)
3 - JSON

Depois, digite Y para ele finalizar a instalação via NPM
- Nota: Ele vai criar um package-lock.json. Pra resolver isso, delete este arquivo e digite somente yarn na pasta do projeto. Assim o lock será apenas do yarn



# MongoDB

Site para testes de Dev
https://www.mongodb.com/cloud/atlas
https://mlab.com/

# Executar o Sequelize
.\node_modules\.bin\sequelize init
ou 
npx sequelize init

# Drive para cada banco de dados

 - postgres: pg
 - mysql: mysql2




# Extra

## Sequelize Reverse

Sequelize reverse - Funciona
https://github.com/sequelize/sequelize-auto
https://stackoverflow.com/questions/10060265/sequelize-how-to-import-definitions-from-an-existing-database

sequelize-auto -h 127.0.0.1 -d "campanha-vacinacao" -u postgres -x postgres -p 5432 -e postgres -o "./src/app/models"

## Docker

https://www.docker.com/get-started



