## Instalando dependencias no Projeto React Native

* Exemplo de instalação de fonte

Adicione os dados abaixo no package.json, no mesmo nivel do "devDependencies"

"rnpm": {
  "assets": {
	"./assets/fonts/"
  }
}

Depois salvar o arquivo, execute o comando:

react-native link