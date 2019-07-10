## Instalando dependencias no Projeto React Native

* Exemplo de instalação de Fontes

Adicione os dados abaixo no package.json, no mesmo nivel do "devDependencies" e "dependencies"

Obs: Para o iOS o meta dados deve ter o mesmo nome do arquivo.

```json
"rnpm": {
  "assets": {
	"./assets/fonts/"
  }
}
```

Depois salvar o arquivo, execute o comando:

```
react-native link
```

Será enviado as fontes para a pasta das respectivas plataformas, configurando o código nativo.

Depois de tudo configurado, basta colocar o nome da fonte dentro do CSS para usar a fonte
