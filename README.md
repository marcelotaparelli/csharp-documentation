# csharp-documentation
Aqui está uma documentação sobre meus estudos em .NET e C#! \o/  =)



<br><br><br><br><br><br>

<h1>.NET</h1>

O .NET é uma PLATAFORMA de desenvolvimento gratuita, de código aberto e multiplataforma (funciona em Windows, Linux e macOS) criada pela Microsoft. 

Ela permite que desenvolvedores criem uma ampla variedade de aplicativos, incluindo aplicativos web, móveis, de desktop, jogos, IoT (Internet das Coisas), serviços em nuvem e microserviços.

<br><br>

<h2>Mas o que é uma plataforma?</h2>

Um plataforma <strong>é um ambiente que fornece as ferramentas, bibliotecas e recursos necessários para criar, desenvolver e executar aplicativos e serviços</strong>. 

Ela serve como uma base sobre a qual os desenvolvedores podem construir soluções tecnológicas. Java e Node.js também são plataformas de desenvolvimento.

<br><br>


<h2>Principais Componentes do .NET</h2>

.NET Runtime: O runtime, como o Common Language Runtime (CLR), gerencia a execução de aplicativos .NET, incluindo coleta de lixo, segurança de tipos e gerenciamento de memória.

Bibliotecas: O .NET inclui uma vasta coleção de bibliotecas reutilizáveis, conhecidas como Framework Class Library (FCL), que fornecem funcionalidades comuns como manipulação de strings, acesso a dados, e muito mais.

SDK (Software Development Kit) e Ferramentas: O .NET SDK inclui ferramentas para compilar, construir e monitorar aplicativos .NET. Ferramentas como o Visual Studio e o Visual Studio Code oferecem ambientes de desenvolvimento integrados (IDEs) para facilitar o desenvolvimento. O Runtime do .NET está dentro do SDK, ou seja, instalando o SDK do .NET vc instala também o runtime.

Linguagens de Programação: O .NET suporta várias linguagens de programação, incluindo C#, F#, e Visual Basic.

ASP.NET: Um framework específico para o desenvolvimento de aplicativos web e APIs.

Xamarin/.NET MAUI: Ferramentas para o desenvolvimento de aplicativos móveis multiplataforma.

<br><br>


<h2>Características do .NET</h2>

Multiplataforma: Funciona em Windows, Linux e macOS.

Desempenho: Oferece alto desempenho e eficiência.

Segurança: Inclui recursos de segurança robustos.

Escalabilidade: Suporta a criação de aplicativos escaláveis e resilientes.

Comunidade e Suporte: Possui uma grande comunidade de desenvolvedores e é mantido como um projeto de código aberto no GitHub.



<br><br><br><br><br><br>



<h1>STRING METHODS</h1>

<h2>Para saber se a string é nula ou vazia</h2>

Use <strong>string.IsNullOrEmpty(yourString)</strong>

<br><br>

<h2>Para dividir uma string</h2>

Use <strong>suaString.Split('coloque aqui o char que vai ser a referência da divisão')</strong>

<br><br>



<br><br><br><br><br><br>



<h1>ARRAY METHODS</h1>

<h2>Para saber quantos elementos tem uma array</h2>

Use <strong>suaArray.Length</strong>

<br><br>

<br><br>

<h2>Para ordenar uma array</h2>

Use <strong>Array.Sort(yourArray)</strong>

<br><br>

<h2>Para encontrar o valor máximo ou mínimo</h2>

Use <strong>nomeDaSuaArray.Max()</strong> ou <strong>nomeDaSuaArray.Min()</strong>. Estas são funções que precisam de "using System.Linq"

<br><br>

<h2>Para encontrar um valor máximo</h2>

Use <strong>nomeDaSuaArray.Max(função)</strong> exemplo de função para achar a maior length dentro de uma array: str => str.Length)

<br><br>

<h2>Para transformar em uma array</h2>

Use <strong>seuObjeto.ToArray()</strong>

