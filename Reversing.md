import java.util.Scanner;
public class Reverse
{
    public static void main(String[] args)
    {
        int count=0;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number : ");
        int n = sc.nextInt();
        int p = n;
        int sum=0;
        //THIS WILL GIVE YOU TOTAL NUMBERS PRESENT IN THE GIVEN USER INPUT
        while(n!=0)
        {
            n=n/10;
            count++;
        }
        for(int i=1;i<=count;i++)
        {
           int r = p % 10;
            sum = (sum * 10) + r;//5
            p = p/10;
        }
        System.out.println(sum);
    }
}