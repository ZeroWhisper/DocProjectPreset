# Dicas de GIT

Para manter!!!

Criar o repositório e adicionar 3 branches, master, develop e features

Dentro do features, pode ter várias branches para ser mergiada com o develop

Depois que a develop for validade, mandar para a master.

Cada branch, tentar manter o nome 20191230\_[nome]

## Resumo

- `git init` // inicia a linha do tempo
- `git add` // adiciona ou atualizar mudanças para irem para a linha do tempo
- `git commit` // adiciona um ponto na linha do tempo
- `git log` // visualiza os pontos na linha do tempo
- `git status` // informa o estado das alterações do nosso projeto
- `git show` // apresenta determina o ponto na história
- `git branch` // gerencia novas linhas do tempo
- `git checkout` // manipula as linhas do tempo
- `git merge` // unir linhas do tempo
- `git push` // enviar alterações locais para o repositório remoto

### Iniciando o Git

git init

- Depois do comando, é gerado uma pasta .git com os dados do git

### Adicionando repositório

git remote add [origin][url-do-github]

- por padrão, o primeiro repositório se chama origin

### Git Status

git status

- Lista os items que foram modificados

### Git log

git log

- Mostra o histórico dos commits git

### Git show

git show [hash || '']

- Mostra o conteudo do ultimo

### Adicionando items para o commit

git commit -m "Minha mensagem"

### Criando uma nova Branch

git branch [pasta/nome]
ou
git branch [nome]

Para remover

git branch -D [pasta/nome]

### Trocando de branch

git checkout [pasta/nome]
ou
git checkout [nome]

### Git merge

git merge [outra/pasta/nome]

- Adiciona contudo da branch da linha de comando na branch atual
