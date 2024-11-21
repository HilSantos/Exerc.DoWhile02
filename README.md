# Exerc.DoWhile02
Calculadora com Do While

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ExercicioDoWhile02
{
    public class Program
    {
        static void Main(string[] args)
        {
            //Do While e Calculadora

  int opcao;
            do
            {
                Console.WriteLine("Escolha uma operação:");
                Console.WriteLine("1. Adição");
                Console.WriteLine("2. Subtração");
                Console.WriteLine("3. Multiplicação");
                Console.WriteLine("4. Divisão");
                Console.WriteLine("5. Sair");
                Console.Write("Opção: ");
                opcao = int.Parse(Console.ReadLine());

  //Para sair
                if (opcao == 5) break;

  //Solicitar os valores e declarar as variaveis
                Console.WriteLine("Digite o valor 1: ");
                double val1 = Convert.ToDouble(Console.ReadLine());

  Console.WriteLine("Digite o valor 2: ");
                double val2 = Convert.ToDouble(Console.ReadLine());

  //Verificação das opções
                switch (opcao)
                {
                    case 1: 
                        Console.WriteLine($"Efetuando a Adição: {val1+val2}");
                        break;
                    case 2: 
                        Console.WriteLine($"Efetuando a Subtração: {val1-val2}");
                        break;
                    case 3: 
                        Console.WriteLine($"Efetuando a Multiplicação: {val1*val2}");
                        break;
                    case 4:
                        if (val2 != 0)
                            Console.WriteLine($"Efetuando a Divisão: {val1/val2}");
                        else
                            Console.WriteLine("Erro: Não há divisão por zero!");
                        break;
                    default:
                        Console.WriteLine("Escolha uma das poções validas!");
                        break;

  }

  } while (true);

  }
  }
   }
