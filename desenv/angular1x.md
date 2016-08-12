# Angular 1.x

## Serviços

### provider()

Usa se você precisa configurar o serviço.

### factory()

Se você não precisa configurar o serviço, use a função `factory` que é mais simples de criar o serviço.
A `factory()` chama a `provider()`.

### service()

É um _wrapper_ em torno da função `factory()`.
A função passada como parâmetro é tratada como um construtor.

### value()

### constant()

É diferente das demais, pois não chama a `factory` nem a `provider`.