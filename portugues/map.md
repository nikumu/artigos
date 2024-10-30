# Introdução ao Map em JavaScript

**Map** em JavaScript é uma estrutura de dados que armazena pares de chave-valor, assim como objetos. Porém, enquanto objetos limitam as chaves a strings ou símbolos, Map permite que as chaves sejam de qualquer tipo, como números, objetos, ou até mesmo funções. Essa característica proporciona mais flexibilidade e controle ao manipular dados.

Aqui está um exemplo básico de como criar um Map, adicionar valores, e acessá-los:

```javascript
// Criando um Map
const frutas = new Map();

// Adicionando valores
frutas.set("maçã", 5);
frutas.set("laranja", 10);

// Acessando valores
console.log(frutas.get("maçã")); // Saída: 5
console.log(frutas.get("laranja")); // Saída: 10
```

No exemplo acima, usamos **.set()** para adicionar pares de chave-valor e **.get()** para recuperar o valor de uma chave específica.

Além disso, podemos verificar se uma chave existe em um Map usando o método **.has()**, e também podemos saber o total de pares chave-valor com **.size**:

```javascript
// Verificando se uma chave existe
console.log(frutas.has("maçã")); // Saída: true
console.log(frutas.has("banana")); // Saída: false

// Verificando o tamanho do Map
console.log(frutas.size); // Saída: 2
```

Também é possível usar o forEach para iterar sobre os elementos de um Map. Assim, podemos exibir todos os pares chave-valor:

```javascript
frutas.forEach((valor, chave) => {
  console.log(`Fruta: ${chave}, Quantidade: ${valor}`);
});
// Saída:
// Fruta: maçã, Quantidade: 5
// Fruta: laranja, Quantidade: 10
```

Map é ideal para situações em que precisamos manter a ordem de inserção e queremos usar chaves não restritas a strings. Ele facilita o gerenciamento de dados complexos, proporcionando uma maneira eficiente de armazenar e acessar informações.
