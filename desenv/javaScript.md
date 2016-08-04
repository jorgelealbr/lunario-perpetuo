# JavaScript

### String

* é **imutável**
* pode ser declarada com aspas **simples** ou **duplas**

### Boolean

* `0`, `NaN`, '', `null` e `undefined` são `false`

### undefined

* é retornado quando um objeto não possui uma propriedade que foi consultada

    ````javascript
    > var pessoa = {};
    > pessoa.idade
    undefined
    ````
* cuidado com a pegadinha

    ````javascript
    > pessoa.nome = 'Jorge';
    > pessoa.nome
    'Jorge'

    > pessoa.nome = undefined
    > pessoa.nome
    undefined
    ````

    Mesmo possuindo a propriedade `nome` o retorno foi `undefined`.

### null

* indica a ausência de valor