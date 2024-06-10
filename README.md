# Java

Java é uma linguagem de programação amplamente usada para codificar aplicações Web. Ela tem sido uma escolha popular entre os desenvolvedores há mais de duas décadas, com milhões de aplicações Java em uso hoje. Java é uma linguagem multiplataforma, orientada a objetos e centrada em rede que pode ser usada como uma plataforma em si. É uma linguagem de programação rápida, segura e confiável para codificar tudo, desde aplicações móveis e software empresarial até aplicações de big data e tecnologias do servidor.

## <a name=“Convenção”><a/> Convenção de código:
A convenção de código do Java é um conjunto de regras recomendadas para escrever código Java que é fácil de ler, entender e manter. Essas regras foram definidas pela Oracle, a empresa que mantém a linguagem Java, e são amplamente seguidas pela comunidade de desenvolvedores Java.

Aqui estão algumas das principais convenções de código do Java:

- Nomes de classes devem começar com letra maiúscula e usar a convenção PascalCase (também conhecida como Upper CamelCase).
  - Exemplo: ` MinhaClasse `
- Nomes de métodos devem começar com letra minúscula e usar a convenção camelCase.
  - Exemplo: ` meuMetodo() `
- Nomes de constantes devem ser totalmente em letras maiúsculas, separadas por underline.
  - Exemplo: ` MINHA_CONSTANTE `
- Nomes de variáveis devem começar com letra minúscula e usar a convenção camelCase.
  - Exemplo: ` minhaVariavel ` 
- Todas as linhas de código devem ter no máximo 80 caracteres de largura para facilitar a leitura.
- Recomenda-se usar espaços em branco para separar operadores, palavras-chave e elementos de controle de fluxo.
  - Exemplo: ` if (condicao) { ` 
- Use comentários para documentar seu código, explicando o que ele faz e por que ele faz isso. Comentários devem ser claros e concisos.
> [!CAUTION]
> Esse ponto anterior, referente aos comentários, é polêmico, pois muitas pessoas desenvolvedoras consideram que um bom código deve ser autoexplicativo. Se você utiliza nomes intuitivos e descritivos para suas variáveis e métodos, fica mais claro de entender o que está acontecendo no código, dispensando a necessidade de uso de comentários.

Essas são apenas algumas das convenções de código mais comuns no Java. Seguir essas regras pode tornar seu código mais fácil de ler e entender, o que pode economizar tempo e esforço no longo prazo.

É importante lembrar que as convenções de código são apenas **recomendações** , e não regras obrigatórias. No entanto, seguir essas convenções pode ajudar a criar um padrão consistente em todo o seu código Java e também torná-lo mais fácil de compartilhar e colaborar com outros desenvolvedores.

## <a name=“tiposPrimitivos”><a/> Tipos primitivos:
Em Java, assim como na maioria das linguagens de programação, existem os tipos primitivos, que são os tipos de dados mais básicos e fundamentais da linguagem. Eles são utilizados para representar valores simples e são definidos pela própria linguagem.

Java possui oito tipos primitivos diferentes: boolean, byte, char, short, int, long, float e double. Cada um desses tipos possui suas próprias características e faixa de valores permitidos, conforme será descrito a seguir.

- boolean: O tipo boolean é utilizado para representar valores lógicos, podendo assumir apenas dois valores: true ou false. É utilizado em expressões condicionais, loops e outros casos onde se deseja avaliar se uma determinada condição é verdadeira ou falsa.

- byte: O tipo byte é utilizado para representar valores numéricos inteiros de 8 bits. Ele possui uma faixa de valores de -128 a 127.

- char: O tipo char é utilizado para representar caracteres individuais. Ele pode armazenar qualquer caractere Unicode e é representado por aspas simples ('').

- short: O tipo short é utilizado para representar valores numéricos inteiros de 16 bits. Ele possui uma faixa de valores de -32.768 a 32.767.

- int: O tipo int é utilizado para representar valores numéricos inteiros de 32 bits. É um dos tipos de dados mais utilizados para representar números inteiros em Java e possui uma faixa de valores de -2.147.483.648 a 2.147.483.647.

- long: O tipo long é utilizado para representar valores numéricos inteiros de 64 bits. Ele é utilizado para representar valores inteiros muito grandes e possui uma faixa de valores de -9.223.372.036.854.775.808 a 9.223.372.036.854.775.807.

- float: O tipo float é utilizado para representar valores numéricos de ponto flutuante, ou seja, valores com casas decimais, sendo que ocupa 32 bits de memória. Ele pode representar números decimais com até sete dígitos e tem uma precisão limitada, o que significa que ele pode arredondar os números se eles forem muito grandes ou muito pequenos.

- double: O tipo double é similar o float, entretanto ele ocupa 64 bits de memória e pode representar números decimais com até 15 dígitos.

## Casting:

Casting é um recurso utilizado em Java para converter um tipo de dado em outro. Essa conversão pode ser feita de forma automática pelo compilador (conversão implícita), quando o tipo de dado de destino é compatível com o tipo de dado de origem, ou de forma manual (conversão explícita), utilizando o operador de casting.

O casting é utilizado para permitir que tipos de dados incompatíveis possam ser utilizados em uma mesma operação ou expressão. Por exemplo, se um método espera um parâmetro do tipo int e o valor que se deseja passar é do tipo double, é necessário fazer um casting para converter o valor em int.

### Casting implícito

