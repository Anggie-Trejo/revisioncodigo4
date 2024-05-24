# revisioncodigo4
revision de codigo4 
//Angelica Fuentes Trejo 
//3:Repasar estructura case 

package com.generation;
//Importar scanner

import java.util.Scanner;

public class pruebareps {
	 {
//Agregar System.in
	    Scanner s = new Scanner(System.in);
	    
	    System.out.print("Turno del jugador 1 (introduzca piedra, papel o tijeras): ");
	    String j1 = s.nextLine();
	    
	    System.out.print("Turno del jugador 1 (introduzca piedra, papel o tijeras): ");
	    Scanner s2 = new Scanner(System.in);
	    String j2 = s.nextLine();
	    //Quitar doble paréntesis, poner breaks en switch
	    if (j1 == j2) {
	      System.out.println("Empate");
	    } else {
	      int g = 2;
	      switch(j1) {
	        case "piedra":
	          if (j2 == "tijeras") {
	            g = 1;
	            break;
	          }

	        case "papel":
	          if (j2 == "piedra") {
	            g = 1;
	          break;
	          }
	        case "tijera":
	          if (j2.equals("papel")) {
	            g = 1;
	         
	          break;
	          }
	        default:
	      }
	      System.out.println("Gana el jugador " + g);
	    }
	  
	  
	}

}
