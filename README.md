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
    

    // Calcula e imprime a Saída (com 2 casas decimais)
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

    // Calcula e imprime a Saída (com 2 casas decimais)
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



DESAFIO PROPOSTO (FINAL)

Descrição
O Microsoft Copilot Studio é uma plataforma de criação de assistentes virtuais (bots) com IA generativa, permitindo a automação de processos e a criação de interações naturais com os usuários. Ele combina o poder do Microsoft Copilot com personalizações específicas para empresas.

Neste desafio, você deve associar conceitos do Microsoft Copilot Studio às suas descrições.

Saiba mais em Microsoft Learn: Microsoft Copilot Studio

Entrada
A entrada consistirá em um conceito relacionado ao Microsoft Copilot Studio, para o qual você deve retornar a descrição correspondente.

Os conceitos válidos são:

"Copilot"
"Fluxo de conversação"
"Tópico"
"Conectores"
Saída
A saída esperada é a descrição associada ao conceito. Seguem as possíveis respostas:

"Assistente de IA que interage por meio de conversação"
"Estrutura de diálogo que orienta as interações"
"Bloco de construção de um chatbot no Copilot Studio"
"Integrações para conectar sistemas externos"

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	           Saída
Copilot	           Assistente de IA que interage por meio de conversação
Fluxo de conversação	    Estrutura de diálogo que orienta as interações
Tópico	                  Bloco de construção de um chatbot no Copilot Studio

Atenção: É extremamente importante que as entradas e saídas sejam exatamente iguais às descritas na descrição do desafio de código.

Os desafios apresentados aqui têm como objetivo principal exercitar os conceitos aprendidos e proporcionar um primeiro contato com lógica de programação. Caso não tenha experiência em programação, utilize o template disponível e preencha com os conceitos aprendidos. Para resetar o template, basta clicar em “Restart Code”.
     


Entrega do Desafio

DESAFIO 1

# Leitura da entrada
conceito = input().strip()

# Mapeamento dos conceitos para suas descrições
if conceito == "Copilot":
    print("Assistente de IA que interage por meio de conversação")
    
elif conceito == "Fluxo de conversação":
    print("Estrutura de diálogo que orienta as interações")
    
elif conceito == "Tópico":
    print("Bloco de construção de um chatbot no Copilot Studio")
    
elif conceito == "Conectores":
    print("Integrações para conectar sistemas externos")


Entrega do Desafio

DESAFIO 2

Descrição
No Microsoft Copilot Studio, as respostas podem ser configuradas de diversas formas para fornecer informações úteis aos usuários. Este desafio ajudará a diferenciar os tipos de respostas utilizadas.

Entrada
Os seguintes tipos de respostas são abordados:

"Resposta rápida"
"Cartão adaptável"
"Ação de chamada de API"
"Texto formatado"
Saída
A saída esperada será uma breve descrição de cada tipo de resposta:

"Exibe uma mensagem curta para resposta rápida"
"Permite criar interfaces interativas no chatbot"
"Executa uma requisição externa para obter dados"
"Exibe texto com opções de formatação avançada"

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	              Saída
Resposta rápida	       Exibe uma mensagem curta para resposta rápida
Cartão adaptável	       Permite criar interfaces interativas no chatbot
Ação de chamada de API	Executa uma requisição externa para obter dados

Atenção: É extremamente importante que as entradas e saídas sejam exatamente iguais às descritas na descrição do desafio de código.

Os desafios apresentados aqui têm como objetivo principal exercitar os conceitos aprendidos e proporcionar um primeiro contato com lógica de programação. Caso não tenha experiência em programação, utilize o template disponível e preencha com os conceitos aprendidos. Para resetar o template, basta clicar em “Restart Code”.


Python
# Leitura da entrada
resposta = input()

# Mapeamento dos tipos de resposta para suas descrições
if resposta == "Resposta rápida":
    print("Exibe uma mensagem curta para resposta rápida")
elif resposta == "Cartão adaptável":
    print("Permite criar interfaces interativas no chatbot")
elif resposta == "Ação de chamada de API":
    print("Executa uma requisição externa para obter dados")
elif resposta == "Texto formatado":
    print("Exibe texto com opções de formatação avançada")



DESAFIO 3

Descrição
As ações no Microsoft Copilot Studio permitem que um chatbot execute tarefas específicas, como chamar APIs ou manipular dados. Seu objetivo é associar cada ação à sua funcionalidade.

Entrada
Os seguintes tipos de ações serão considerados:

"Ação de chamada de API"
"Ação de lógica condicional"
"Ação de armazenamento de variável"
"Ação de loop"
Saída
A saída será uma breve explicação de cada ação:

"Chama um serviço externo para buscar ou enviar dados"
"Executa lógica baseada em condições definidas"
"Salva informações temporárias para uso posterior"
"Executa uma tarefa repetidamente até atender um critério"
Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	                         Saída
Ação de chamada de API	           Chama um serviço externo para buscar ou enviar dados
Ação de lógica condicional	           Executa lógica baseada em condições definidas
Ação de armazenamento de variável	    Salva informações temporárias para uso posterior

Atenção: É extremamente importante que as entradas e saídas sejam exatamente iguais às descritas na descrição do desafio de código.

Os desafios apresentados aqui têm como objetivo principal exercitar os conceitos aprendidos e proporcionar um primeiro contato com lógica de programação. Caso não tenha experiência em programação, utilize o template disponível e preencha com os conceitos aprendidos. Para resetar o template, basta clicar em “Restart Code”.



# Leitura da entrada
acao = input().strip()

# Mapeamento das ações para suas funcionalidades
if acao == "Ação de chamada de API":
    print("Chama um serviço externo para buscar ou enviar dados")
    
elif acao == "Ação de lógica condicional":
    print("Executa lógica baseada em condições definidas")
    
elif acao == "Ação de armazenamento de variável":
    print("Salva informações temporárias para uso posterior")
    
elif acao == "Ação de loop":
    print("Executa uma tarefa repetidamente até atender um critério")
