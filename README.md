# csharp-documentation
Aqui está uma documentação sobre meus estudos em .NET e C#! \o/  =)

<br><br><br><br>

<h1>LINQ</h1>

LINQ significa <strong>Language Integrated Query</strong>, ou seja, Consulta Integrada à Linguagem. 

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

