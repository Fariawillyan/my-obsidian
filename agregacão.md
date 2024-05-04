Agregação -> vinculo fraco do objeto principal e forte das partes, exemplo:

public class Venda {

String nome;
String sobrenome;
String email;

*Vendedor vendedor;*
*Produto produto;*
*Comprador comprador;*

}

Isso ocorre porque uma classe usa outras classes utilizadas que participam da classe principal, mas a classe principal não contém estas classes utilizadas como sendo partes suas.