# Prova 2

Há 2 padrões principais implementados nesse projeto. O primeiro é o builder, reperesentado pela classe Builder, que é usado para impedira ambiguidade 
nas chamadas dos construtores da classe Pessoa. Além das vantagens conhecidas do padrão: favorecer o encapsulamento do código, 
permite variar a representação da Pessoa e permite um controle durante a construção do produto.

O outro é o padrão memento, que é utilizado para realizar as funcionalidades undo e redo. É representado pelas classes Memento
e CareTaker. O memento é essencial para o bom funcionamento deste projeto, pois sem ele, a complexidade para realizar as funcionalidades
citadas cresce bastante. A classe Sistema consegue acessar os estados salvos (mementos) através do CareTaker.

Além destes, um padrão facade pode ser considerado, visto que todas as classes são unificadas pela classe Sistema, o que torna mais simples
fazer com que esse projeto se torne uma subrotina de um projeto maior.

Vale ressaltar as heranças entre as classes Pessoa, Horista e Comissionado. Essas duas últimas herdam da primeira. Há polimorfismos
nestas classes também, do método editPessoa()
