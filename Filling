using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.IO;

namespace Cocktail__sort
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] arr = new int[100];
            int i=0;
            string a;
            StreamReader sw = new StreamReader(@"C:\Users\sadiq\Desktop\file.txt");
            while((a=sw.ReadLine())!=null)
            {
                arr[i] = int.Parse(a);
                i++;
            }
            Console.WriteLine("\t\t\tUnsorted Arrray  ");
            for (int c = 0; c < i; c++)
            {
                Console.WriteLine(arr[c]);
            }


            //cocktail_Sort
            int f; int start = 0; int end = i - 1;
            for(int y=0;y<i;y++)
            {   
                for(int z=start;z<end;z++)
                {
                    if(arr[z]>arr[z+1])
                    {
                         f = arr[z];
                        arr[z] = arr[z + 1];
                        arr[z + 1] = f;
                    }
                    

                }
                
                for(int x=end;x>start;x--)
                {
                    if (arr[x] < arr[x - 1])
                    {
                        f = arr[x];
                        arr[x] = arr[x - 1];
                        arr[x - 1] = f;
                    }
                    

                }
                start++;
                end--;
            }
            Console.WriteLine("\t\t\tSorted Array ");
            for (int c = 0; c < i; c++)
            {
                Console.WriteLine(arr[c]);
            }
            
            StreamWriter s = new StreamWriter("new_file.txt");
            int q=i;
            i = 0;
            s.WriteLine("After Sorting Numbers by cockTail Sort\n");
            while(q!=0)
            {
                

                s.WriteLine("{0}",arr[i]);
                i++;
                q--;

            }
            s.Close();
        }
    }
}
