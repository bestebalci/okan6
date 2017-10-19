package okan6;

import java.util.Scanner;

public class okan61 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		//verilei yarat
		
		int input1, input2, sistem1, sistem2;
		
		
		
		// rastgele 2 sayı 
		
		sistem1 = (int) (Math.random() * 10);
		sistem2 = (int) (Math.random() * 10);
		System.out.println("sayilar" + sistem1 + "=" + sistem2 );
		
		//  kullanıcıdan 2 sayı girmesini iste
		System.out.println("Lütfen iki int 0-9 sayısı girin");
		Scanner input = new Scanner (System.in);
		input1= input.nextInt();
		input2= input.nextInt();
		
		// karşılaştırma yap ve gerekli mesajı göster
		if (input1== sistem1 && input2 == sistem2)

			System.out.println("10000 kazandınız");
		else if (input1 == sistem1 && input2 == sistem1)
			System.out.println("3000 kazandınız");
		else if ( input1== sistem1 || input1 == sistem2 || input2 == sistem1 || input2 == sistem2)
			System.out.println("1000 kazandınız");
	}

}
