# ejercicios_arrays_clases
 Practica 4
 
 //1. Un programa que pida al usuario 4 números, los memorice (utilizando un array), calcule su media aritmética y después muestre en pantalla la media y los datos tecleados.
using System;

namespace Practica_4
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] num = { 1, 2, 3, 4 };
            
           Console.WriteLine("\nIngrese 4 numeraciones\n");

            Console.WriteLine("\nPrimera Numeracion\n");
            num[0] = int.Parse(Console.ReadLine());

            Console.WriteLine("\nSegunda Numeracion\n");
            num[1] = int.Parse(Console.ReadLine());

            Console.WriteLine("\nTercera Numeracion\n");
            num[2] = int.Parse(Console.ReadLine());

            Console.WriteLine("\nCuarta Numeracion\n");
            num[3] = int.Parse(Console.ReadLine());

            Console.Clear();

            for (int contador = 0; contador < num.LongLength; contador++)
            
            {
                Console.WriteLine("Numeracion: " + contador + "\nNumeros Ingresados\n " + num[contador]);
                           
                int Resultado;
                Resultado = (num[0] + num[1] + num[2] + num[3] /4);

                Console.WriteLine("Media Aritmetica: " + Resultado);
                            
            }

            Console.ReadKey();
        }
    }
}









//2. Un programa que pida al usuario 5 números reales (pista: necesitarás un array de "float") y luego los muestre en el orden contrario al que se introdujeron.


using System;

namespace Practica_4
{
    class Program
    {
        static void Main(string[] args)
        {
            float[] num = new float[5];

            Console.WriteLine("\nIngresa 5 Digitos:\n ");

            Console.WriteLine("Primer Digito: ");
            num[0] = float.Parse(Console.ReadLine());

            Console.WriteLine("Segundo Digito: ");
            num[1] = float.Parse(Console.ReadLine());

            Console.WriteLine("Tercer Digito: ");
            num[2] = float.Parse(Console.ReadLine());

            Console.WriteLine("Cuarto Digito: ");
            num[3] = float.Parse(Console.ReadLine());

            Console.WriteLine("Quinto Digito: ");
            num[4] = float.Parse(Console.ReadLine());

            Console.WriteLine("Orden inverso de los digitos ingresados: ");       
           
            Console.WriteLine("1. " + num[4]);
            Console.WriteLine("2. " + num[3]);
            Console.WriteLine("3. " + num[2]);
            Console.WriteLine("4. " + num[1]);
            Console.WriteLine("5. " + num[0]);

        }
    }
}

















//3. Un programa que almacene en un array el número de días que tiene cada mes (supondremos que es un año no bisiesto), pida al usuario que le indique un mes (1=enero, 12=diciembre) y muestre en pantalla el número de días que tiene ese mes.



using System;

namespace Practica_4
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] dias = new int[12] { 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31 };
            int Ene, Feb, Mar, Abr, May, Jun, Jul, Ago, Sep, Oct, Nov, Dic;

            Ene = dias[0];
            Feb = dias[1];
            Mar = dias[2];
            Abr = dias[3];
            May = dias[4];
            Jun = dias[5];
            Jul = dias[6];
            Ago = dias[7];
            Sep = dias[8];
            Oct = dias[9];
            Nov = dias[10];
            Dic = dias[11];

            string datos = null;

            Console.WriteLine("\nElija un mes y le mostrara la cantidad de dias que tiene cada mes del año 2021:\n " +
            "\n1. Enero\n" +
            "\n2. Febrero\n" +
            "\n3. Marzo\n" +
            "\n4. Abril\n" +
            "\n5. Mayo\n" +
            "\n6. Junio\n" +
            "\n7. Julio\n" +
            "\n8. Agosto\n" +
            "\n9. Septiembre\n" +
            "\n10. Octubre\n" +
            "\n11. Noviembre\n" +
            "\n12.Diciembre\n");

            datos = Console.ReadLine();
            Console.WriteLine("Opcion: " + datos);

            switch (datos)
            {

                case "1":
                    Console.WriteLine("Enero " + Ene + " Dias");
                    break;

                case "2":
                    Console.WriteLine("Febrero " + Feb + " Dias");
                    break;

                case "3":
                    Console.WriteLine("Marzo " + Mar + " Dias");
                    break;

                case "4":
                    Console.WriteLine("Abril " + Abr + " Dias");
                    break;

                case "5":
                    Console.WriteLine("Mayo " + May + " Dias");
                    break;

                case "6":
                    Console.WriteLine("Junio " + Jun + " Dias");
                    break;

                case "7":
                    Console.WriteLine("Julio " + Jul + " Dias");
                    break;

                case "8":
                    Console.WriteLine("Agosto " + Ago + " Dias");
                    break;

                case "9":
                    Console.WriteLine("Septiembre " + Sep + " Dias");
                    break;

                case "10":
                    Console.WriteLine("Octubre " + Oct + " Dias");
                    break;

                case "11":
                    Console.WriteLine("Noviembre " + Nov +" Dias");
                    break;

                case "12":
                    Console.WriteLine("Diciembre " + Dic + " Dias");
                    break;


            }
            Console.ReadKey();    












