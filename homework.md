Задача 64

static void Natural_Num(int n)
{
    if (n > 0)
    {

        Console.WriteLine(n);
        Natural_Num(n - 1);
    }
}

Natural_Num(5);
Natural_Num(8);


Задача 66
int Amount(int m, int n)
{


    if (n == m)
    {
        return m;
    }
    if (n == m + 1)
    {
        return n + m + 1;
    }
    return m + n + Amount(m + 1, n - 1);

}

Console.WriteLine(Amount(1, 15));
Console.WriteLine(Amount(4, 8));

Задача 68

int Akkerman(int m, int n)
{
    if (m == 0)
    {
        return n + 1;
    }
    else if (m > 0 && n == 0)
    {
        return Akkerman(m - 1, 1);
    }
    else
    {
        return Akkerman(m - 1, Akkerman(m, n - 1));
    }
}


Console.WriteLine(Akkerman(2, 3));
Console.WriteLine(Akkerman(3, 2));
