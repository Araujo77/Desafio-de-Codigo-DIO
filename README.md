#1º Desafio JAVA

       // new Scanner (System.in): criar um leitor de Enrtadas, com métodos úteis com prefixo "next";
       // System.out.println:. imprime um texto de Saída (Output) e pulando uma linha.

import java.util.Sacanner;

public class Desafio {
  public static void main (String[] args) {
  
     //Lê os valores de Entrada:
  Scanner leitorDeEntrada = new Scanner(System.in);
  float valorSalario = leitorDeEntradas.nextFloat ();
  float valorBeneficios = leitorDeEntradas.nextFloat ();

  float valorInposto = 0;
  if (valorSalario >= 0 && valorSalario <= 1100) {
  
     //Atribui a aliquota de 5% meante o salário:
   valorImposto = 0.05F * valorSalario;
    } else if (valorSalario >= 1100.01 && valorSalario <= 2500.00) {
    valorImposto = 0.10F * valorSalario;
    } else {
    valorImposto = 0.15F * valorSalario;
    }
    

  //Calcula e imprime a Saída (com 2 casas decimais)
    float saida = valorSalario - valorImposto + valorBeneficios;
    System.out.println(String.format("%.2f", saida ));
    }
    }


#2º Desafio C#

using System;

public class Desafio 
{
  public static void Main () 
  {
  //Lê os valores de Entrada:
  float valorSalario = float.Parse(Consle.ReasLine());
  float valorBeneficios = float.Parse(Consle.ReasLine());

  float valorInposto = 0;
  if (valorSalario >= 0 && valorSalario <= 1100)
  {
    //Atribui a aliquota de 5% meante o salário:
    valorImposto = 0.05F * valorSalario;
    } 
    else if (valorSalario >= 1100.01 && valorSalario <= 2500.00)
    {
    valorImposto = 0.10F * valorSalario;
    } 
    else 
    {
    valorImposto = 0.15F * valorSalario;
    }

  //Calcula e imprime a Saída (com 2 casas decimais)
    float saida = valorSalario - valorImposto + valorBeneficios;
    Console.WriteLine(saida.ToString("0.00"));
    }
    }

  
#3º Desafio JavaScript

    // nDesafio JavaScript na DIO tem funções "gets" e "print" acessiveis globalmente:
    // - "gets": L~e UMA linha com dados(s) de entrada (inputs) do usuário;
    // - "print": imprime um texto de saída (output), pulando linha.
  
     //Lê os valores de Entrada:
  
  const valorSalario = parseFloat (gets());
  const valorBeneficios = parseFloat(gets());

    // Calcula o imposto através da função "calcularImposto":
const valorImposto = calcularImposto(valorSalario);

    // Calcula e imprime a Saída (com 2 casas decimais):
 const saida = valorSalario - valorImposto + valorBeneficios;
 print (saida.toFixed(2));
  
    // Função útil para o calculo do imposto (baseado nas aliquotas).
    
function calcularImposto(salario) {
Let aliquota;
if (salario >= 0 && salario <= 1100) {
aliquota = 0.05;
}

    //TODO Criar as demais condições para as aliquotas de 10.00% e 15.00%.
return aliquota * salario;
}



#4º Desafio Python

Para ler e escrever dados em Python, utilizamos as seguintes funções:
- input: Lê UMA linha com dado (s) de Entrada do usuário;
- print: imprime um texto de Saída (Output), pulando linha.


      #Função útil para o calculo do imposto (baseado nas aliquotas).
def calcular_imposto (salario):
aliquota = 0.00
if (salario >= 0 and salario <= 1100):
aliquota = 0.05
elif (salario >= 1100.01 and salario <= 1100):
aliquota = 0.10
else:
aliquota = 0.15
return aliquota * salario

    #Lê os valores de Entrada:
valor_salario = float (input())
valor_beneficios = float(input())

    #Calcula o imposto através da função "calcular_imposto":
valor_imposto = calcular_imposto(valor_salario)

    #Calcular e imprime a Saída ( com 2 casas decimais):
saida = valor_salario - valor_imposto + valor_beneficios
print(f' {saida:.2f}')



 # Simplificando a Orientação a Objetos com Kotlin 

 object ReceitaFederal {
  fun calcularImposto (salario: Double): Double {
   val aliquota = when {
    (salario >= 0 && salario <= 1100)  -> 0.05
     (salario >= 1100.01 && salario <= 1100)  -> 0.05
     else  -> TODO ("Criar as condições para as aliquotas de 10.00% e 15.00%")
     }
     return aliquota * salario
        }
     }
     fun main() {
val valorSalario = readLine()!!.toDouble();
val valorBeneficios = readLine()!!.toDouble();

val valorImposto = ReceitaFederal.calcularImposto(valorSalario);
val saida = valorSalario -valorImposto + valorBeneficios;

println (String.format("%.2f", saida));
     }


     

