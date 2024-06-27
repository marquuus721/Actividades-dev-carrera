/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package traductor_binario;

import java.util.Scanner;

/**
 *
 * @author Marcos
 */
public class Traductor_Binario {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
    
    Scanner teclado =new Scanner (System.in);    
    
    //Defino variable de numero a ingresar
    String num;
        
        
    //le pedimos que ingrese el numero de 16 digitos
    System.out.println("*TRADUCTOR Binario*");
    
    //condicional while para asegurarme de que el numero que ingrese sea binario
    boolean esono= false;
    do {
        //input
        System.out.println("Ingrese un numero binario de 16 digitos");
        num = teclado.nextLine();
        
        //traduzco el dato a entero
        int numero = Integer.parseInt(num);

        //verifico que num sea binario..
        if (numero != 0 && numero != 1){
            esono=true;
        }else{
            esono=false;
        }
        
    } while (esono=false);
    
    //Convierto el numero Binario a Decimal
    double sumDECIM =0; //e definido la variable que mostrara el numero decimal del binario
        //defino vector 
        int [] vectorbin = new int [16];

        //coloco num (el dato en tipo String) en el vector
        for (int i=0; i< num.length(); i++){
            //separo el digito de la posicion i como un caracter
            char caracter= num.charAt(i);
            //el caracter lo convierto a entero
            int number = Character.getNumericValue(caracter);
            
                //Hago la conversion de binario a decimal
                    //Formula:
                        //potencia de 2
                        double exponente= 16-(i+1);

                        double pot= Math.pow( 2 , exponente ); 
                        //..en el parentesis de arriba se coloca (base ,exponente)
                    //formulaaa..
                    //no es necesario convertir int number a double:

                    double formula = number*pot; //Esta es la FORMULA!!

                    //sumo cada termino convertido operado a la variable suma "sumaDECIM" que sera al final el numero binario convertido a decimal          
                    sumDECIM += formula;
        }
        
    //Resultado
    System.out.println("El número binario: "+ num + " es equivalente a:");
    System.out.println("");
    System.out.println("\n . "+ sumDECIM +" ,en números decimales");
    
        
        

    }
    
}
