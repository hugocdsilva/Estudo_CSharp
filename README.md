# Estudo_C#

Estudo de fundamentos:

1. Declare as variáveis nome, idade e nota atribuindo os valores “Paulo”, 17 e 7.5 e exiba a saída no formato :
Aluno <nome> tem <idade> anos e nota <nota> usando a concatenação e a interpolação de strings:

//var nome = "Paulo";
//var idade = 17;
//var nota = 7.5;

/*Console.WriteLine("Aluno "+nome+" tem "+idade+" anos e nota " + nota +".");
Console.WriteLine($"Aluno {nome} tem {idade} anos e nota {nota}.");*/

//Console.WriteLine($"{nome}\n{idade}\n{nota}");


2. Escreva um programa que recebe 3 letras via teclado e as exiba na ordem reversa usando
a concatenação e também a interpolação de strings:

Console.WriteLine("Digite a primeira letras:\n");
string letra1 = Console.ReadLine();
Console.WriteLine();

Console.WriteLine("Digite a segunda letras:\n");
string letra2 = Console.ReadLine();
Console.WriteLine();

Console.WriteLine("Digite a terceira letras:\n");
string letra3 = Console.ReadLine();
Console.WriteLine();

Console.WriteLine("As letras digitadas foram: "+"terceira \""+letra3+"\", "+ "segunda \"" +letra2+ "\", "+ "primeira \"" + letra1 + "\". ");
Console.WriteLine($"As letras digitadas foram: terceira \"{letra3}\", segunda \"{letra2}\", primeira \"{letra1}\".");


3. Escreva um programa para receber dois valores via teclado do tipo double e a seguir
realize as operações de soma, subtração, multiplicação, exponenciação, divisão e módulo
exibindo o resultado:

Console.WriteLine("Escolha o primeiro valor:\n");
double valor1 = double.Parse(Console.ReadLine());
Console.WriteLine();

Console.WriteLine("Escolha o segundo valor:\n");
double valor2 = double.Parse(Console.ReadLine());
Console.WriteLine("_______________________________________");

Console.WriteLine("A operação do primeiro e segundo valores, são:");
Console.WriteLine();
Console.WriteLine($"Soma: {valor1} + {valor2} = {valor1+valor2}");
Console.WriteLine($"Subtração: {valor1} - {valor2} = {valor1-valor2}");
Console.WriteLine($"Multiplicão: {valor1} x {valor2} = {valor1 * valor2}");
Console.WriteLine($"Divisão: {valor1} / {valor2} = {valor1 / valor2}");
Console.WriteLine($"Exponete: {valor1} elevado a {valor2} = {Math.Pow(valor1,valor2)}");
Console.WriteLine($"Módulo: {valor1} % {valor2} = {valor1 % valor2}");


4. Escreva um programa que receba um nome e uma senha via teclado. Nome é uma string e
Senha é um inteiro. Se o nome for igual a ‘admin’ ou ‘maria’ e a senha for igual a ‘123’
então exiba a mensagem ‘Login feito com sucesso’ caso contrário exiba a mensagem ‘Login
inválido’: (use o operador condicional ternário):

int senha = 123;
string nome1 = "admin";
string nome2 = "maria";

Console.WriteLine("Digite o nome de usuário:"); 
string usuario = Console.ReadLine();
Console.WriteLine();

Console.WriteLine("Digite a senha:");
int senhaDigitada = int.Parse(Console.ReadLine());
Console.WriteLine();
Console.WriteLine("_______________________");

if ((usuario == nome1 || usuario == nome2) && senhaDigitada == senha)
{
    Console.WriteLine("Login feito com sucesso");
}
else
{
    Console.WriteLine("Login inválido");
}
Console.WriteLine("_______________________");


5. Escreva um programa que recebe via teclado dois números inteiros x e y e imprima no
console se x é par ou não e se y é par ou não. Use o operador condicional ternário (? :):

Console.WriteLine("Escola um número para representar \"x\":");
int x = int.Parse(Console.ReadLine());
Console.WriteLine();

Console.WriteLine("Escola um número para representar \"y\":");
int y = int.Parse(Console.ReadLine());
Console.WriteLine();

string resultadoX = x % 2 == 0 ? "Par" : "ìmpar";
string resultadoY = y % 2 == 0 ? "Par" : "ìmpar";

Console.WriteLine($"O valor de \"x\" é {resultadoX}, e o valor \"y\" é {resultadoY}.");
