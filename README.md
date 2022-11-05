using System;

namespace ConsoleApp7
{
    class Program
    {
        static void Main(string[] args)
        {

            //Console.WriteLine("Program oblicza pole powierzchni prostokąta");
            //double A, B, C;
            //Console.WriteLine("Podaj bok A: ");
            //A = double.Parse(Console.ReadLine());
            //Console.WriteLine("Podaj bok B: ");
            //B = double.Parse(Console.ReadLine());
            //C = A * B;
            //Console.WriteLine("Pole powierzchni prostokąta o bokach A i B wynosi: "+ C);

            //double r,v;
            //Console.WriteLine("Program oblicza objętość kuli o promieniu podanym przez użytkownika.");
            //Console.WriteLine("Podaj promień kuli: ");
            //r = double.Parse(Console.ReadLine());
            //v = (4* Math.PI * Math.Pow(r,3))/3;
            //Console.WriteLine("Objętość kuli o promieniu {0} wynosi {1}",r,v);

            //try
            //{
            //double euro, pln, kurs;
            //Console.WriteLine("Program przelicza kwotę Euro na Pln, po określonym kursie");
            //Console.WriteLine("Podaj kwotę Euro: ");
            //euro = double.Parse(Console.ReadLine());
            //Console.WriteLine("Podaj kwotę Kurs: ");
            //kurs = double.Parse(Console.ReadLine());
            //pln = euro * kurs;
            //Console.WriteLine("Kwota {0} Euro w przeliczeniu na Pln po kursie {1} wynosi {2} złotych",euro,kurs,pln);
            //}
            //catch (Exception e)
            //{

            //    Console.WriteLine(e);
            //}

            //double liczba;
            //Console.WriteLine("Podaj liczbę: ");
            //liczba = double.Parse(Console.ReadLine());
            //if(liczba < 5)
            //{
            //    Console.WriteLine("Liczba jest mniejsza od 5");
            //}
            //if (liczba > 5)
            //{
            //    Console.WriteLine("Liczba jest większa od 5");
            //}
            //if (liczba == 5)
            //{
            //    Console.WriteLine("Liczba jest równa 5");
            //}

            //double liczba, reszta;
            //Console.WriteLine("Program sprawdza czy liczba jest parzysta");
            //Console.WriteLine("Podaj liczbę: ");
            //liczba = double.Parse(Console.ReadLine());
            //reszta = liczba % 2;
            //if(reszta==0)
            //    Console.WriteLine("Liczba parzysta");
            //else
            //    Console.WriteLine("Liczba nieparzysta");

            //Console.WriteLine("Program rozwiązuje równanie kwadratowe.");
            //  double a, b, c, delta;
            //            Console.WriteLine("Podaj a: ");
            //                a = double.Parse(Console.ReadLine());
            //                if (a == 0)
            //                    Console.WriteLine("To nie jest równanie kwadratowe!");

            //                else
            //                {
            //                    Console.WriteLine("Podaj b: ");
            //                    b = double.Parse(Console.ReadLine());
            //                    Console.WriteLine("Podaj c: ");
            //                    c = double.Parse(Console.ReadLine());
            //                    delta = Math.Pow(b, 2) - 4 * a * c;
            //                    if (delta > 0)
            //                    {
            //                        double x1 = (-b + Math.Sqrt(delta)) / 2 * a;
            //                        double x2 = (-b - Math.Sqrt(delta)) / 2 * a;

            //                    }
            //                    if (delta < 0)
            //                    {
            //                        Console.WriteLine("Nie ma miejsc zerowych!");
            //                    }
            //                    if (delta == 0)
            //                    {
            //                        double x0 = -b / 2 * a;
            //                    }
            //                }
            //        }
            //    }
            //}


            //int a, b, c;
            //bool czyniewlasciwyznak = true;
            //Console.Write("Podaj pierwszą liczbę: ");
            //a = int.Parse(Console.ReadLine());
            //Console.Write("Podaj znak operacji: ");
            //c = char.Parse(Console.ReadLine());
            //Console.Write("Podaj drugą liczbę: ");
            //b = int.Parse(Console.ReadLine());
            //while(czyniewlasciwyznak)
            //{

            //    czyniewlasciwyznak = false;
            //    switch (c)
            //    {
            //        case '+':
            //            Console.WriteLine(a + b);


            //            break;
            //        case '-':
            //            Console.WriteLine(a - b);

            //            break;
            //        case '*':
            //            Console.WriteLine(a * b);

            //            break;

            //        case '/':
            //            Console.WriteLine(a / b);

            //            break;

            //        default:
            //            czyniewlasciwyznak = true;
            //            Console.WriteLine("Podano zły znak działania");
            //            break;
            //    }
            //    break;
            //}
            //Console.WriteLine("Podaj liczbę: ");
            //bool czypierwsza = true;
            
            //uint liczba = uint.Parse(Console.ReadLine());
            //if (liczba <= 1)
            //{
            //    Console.Write("liczba "  + liczba +  " nie jest pierwsza ani zlozona ");
            //}
            //else
            //{
            //    for (uint i = 2; i <= Math.Sqrt(liczba); i++)

            //    {
            //        if (liczba % i == 0)
            //        {
            //            Console.Write("liczba "  + liczba  +  " jest liczbą złożoną podzielną przez " + i);
            //            break;
            //        }
            //    }
            //    if (czypierwsza) Console.Write("liczba " +  liczba  +" jest liczbą pierwszą ");
            //}    
            using System;

////////////namespace ConsoleApp10
{
    class Program
    {
        static void Main(string[] args)
        {
            
            int n = 0;
            while(true)
                {
                Console.WriteLine("Podaj liczbę n: ");
                try
                {
                    n = int.Parse(Console.ReadLine());
                    break;
                }
                catch (FormatException formatException)
                {
                    Console.WriteLine(formatException.Message);
                }
                catch (OverflowException overflowException)
                {
                    Console.WriteLine(overflowException.Message);
                }
                catch (Exception)
                {
                    Console.WriteLine("Jakiś inny wyjątek");
                }
                Console.WriteLine("Podaj liczbe m: ");
                int m = int.Parse(Console.ReadLine());
            }

            int suma = 0;
            for (int i = n; i <= m; i++)
            {
                suma += (int)Math.Pow(i, 3);

            }
            Console.WriteLine("Suma wynosi " + suma);
        }
    }
}
///////////////////
        }
        }
   }