//4. Un programa que pida al usuario 10 números y luego calcule y muestre cuál es el mayor de todos ellos.

using System;

namespace Practica_4
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] numeros = new int[10];
            int i, mayor = 0, d = 0;
            for (i = 0; i < 10; i++)
            {
                Console.WriteLine("Digite valores {0}: ", (i+1));
                numeros[i] = int.Parse(Console.ReadLine()); 

            }
            while (d < 10)
            {
                if (numeros[d] > mayor)
                    mayor = numeros[d];
                d++;
            }

            Console.WriteLine("El mayor de los numeros ingresados es: {0}", mayor);
            Console.ReadKey();
                 
        }
    }
}


//7. Un programa que te pida tu nombre y lo muestre en pantalla separando cada letra de la siguiente con un espacio. Por ejemplo, si tu nombre es "Moreta", debería aparecer en pantalla "M o r e t a".


using System;

namespace Practica_4
{
    class Program
    {
        static void Main(string[] args)
        {
            string nombre;
            
            Console.WriteLine("\nInserte su nombre:\n ");
            nombre = Console.ReadLine();

            foreach(var letras in nombre)
            {
                Console.Write(letras + " ");
            }

            Console.ReadKey();
                               
        }
    }
}




8. Crear un programa que defina un array de 5 elementos de tipo float que representen las alturas de 5 personas. Obtener el promedio de las mismas. Contar cuántas personas son más altas que el promedio y cuántas más bajas.

using System;

namespace AA
{
    class Program
    {
        static void Main(string[] args)
        {

            float[] altura;
            altura = new float[5];
            float promedio;
            for(int i=0; i<5; i++)
            
            {
                Console.WriteLine("Ingrese la altura de la persona: ");
                string datos = Console.ReadLine();
                altura[i] = float.Parse(datos);

            }

            float suma;
            suma = 0;
            for(int i = 0; i < 5; i++)
            {
                suma = suma + altura[i];
            }

            promedio = suma / 5;
            Console.WriteLine("Promedio de alturas: " + promedio);

            int mayor, menor;
            mayor = 0;
            menor = 0;

            for(int i = 0; i < 5; i++)
            {
                if (altura[i] > promedio)
                {
                    mayor++;
                }
                else
                {
                    if (altura[i] < promedio)
                    {
                        menor++;
                    }
                }

            }
            Console.WriteLine("Cantidad de personas mayores al promedio: " + mayor);
            Console.WriteLine("Cantidad de personas menores al promedio: " + menor);

            Console.ReadKey();
        }
    }
}




//9. Crear una clase que permita ingresar valores enteros por teclado y nos muestre la tabla de multiplicar de dicho valor. Finalizar el programa al ingresar el -1.



using System;

namespace AA
{
    class Program
    {
        static void Main(string[] args)
        {

            int valor;
            
            Console.WriteLine("Ingrese un valor: ");
            valor = int.Parse(Console.ReadLine());

            if (valor != -1)
                    
          
            Console.WriteLine("Multiplicacion del valor ingresado: ");

            for (int i = valor; i <= valor * 10; i = i + valor)
            {
                Console.Write(i + "-");
            }

            Console.ReadKey();

        }
    }
}





//10. Confeccionar una clase que permita carga el nombre y la edad de una persona. Mostrar los datos cargados. Imprimir un mensaje si es mayor de edad (edad>=18).

using System;

namespace AA
{
    class Program
    {
        static void Main(string[] args)
        {

            string nombre;
            int edad;

            Console.WriteLine("Ingresa su nombre: ");
            nombre = Console.ReadLine();

            Console.WriteLine("Ingresa tu edad: ");
            edad = int.Parse(Console.ReadLine());


            Console.WriteLine("Datos de la persona:\n " + "\nNombre: "+ nombre + "\n" + "\nEdad: " + edad);

            if (edad >= 18) 
            {
                Console.WriteLine("\nEsta persona es mayor de edad");

            }
            else 
            {
                Console.WriteLine("\nEsta persona no es mayor de edad");

            }

            Console.ReadKey();                               
                           
        }
    }
}


