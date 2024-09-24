# csharp-documentation
Aqui está uma documentação sobre meus estudos em .NET e C#! \o/  =)

<h1>LINQ</h1>

LINQ significa <strong>Language Integrated Query</strong>, ou seja, Consulta Integrada à Linguagem. 

Isso significa que com essa ferramenta, <strong>conseguimos fazer consultas/pesquisas/queries como se estivéssemos usando a linguagem SQL, mas de maneira integrada à linguagem C#</strong>.

Aqui está um exemplo:

\`\`\`csharp

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

\`\`\`

