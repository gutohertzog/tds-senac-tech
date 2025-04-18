# Operações Relacionais

Vamos imaginar que você precise verificar se um número digitado pelo usuário é positivo ou negativo. Como poderíamos verificar isto? Através de uma operação relacional. As operações relacionais também são nossas conhecidas da Matemática. Em algoritmos, os operadores relacionais são importantes, pois permitem realizar comparações que terão como resultado um valor lógico (*verdadeiro* ou *falso*).

Os símbolos que usamos para os operadores também mudam um pouco em relação ao que usamos no papel. Os símbolos para diferente, maior ou igual e menor ou igual mudam pois não existem nos teclados convencionais. A tabela a seguir mostra todas as operações relacionais e os símbolos que o Portugol utiliza.
| Operação | Símbolo |
| :----: | :----: |
| Maior | > |
| Menor | < |
| Maior ou igual | >= |
| Menor ou igual | <= |
| Igual | == |
| Diferente | != |

A tabela a seguir apresenta a estrutura de algumas dessas operações.
| Operação | Resultado |
| :----: | :----: |
| 3 > 4 | Falso |
| 7 != 7 | Falso |
| 9 == 10 - 1 | Verdadeiro |
| 33 <= 100 | Verdadeiro |
| 6 >= 5 + 1 | Verdadeiro |
| 5 + 4 <= 11 - 2 | Verdadeiro |

Nos dois últimos exemplos, temos [operadores aritméticos](operadores-aritmeticos.md) e [relacionais juntos](operadores-relacionais.md). Nestes casos, realiza-se primeiro a operação aritmética e depois a relacional.

Em geral, as operações relacionais são utilizadas em conjunto com as Estruturas de Controle.

Veja a sintaxe :

```portugol
// estrutura de controle: "se (...)", operação relacional: "5 > 3"
se (5 > 3)
{
    // conjunto de comandos se for verdadeiro
}
```

Para melhor compreensão deste conceito, confira o exemplo abaixo :

```portugol
programa
{
    funcao inicio()
    {
        // comparação entre valor A e B utilizando o operador maior que
        inteiro a = 5, b = 3
        se(a > b){
            escreva("A é maior que B")
        }

        // comparação entre A e B utilizando o operador igual a
        se(a == b){
            escreva("A é igual a B")
        }

        // comparação entre A e B utilizando o operador maior ou igual a
        se(a >= b){
            escreva("A é maior ou igual a B")
        }

        // nos testes acima somente o primeiro teste A > B é verdadeiro,
        // deste modo somente esta mensagem será exibida
    }
}
```

## precedência dos operadores

| prioridade | operador símbolo | operador nome | tipo operador |
| :----: | :----: | :----: | :----: |
| 1 | `()` | parênteses | operadores aritméticos |
| 2 | `*`<br>`/`<br>`%` | multiplicaçao<br>divisão<br>módulo | operadores aritméticos |
| 3 | `+`<br>`-` | soma<br>subtração | operadores aritméticos |
| 4 | `==`<br>`>`<br>`<`<br>`>=`<br>`<=`<br>`!=` | igual a<br>maior que<br>menor que<br>maior ou igual a<br>menor ou igual a<br>diferente de | operadores relacionais |
