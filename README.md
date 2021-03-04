# TypeScript
Repositório com estudos realizados sobre TypeScript

Considerações: TypeScript > ECMScript6 (2015) > ECMAScript5 (2009)

https://www.typescriptlang.org/

* Instalação:
* $ npm install -g typescript	    // pre-requesito: Node.js
* $ tsc nome_arquivo.ts --watch   // Compilar via terminal
* $ tsc --init                    // cria arquivo tsconfig.jason (conf, regras, compatibilidade,..)

# Sintaxe

# Tipos de dados

 * `boolean`
~~~TypeScript
//boolean (true / false)
let conectado: boolean
    conectado = true / false
~~~

* `string`
~~~TypeScript
// String ('texto' , "texto", `texto`) // backstick
let message: string
    message = `texto ${ conectado }`  // incluir variavel isOpen
~~~

* `number`
~~~TypeScript
// number (int, float, hex, binary)
let total: number
   total = 45.6  / 0xff0 (hexa)
~~~

* `Array`
~~~TypeScript
// array
let items: number[]  //array de numeros
    items = [1,2,3]

let items: string[]
    items['um', 'dois']

let total: Array<number>
    items = [1,2,3]

let items: Array<string>	// notação generic
    items['um', 'dois']
~~~

* `tuple`
~~~TypeScript
// tuple: array sabe o numero de elementos e o tipo
let titulo: [number, string, boolen]
    titulo = [5 , "texto", true]
~~~

* `enum`
~~~TypeScript
// enum : conjunto Chave/Valor
enum Cores {
	branco = '#fff',   
	preto  = '#000'
}
~~~

* `any`
~~~TypeSript
// any : QUALQUER COISA
let coisa: any
    coisa = "true" // string
    coisa = true   // boolena
    coisa = 123    // numero
~~~

* `void`
~~~TypeScript
// void
function menssagem(): void{	// tipar a funçao >> retorna nada, float, ..
	console.log('texto')
}
~~~

* `null`
~~~TypeScript
// null / undefined
// tipo não primitivo
type coisa = string | underfined   // pode ser string ou nao definido
~~~

* `never`
~~~TypeScript
// never (nunca vai retornar)
function menssagem(): never {
	throw new messagem("Error");
}
~~~

* `Object`
~~~TypeScript
// Object "qualque coisa não primitiva" (equivale a uma Classe)
let compra: object
    compra = {
	id: 	"identificação",
	valor: 	123.45
    }

~~~ 

