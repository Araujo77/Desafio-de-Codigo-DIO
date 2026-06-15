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
