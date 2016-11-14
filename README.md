# mas_dinero
en 5 monedas, dice quien tiene mas dinero
//*trata de que , pedir 5 monedas, las tres primeras son de pedro y las siguientes de juan, con esto saber quien tene mas dinero

import java.util.Scanner;
import javax.swing.JOptionPane;


public class NewClass 
{
    public static void main(String[] args) 
    {
        Scanner sc =  new Scanner(System.in);
        int pedro=0, juan=0, monedas=0;
        
        for (int i = 1; i < 6; i++) 
        {
            monedas = sc.nextInt();
            if(i<4)
                juan += monedas;
            else
                pedro += monedas;
        }
        
        if (juan>pedro)
            System.out.println("Juan");
        else
            System.out.println("Pedro");
        
    }
    
}
