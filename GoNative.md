## Emulador Sugerido

https://visualstudio.microsoft.com/pt-br/vs/msft-android-emulator/

## Ambiente Native (*Download and Install*)

1. [Android Studio](https://developer.android.com/studio/) (Download pesado)  
Acesse o site e fazer o download do Android Studio para seu OS. Usar o Samsung Galaxy S8 7.0.0 de preferência. Ou um Android 6.0.0+

2. [Chocolatey](https://chocolatey.org/docs/installation)
Resumo: Abrir o PowerShell como admin e execute o seguinte comando. (Depois da instalação execute choco -v para ver se a instalação teve sucesso)
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')) 
```

3. Esse comando vai instalar várias dependências preparando o ambiente de desenvolvimento. Ou acesse o site do [Node.js](https://nodejs.org/en/)
```
choco install -y nodejs.install python2 jdk8
```


4. Instalar [Yarn](https://yarnpkg.com/lang/en/docs/install/#windows-stable)  
Ou se você tiver o Chocolatey
```
choco install yarn
```

## Iniciando o Projeto (*Configs*)

1. Iniciando um projeto React-Native
```
react-native init nomeDoProjeto
```

2. Depois de iniciar o Projeto (Esse passo deve ser executado apenas uma vez)
Preparar o ambiente que você está usando, setar o dispositivo que será usado para testes já com o Disposito aberto.
Ou seja, se você vai usar android, você deve estar com o Android Virtual (genymotion) aberto neste momento.

* Android
```
react-native run-android
```

* iOS
```
react-native run-ios
```

3. Instanciando o Servidor para testes. Nesse caso, você já fez o passo 2.2.
Pra iniciar e começar os teste no Android, execute o comando:
```
react-native start
```

Caso existe cache e você precise limpar. Carrega todos os arquivos do Projeto novamente para o Disposito Virtual
```
react-native start --reset-cache
```

## Pacotes extras

// Plugin para forçar tipo de valor nos Componentes do react-native
```
yarn add prop-types
```

// Plugin para auxiliar no debbug do Projeto
```
yarn add reactotron-react-native
```

// Plugin para padrão de código
* ESLint
```
yarn global add eslint  
npm install -D eslint (Comando do curso GoReact)  
npm install -D babel-eslint (Necessário no curso GoReact)  
```

Execute o comando para inicializar o ESLint dentro do projeto.
```
node_module/.bin/eslint --init
```

Depois, forme as respostas:
- Use a populat style guide
- Airbnb
Do you use React? (ocasional)
- JSON

### Configs do Visual Code Studio!

Arquivo .eslint.json
```json
{
  "parser": "babel-eslint",
  "extends": "airbnb",
  "env": {
	"browser": true,
	"jest": true, // GoReact
  },
  "plugins": [
	"react",
	"jsx-a11y",
	"import"
  ],
  "rules": {
    "react/jsx-filename-extension": [
	"error",
	{
	  "extension": [
	    ".js",
		".jsx"
	  ]
	}
	],
	"global-require": "off",
	"import/prefer-default-export": "off",
	"no-unused-vars": [
	  "error", 
	  {
	    "argsIgnorePattern": "^_"
	  }
	]
  }
}
```


* O compando "yarn", funciona como o "npm install"
Plugins extras para o ESLint

    "eslint": "\~",  
    "eslint-plugin-import": "\~",  
    "eslint-plugin-jsx-a11y": "\~",  
    "eslint-plugin-react": "\~"  

* Fazer o projecto funcionar com acesso ao caminha raiz, e não caminha relativo
```
yarn add babel-plugin-module-resolver --dev
```
* Caso você tenha o ESLint (Rever essa linha)
```
yarn add eslint-import-resolver-babel-module --dev 
```

* Plugin para exibir o DOM do seu React-Native, pronto pra você inspecionar o HTML
```
yarn add react-devtools --dev
```

* Abas para navegação dentro do aplicativo
```
yarn add react-navigation@1.5.2
```

* Axios para fazer requisições https
```
yarn add axios
```

* Icones para React-Native
```
yarn add react-native-vector-icons
react-native link react-native-vector-icons
```


Modulo 3:
```
yarn add redux react-redux
```
