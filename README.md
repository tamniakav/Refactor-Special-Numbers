# Refactor-Special-Numbers
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Refactor_Special_Numbers
{
    class Program
    {
        static void Main(string[] args)
        {

            int n = int.Parse(Console.ReadLine());

            for (int i = 1; i <= n; i++)
            {
                int sum = 0;
                int count = 0;
                bool isTheSpecialNum = false;

                if (i > 0)
                {

                    count = i;
                    sum += i % 10;
                    sum += i / 10;

                    isTheSpecialNum = (sum == 5) || (sum == 7) || (sum == 11);
                    Console.WriteLine($"{count} -> {isTheSpecialNum}");
                }
                sum = 0;

            }

        }
    }
}
