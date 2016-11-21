# Angular 1.x

## Serviços

### provider()

Permite que você configure explicitamente o serviço.
Para usar a função `provider()` a função passada como parâmetro deve conter uma propriedade chamada `$get`.
A função atribuída a essa propriedade será a função executada pelo Angular para criar o serviço, que será representado pelo objeto retornado
por esta função.

````javascript
    $provide.provider('books', function() {
        this.$get = function() {
            var appName = 'Book Logger';
            return {
                appName: appName
            };
        }
    });
````

### factory()

Se você não precisa configurar o serviço, use a função `factory()` que é mais simples de criar o serviço.
A `factory()` chama a `provider()`.

### service()

É um _wrapper_ em torno da função `factory()`.
A função passada como parâmetro é tratada como um construtor.

### value()

Também é um _wrapper_ em torno da função `factory()`.

### constant()

É diferente das demais, pois não chama a `factory` nem a `provider`.