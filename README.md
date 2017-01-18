using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace December_Exam
{
    class Program
    {
        static void Main(string[] args)
        {

            int n = int.Parse(Console.ReadLine());

            int figurewidth = 4 * n + 1;

            Console.WriteLine(@"{0}/|\{0}", new string('.', n * 2 - 1));
            Console.WriteLine(@"{0}\|/{0}", new string('.', n * 2 - 1));
            Console.WriteLine(@"{0}***{0}", new string('.', n * 2 - 1));

            for (int currow = 1; currow <= n*2-1; currow++)
            {

                Console.WriteLine("{0}*{1}*{1}*{0}", new string('.', (figurewidth - 3 - (currow * 2)) / 2), new string('_', currow));
            }
            Console.WriteLine("{0}", new string('*', figurewidth));
           
                Console.Write("*");
                Console.Write(".");
                for (int cur = 0; cur<(4*n-1)/2; cur++)
                {

                    Console.Write("*");
                    Console.Write(".");

                }
               


            
            Console.WriteLine('*');
          
            Console.WriteLine("{0}", new string('*', figurewidth));
        }
    }
}