<br><br>

<h2>Para filtrar uma array</h2>

Use <strong>suaArray.Where(função)</strong> exemplo de função para achar as strings que tenham mais de 4 chars: str =: str.Length > 4

<br><br>

<h2>Para conferir se todos os elementos de uma array satisfazem uma condição</h2>

Use <strong>suaArray.All(função)</strong>

<br><br><br><br><br><br>



<h1>INTEGER METHODS</h1>

<h2>Quando precisar que uma variável tenha o menor valor da lógica</h2>

Use <strong>int.MinValue</strong>

<br><br>

<h2>Para fazer o módulo, ou converter no número absoluto</h2>

Use <strong>Math.Abs(seuNumero)</strong>.

<br><br>

<h2>Para transformar uma string em int</h2>

Use <strong>int.TryParse(yourString, out int num)</strong>. A função retorna um bool para sucesso e tem como saída a variável num.



<br><br><br><br><br><br>



<h1>HASHSET</h1>

<h2>Características</h2>

HashSets são similares a Lists mas naturalmente <strong>aceitam apenas valores únicos, não permitindo a duplicação de dados iguais</strong>.

<br><br>

<h2>Para criar</h2>

Use <strong>HashSet&lt;tipoDeVariavel&gt; nome da variavel = new()</strong>

<br><br>

<h2>Para eliminar duplicatas de uma List</h2>

Caso você tenha uma List&lt;string&gt; com dados duplicados, vc pode transformar essa List em HashSet e as duplicatas serão eliminadas, exemplo: <strong>HashSet&lt;string&gt; nomeDoHashSet = new HashSet&lt;string&gt;(nomeDaList)</strong>.

<br><br>

<h2>Métodos</h2>

<h3>Para checar se um valor existe</h3>

Use nomeDoHashSet.Contains("valorQueDesejaConsultar")

<br><br>

<h3>Para unir dois HashSets</h3>

Use nomeDoHashSet1.UnionWith("nomeDoHashSet2")

<br><br>

<h3>Para a intersecção de dois HashSets</h3>

Use nomeDoHashSet1.IntersectWith("nomeDoHashSet2")

<br><br>



<br><br><br><br><br><br>



<h1>LOOPS</h1>

<h2>Interrupções de loops</h2>

Use <strong>break</strong> para parar o loop e <strong>continue</strong> para ir para a próxima iteração.



<br><br><br><br><br><br>


<h1>Dicionário</h1>

<h2>Para criar</h2>

Use <strong>Dictionary<int, string> variableName = new();</strong>.

Para já definir valores use: <br><br>

private Dictionary<string, string> daysOfTheWeek = new ()<br>
{<br>
    { "Segunda-feira" , "Monday" },<br>
    { "Terça-feira" , "Tuesday" },<br>
    { "Quarta-feira" , "Wednesday" },<br>
    { "Quinta-feira" , "Thursday" },<br>
    { "Sexta-feira" , "Friday" }<br>
};<br>

<br><br>

<h2>Para acessar valores e chaves</h2>

Use <strong>seuDicionario.Values</strong> e <strong>seuDicionario.Keys</strong>.

<br><br>

<h2>Para saber se contém alguma chave</h2>

Use <strong>seuDicionario.ContainsKey(chave)</strong>.

<br><br><br><br><br><br>

<h1>LINQ</h1>

LINQ é uma biblioteca da plataforma .NET e significa <strong>Language Integrated Query</strong>, ou seja, Consulta Integrada à Linguagem. 

Isso significa que com essa ferramenta, <strong>conseguimos fazer consultas/pesquisas/queries como se estivéssemos usando a linguagem SQL, mas de maneira integrada à linguagem C#</strong>.

Aqui está um exemplo:

```csharp

using System;
using System.Linq;

class Program
{
    static void Main()
    {
        int[] numeros = { 1, 2, 3, 4, 5, 6 };

        // Consulta LINQ para selecionar números pares
        var numerosPares = from num in numeros
                           where num % 2 == 0
                           select num;

        foreach (var num in numerosPares)
        {
            Console.WriteLine(num); // Saída: 2 4 6
        }
    }
}

```

