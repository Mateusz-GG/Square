# Square

To build a Square open console and type the ammount of stars in all sides.


{

    class Program
    {
        public static void ZbudujPelnaLinie(int dlugosc)
        {
            for (int i = 0; i < dlugosc; i++)
            {
                Console.Write("");
            }
            Console.Write("\n");
        }
        public static void ZbudujLinieZdziura(int dlugosc)
        {
            Console.Write("");
            for (int i = 2; i < dlugosc; i++)
            {
                Console.Write(" ");
            }
            Console.Write("*\n");
        }
        static void Main(string[] args)
        {

            int A = 0;
            Console.WriteLine("Podaj długość boku gwiazdkowego kwadratu");
            A = Convert.ToInt32(Console.ReadLine());

            ZbudujPelnaLinie(A);
            for (int i = 2; i < A; i++)
            {
                ZbudujLinieZdziura(A);
            }
            ZbudujPelnaLinie(A);

        }
    }
}
