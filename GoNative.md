## Emulador sugerido

https://visualstudio.microsoft.com/pt-br/vs/msft-android-emulator/

# ZeroWhisper :stuck_out_tongue_winking_eye:

## Ambiente Native (*Download*)

1.1. Android Studio (Download pesado)
Acesse o site e fazer o download do Android Studio para seu OS.
Link: [Androind Studio](https://developer.android.com/studio/)

Depois do Download...

Usar o Samsung Galaxy S8 7.0.0

1.2. Chocolatey
Abrir o PowerShell como admin
Execute o seguinte comando. (Depois da instalação execute choco -v para ver se a instalação teve sucesso)
cmd: Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

1.3. Esse comando vai instalar várias dependecias
cmd: choco install -y nodejs.install python2 jdk8


1.4. Instalar yarn
Acesse o site do [Yarn](https://yarnpkg.com/lang/en/docs/install/#windows-stable) ou se você tiver o Chocolatey
cmd: choco install yarn

## Iniciando o Projeto (*Configs*)

2.1. Iniciando um projeto React-Native
cmd: react-native init nomeDoProjeto

2.2. Depois de iniciar o Projeto (Esse passo deve ser executado apenas uma vez)
Preparar o ambiente que você está usando, setar o dispositivo que será usado para testes já com o Disposito aberto.
Ou seja, se você vai usar android, você deve estar com o Android Virtual (genymotion) aberto neste momento.

* Android
cmd: react-native run-android

* iOS
cmd: react-native run-ios

2.3. Instanciando o Servidor para testes. Nesse caso, você já fez o passo 2.2.
Pra iniciar e começar os teste no Android, execute o comando:
cmd: react-native start

Caso existe cache e você precise limpar. Carrega todos os arquivos do Projeto novamente para o Disposito Virtual
cmd: react-native start --reset-cache

## Pacotes extras

// Plugin para forçar tipo de valor nos Componentes do react-native
cmd: yarn add prop-types

// Plugin para auxiliar no debbug do Projeto
cmd: yarn add reactotron-react-native


// Plugin para padrão de código
* ESLint
cmd: yarn global add eslint
cmd: npm install -D eslint (Comando do curso GoReact)
cmd: npm install -D babel-eslint (Necessário no curso GoReact)

Execute o comando para inicializar o ESLint dentro do projeto.
cmd: node_module/.bin/eslint --init

Depois, forme as respostas:
- Use a populat style guide
- Airbnb
Do you use React? (ocasional)
- JSON

### Configs do Visual Code Studio!

Arquivo .eslint.json
´´´json
{
  "parser": "babel-eslint",
  "extends": "airbnb",
  "env": {
	"browser": true,
	"jest": true, // GoReact
  },
  "plugins": [
	"react",
	"jsx-a11y"microsoft",
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
´´´


* O compando "yarn", funciona como o "npm install"
Plugins extras para o ESLint

    "eslint": "~",
    "eslint-plugin-import": "~",
    "eslint-plugin-jsx-a11y": "~",
    "eslint-plugin-react": "~"

// Fazer o projecto funcionar com acesso ao caminha raiz, e não caminha relativo
cmd: yarn add babel-plugin-module-resolver --dev
// Caso você tenha o 
cmd: yarn add eslint-import-resolver-babel-module --dev 

// Plugin para exibir o DOM do seu projeto, pronto pra você inspecionar o HTML
cmd: yarn add react-devtools --dev

// Abas para navegação dentro do aplicativo
cmd: yarn add react-navigation@1.5.2

// Axios para fazer requisições https
cmd: yarn add axios

// Icones para React-Native
cmd: yarn add react-native-vector-icons
cmd: react-native link react-native-vector-icons


Modulo 3:
yarn add redux react-redux