<br><br><br><br>

<h2>Qual tipo o LINQ retorna?</h2>

O tipo de retorno de uma consulta LINQ depende do tipo de dados que está sendo consultado e das operações realizadas na consulta. Aqui estão alguns exemplos comuns:

<br><br>

<strong>1. IEnumerable<T> </strong> <br>
Quando você consulta uma coleção em memória, como uma lista ou um array, o LINQ geralmente retorna um IEnumerable<T>. Por exemplo:

```csharp

int[] numeros = { 1, 2, 3, 4, 5 };
var numerosPares = numeros.Where(n => n % 2 == 0); // Retorna IEnumerable<int>

```

<br><br>

<strong>2. IQueryable<T> </strong> <br>
Quando você consulta uma fonte de dados que suporta a execução de consultas remotas, como um banco de dados usando Entity Framework, o LINQ retorna um IQueryable<T>. Por exemplo:

```csharp

using (var contexto = new MeuDbContext())
{
    var clientes = contexto.Clientes.Where(c => c.Idade > 18); // Retorna IQueryable<Cliente>
}

```

<br><br>

<strong>3. Tipos Anônimos </strong> <br>
Se a consulta seleciona propriedades específicas ou cria novos objetos, o LINQ pode retornar uma coleção de tipos anônimos. Por exemplo:

```csharp

var resultado = numeros.Select(n => new { Valor = n, Quadrado = n * n }); // Retorna IEnumerable<{ int Valor, int Quadrado }>

```
<br><br>

<strong>4. Tipos Específicos </strong> <br>
Você também pode projetar a consulta para retornar tipos específicos, como listas ou arrays:

```csharp

var listaPares = numeros.Where(n => n % 2 == 0).ToList(); // Retorna List<int>
var arrayPares = numeros.Where(n => n % 2 == 0).ToArray(); // Retorna int[]

```

<br><br><br><br>

<h1>LINQ é uma lib(biblioteca) enquanto ASP.NET é um framework, qual a diferença?</h1>

<br><br>

<h2>Framework</h2>

Um framework é uma estrutura que fornece diretrizes e padrões para o desenvolvimento de uma aplicação completa. 

Ele define a arquitetura da aplicação e oferece funcionalidades prontas que você pode usar. 

O framework controla o fluxo da aplicação e chama o seu código quando necessário. Isso é conhecido como inversão de controle.

Exemplos de Frameworks:

ASP.NET: Para desenvolvimento web.
Angular: Para desenvolvimento de aplicações web front-end.
Spring: Para desenvolvimento de aplicações Java.

<br><br><br><br>

<h2>Biblioteca</h2> 

Uma biblioteca é um conjunto de funções ou métodos que você pode chamar para realizar tarefas específicas. 

Diferente de um framework, você está no controle do fluxo da aplicação e decide quando e onde chamar a biblioteca.

Exemplos de Bibliotecas:

jQuery: Para manipulação de DOM e eventos em JavaScript.
NumPy: Para computação numérica em Python.
D3.js: Para criação de visualizações de dados em JavaScript.

<br><br><br><br>

<h2>Diferença Principal</h2>  

A principal diferença entre um framework e uma biblioteca está na <strong>inversão de controle</strong>:

Framework: O framework chama o seu código. Ele define a estrutura e o fluxo da aplicação.
Biblioteca: Você chama o código da biblioteca. Você controla o fluxo da aplicação.

<h3>Metáfora para Entender Melhor</h3>

Biblioteca: É como ir a uma loja de ferramentas. Você escolhe as ferramentas que precisa e as usa como quiser. <br>
Framework: É como construir uma casa com um conjunto de plantas-baixas. Você segue as diretrizes e padrões definidos pelo framework, mas ainda pode personalizar alguns aspectos.
