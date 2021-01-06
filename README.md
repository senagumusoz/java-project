# java ile taş_kağıt_makas

package tas_kagit_makas;

import java.util.Scanner;

public class taskagitmakas {

	public static void main(String[] args) {
		int kazanmaSayi_Bilgisayar=0;
		int kazanmaSayi_kullanici=0;
			System.out.println("Tas=0,Makas=1,Kağıt=2");
		int bitis=3;
		while(kazanmaSayi_Bilgisayar<bitis && kazanmaSayi_kullanici<bitis)
		{
		
			int bilgisayar_tahmin=(int)(Math.random()*3);
			
			System.out.println("tahmininiz : ");
			Scanner input=new Scanner(System.in);
			int kullanici_tahmin=input.nextInt();
			
			System.out.println(bilgisayar_tahmin+" bilgisayar-- kullanıcı "+kullanici_tahmin);
		
		if(bilgisayar_tahmin==0)
		{
			System.out.println("TAŞ");
		}
		else if(bilgisayar_tahmin==1)
		{
			System.out.println("makas");
		}
		else if(bilgisayar_tahmin==2)
		{
			System.out.println("kağıt");
		}
		
			if(kullanici_tahmin==bilgisayar_tahmin)
			{
				System.out.println("berabere");
			}
			else if((kullanici_tahmin==0 && bilgisayar_tahmin==1 )||(kullanici_tahmin==1 && bilgisayar_tahmin==2) ||(kullanici_tahmin==2 && bilgisayar_tahmin==0))
				{System.out.println("kullanıcı kazandı");
				kazanmaSayi_kullanici++;
				}
		
			else
				{System.out.println("bilgisayar kazandı");
				kazanmaSayi_Bilgisayar++;
				}
				}
				}
		
	}


