Composicão -> vinculo forte da classe principal e fraco das partes, exemplo:

Class Branco{
String nome;
String email;

*ContaCorrente contaCorrente;*
*Poupanca Poupanca;*

}

No caso da composição, se o objeto principal for destruido, todas os objetos "poupanca" e "conta corrente " deverão ser destruidos: