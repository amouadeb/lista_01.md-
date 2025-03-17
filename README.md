# lista_01.md-

1- (a) // var x é e inicializado como undefined, então console.log(x); imprime undefined. let y
<br>
2- (a) //A condição if a || b === 0 está errada porque b === 0 esta antes, e a || true sempre será true
<br>
3- (a) // o break impede a execução dos próximos case. Assim, a função retorna 200.
<br>
4- (d) // O código primeiro multiplica cada número por 2, filtra os maiores que 5 6/8/10 e dps soma esses valores 8+10 = 18 + 6 = 24
<br>
5- (c) // Começa na posição 1 ("maçã") tira ("maçã" e "uva") e poem  "abacaxi" e "manga".
<br>
6- (a) // extends usa a herança de classe evitando repetição no codigo
<br>
7- (a) // terceira é falsa I: JavaScript tem sim herança de classes com extends, e o código funciona corretamente. As outras estão corretas
<br>
8- (b) // verdadeiro pois  O polimorfismo deixa os objetos diferentes respondam à mesma mensagem de maneiras distinta, mas falso pois  Em JavaScript, não existe sobrecarga de métodos nativa como em outras linguagens 
<br>
9-
```javascript
function somaArray(numeros) {
    let soma = 0; //  mostra a  variável soma corretamente.

     //'i' precisa ser declarado com 'let' para evitar erro de escopo.
    //  ' correto é 'numeros.length'.
    for (let i = 0; i < numeros.length; i++) { 
        soma += 2 * numeros[i]; // CSomar o dobro dos números  de forma correta
    }

    return soma;
}

console.log(somaArray([1, 2, 3, 4])); // Saída correta: 20
```
<br>
10-

```javascript
// Classe Produto
class Produto {
    constructor(nome, preco) {
        this.nome = nome; // Corrige os nomes dos parâmetros e propriedades.
        this.preco = preco;
    }

    calcularDesconto() {
        return this.preco * 0.9; // Calcula o desconto corretamente.
    }
}

class Livro extends Produto {
    constructor(nome, preco, autor) {
        super(nome, preco); // Corrige os nomes dos parâmetros e propriedades.
        this.autor = autor;
    }

    calcularDesconto() {
        return this.preco * 0.8; // Calcula o desconto específico para livros.
    }
}

const produto1 = new Produto("Cadeira", 100);
console.log(produto1.calcularDesconto()); // Saída: 90

const livro1 = new Livro("JavaScript Básico", 100, "Autor X");
console.log(livro1.calcularDesconto()); // Saída: 80
```
