# Exercicios revisão Java

1. Overload é a utilização de um mesmo operador, ou metódo, que irá desenvolver diferentes comportamentos
dependendo dos objetos no qual ele está sendo utilizado. Por exemplo, o operador '+' possui uma sobrecarga
para diferentes tipos primitivos de dados, no caso de números(inteiros ou reais) ele significa soma, já
em relação a strings ele significa concatenação de duas strings. Override é a sobreposiççao de um metódo
herdado ou não implementado de uma classe pai ou interface, ou seja, a criação de um comportamento específico
para aquela classe que adquiriu este metódo.
2. O override é necessário toda vez que um metódo é herdado de uma classe pai ou uma interface. Por exemplo,
digamos que exista a classe Animal, e nela contem o método som(). Uma segunda classe Cachorro herda de Animal,
mas o método som() precisa sofrer um override, pois o som de um cachorro é diferente dos outro animais. Caso exista
uma classe Gato que também herda de Animal, o método precisaria sofrer um override.
3. Classes abstratas são classes que, a príncipio, nunca devem ser instanciadas durante a execução do programa. Elas
servem apenas como uma classe base, que servirá com "molde" pra outras classes mais especializadas, que irão compartilhar
alguns atributos e métodos em comum. As classes que herdam da classe abstrata devem ser instanciadas. Imaginemos o seguinte
problema: um empresa precisa de um sistema para monitorar todos os seus funcionários. Nessa empresa existem secretários, gerentes
diretores, e terceirizados. Todos eles possuem em comum um código de identificação, um nome, e onde estão alocados como atributos.
Como métodos, possuem um método de checkin e outro de checkout. Este é um bom exemplo para utilização de uma classe abstrata Funcionário,
englobando todas essas características em comum mostradas acima, e as classes especializadas: Secretário, Gerente, Diretor e Terceirizado
devem herdar esses atributos.
4. Casts são transformações de uma instancia de um objeto para outro. Casts são necessários quando é preciso manter certa coerência na
execução de um programa. Digamos que um programa so trabalhe com números inteiros, fazendo algum tipo de divisão sobre esses valores. Caso
seja fornecido um numero não-inteiro, o cast desse valor n para um inteiro é ncessário para que nao ocorra futuros bugs na execução. Ja o
instanceof é necessário para sabermos qual a instanciação de um determiando objeto(é um int ou um float)
5. Interfaces podem ser comparadas a um tipo de contrato entre as classes que a implementam e a própria interface. Toda classe que implementa
uma interface deve implementar seus métodos. As classes abstratas não requerem esse tipo de comportamento entre as classes filhas. Exemplo
da interface Map do java.
6.
..1. A classe E deve implementar '''java public abstract m2(double x);''', '''java public abstract void m3(String x);'''e '''java public abstract void m4();'''.
..2. A classe D deve implementar '''java public abstract void m1();''', '''java public abstract void m1();''', '''java public abstract void m3(String x);'''
..3. Não, pois a classe E implementa a interface I1(pela herança de A), logo ela pode ser instanciada.
..4. '''java
        I1 x = new D();
        x.m3("5");
        ((A)x).m2(2.0);
        E y = (E)x;
        I2 k = (C)x;
     '''
..5. false, true, true, true, true