O casting implícito é realizado automaticamente pelo compilador quando o tipo de dado de origem é compatível com o tipo de dado de destino. Por exemplo, é possível atribuir um valor de tipo int a uma variável do tipo double, pois o tipo double é maior e suporta todos os valores que o tipo int pode armazenar:

```
int x = 10;
double y = x; // casting implícito
```

### Casting explícito
O casting explícito é realizado quando o tipo de dado de origem é incompatível com o tipo de dado de destino. Nesse caso, devemos utilizar o operador de casting para realizar a conversão:

```
double x = 10.5;
int y = (int) x; // casting explícito
```

No exemplo anterior, o valor da variável x é convertido em um valor inteiro utilizando o casting explícito. É importante notar que, neste caso, a parte decimal será descartada e o valor atribuído à variável y será 10.

Abaixo tem uma tabela, onde você pode visualizar mais facilmente as conversões que são implícitas e as que necessitam ser feitas de forma explícita.
<div align="center">
  <img width="50%" title="Tabela de conversões implícitas/explicitas" src="https://github.com/Arthur-Sena/Java/assets/57300757/6f02c7d3-d59d-42a0-b050-cfd77ae86625)"/>
</div>

## Para saber mais: a classe Scanner:

A classe Scanner do Java é utilizada para ler dados de entrada em um programa Java. Esses dados podem ser lidos a partir de várias fontes de entrada, como arquivos, fluxos de entrada, Strings e até mesmo a entrada do usuário através do teclado, como vimos em aula.

Ela oferece uma série de métodos para ler dados de diferentes tipos, como inteiros, números de ponto flutuante, strings e caracteres.

Para utilizar a classe Scanner, primeiro é necessário importá-la no início do seu programa. Provavelmente ao incluir a mesma no código, a IDE já vai sugerir o import. Esse import ficará como descrito abaixo:
```
import java.util.Scanner;
```

Veja um exemplo básico de como utilizar a classe Scanner para ler dados distintos:

```
public class ExemploScanner {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite seu nome: ");
        String nome = scanner.nextLine();
        System.out.print("Digite sua idade: ");
        int idade = scanner.nextInt();
        System.out.print("Digite o valor que pretende investir esse mês: ");
        double valor = scanner.nextDouble();

        System.out.println(nome + " que tem " + idade + " anos, irá investir R$ " + valor + " esse mês.");

        scanner.close();
    }
}
```

Nesse exemplo, primeiro importamos a classe Scanner e, em seguida, criamos uma instância dela passando o objeto `System.in` como parâmetro para indicar que queremos ler a entrada do usuário pelo teclado.

Depois, usamos o método `nextLine()` para ler uma linha de texto. Além desse, utilizamos também o `nextInt()` para ler um número inteiro e o `nextDouble()` para ler um número decimal.

Você pode encontrar a lista completa de métodos na [documentação oficial do Java](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Scanner.html).

## Classes e objetos

Uma classe é uma estrutura que define um tipo de objeto. A classe é como um molde, que define quais são as características (atributos) e comportamentos (métodos) que os objetos desse tipo vão possuir. Por exemplo, podemos definir uma classe chamada `Pessoa` que tenha os atributos `nome` e `idade`, além do método `fazAniversario()`

A sintaxe para definir essa classe em Java é a seguinte:
```
public class Pessoa {

    String nome;
    int idade;
    
    void fazAniversario() {
      idade++;
    }

}
```

Já um objeto, é uma instância de uma classe, sendo por meio dele que conseguimos representar informações na aplicação, pois a classe serve apenas para padronizar os objetos, mas não para representar um objeto em si. Para criar um objeto em Java, precisamos utilizar a palavra reservada new seguida do nome da classe e de parênteses vazios. Por exemplo, para criar um objeto do tipo Pessoa, podemos escrever o seguinte código:

```
Pessoa pessoa1 = new Pessoa();
```

Nesse exemplo, criamos um objeto a partir da classe Pessoa, e guardamos na variável pessoa1 uma referência a ele. Como esse objeto foi criado como sendo do tipo Pessoa, ele possui os atributos nome e idade, além do método fazAniversario(). É a partir do objeto que podemos de fato representar uma pessoa, ou seja, preencher os atributos e chamar os métodos. Por exemplo:

```
Pessoa pessoa1 = new Pessoa();

pessoa1.nome = "Ana";
pessoa1.idade = 20;

System.out.println(pessoa1.nome + " tem " + pessoa1.idade + " anos");

pessoa1.fazAniversario();

System.out.println("A idade agora é: " +pessoa1.idade);
```

Podemos criar vários objetos do tipo Pessoa, sendo que todos eles terão os mesmos atributos e métodos, já que são da mesma classe, mas cada um pode possuir informações distintas. Por exemplo:

```
Pessoa pessoa1 = new Pessoa();

pessoa1.nome = "Ana";
pessoa1.idade = 20;

System.out.println(pessoa1.nome + " tem " + pessoa1.idade + " anos");

pessoa1.fazAniversario();

System.out.println("A idade agora é: " +pessoa1.idade);

Pessoa pessoa2 = new Pessoa();

pessoa2.nome = "Carlos";
pessoa2.idade = 20;

System.out.println(pessoa2.nome + " tem " + pessoa2.idade + " anos");

pessoa2.fazAniversario();

System.out.println("A idade agora é: " +pessoa2.idade);
```
