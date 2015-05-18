package es.ramonmerino.solo5;

import java.util.Scanner;

public class Main {
	
	public static Scanner scan;

	public static void main(String[] args) {
		
		int[] v = new int[3];
		int media;
		
		v[0] = hola();
		v[1] = hola();
		v[2] = hola();
		
		media = (v[0] + v[1] + v[2])/3;
		System.out.println("Su media es: "+ media);
		System.out.println("Inserta nombre");
		
		String[] n = new String[2];
		n[0] = nombre();
		n[1] = Integer.toString(media);
		
		System.out.println("La media de "+ n[0]+ " es "+ n[1]);
		
		

	}
	
	public static int hola(){
		scan = new Scanner(System.in);
		int in = scan.nextInt();
		
		return in;
				
	}
	
	public static String nombre(){
		
		String str = scan.next();
		
		return str;
		
		
	}
	

}
