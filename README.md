Console.WriteLine("==========CALCULADORA==========");

Console.WriteLine("Escreva seu primeiro numero: ");
double num1 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Escreva seu segundo numero: ");
double num2 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Digite a operação desejada: + - * / ");
var operacao = Console.ReadLine();

double resultado = 0;

switch (operacao)
{
    case "+":
    resultado = num1 + num2;
    break;

     case "-":
    resultado = num1 - num2;
    break;

     case "*":
    resultado = num1 * num2;
    break;

    case "/":
    if (num2 != 0)
    resultado = num1 / num2;

        else
        {
            Console.WriteLine("operação ivalida, pois nao tem como dividir por zero");
            return;
        }
         break;

            default:
        Console.WriteLine("Operação inválida.");
        return;
}

Console.WriteLine($"Resultado: {resultado}");
