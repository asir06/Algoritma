

package Uygulamalar;
import java.util.Scanner;
public class Uygulamalar51 {

	 public static void main(String[] args){     
		 Scanner giris=new Scanner(System.in);
		 System.out.println("Bir Cümle Giriniz");
		 String harfler=giris.nextLine();
		 harfler=harfler.toLowerCase();
	     String harfler1="abcçdefgğhıijklmnoöpqrsştuvwxyzABCÇDEFGĞHIİJKLMNOÖPRSŞTUVWXYZ";
	     int[] harf = new int[harfler.length()];    
	     for(int i = 0; i < harfler.length(); i++)
	     {
		 int find = harfler.indexOf(harfler.charAt(i));
		 if (find < 0)  
	     continue;
		 harf[find]++;
	     }    
		 for (int i = 0; i<harf.length; i++)
		 {     
		 if (harf[i] < 1)
		 continue;
		 System.out.println(String.format("%s (%d) %s",
				 harfler.charAt(i),
				 harf[i],
		 new String(new char[harf[i]])));} }
	     }
  
  
