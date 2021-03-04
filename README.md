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
let isOpen: boolean
    isOpen = true / false
~~~

* `string`
~~~TypeScript
// String ('foo' , "foo", `foo`) // backstick
let message: string
    message = `foo ${ isOpen }`  // incluir variavel isOpen
~~~

* `number`
~~~TypeScript
// number (int, float, hex, binary)
let total: number
   total = 20.3  / 0xff0 (hexa)
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
let title: [number, string, boolen]
    title = [1 , "nome", true]
~~~

* `enum`
~~~TypeScript
// enum : conjunto Chave/valor
enum Colors {
	white = '#fff',   
	black = '#000'
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
function logger(): void{	// tipar a funçao >> retorna nada, float
	console.log('foo')
}
~~~

* `null`
~~~TypeScript
// null / undefined
// tipo não primitivo
type Bla = string | underfined   // pode ser strin ou nao definido
~~~

* `never`
~~~TypeScript
// never (nunca vai retornar)
function error(): never {
	throw new error("Error");
}
~~~

* `Object`
~~~TypeScript
// Object "qualque coisa não primitiva" (equivale a uma Classe)
let cart: object
    cart = {
	key: "chave"
    }

~~~ 

