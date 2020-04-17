# codigos-de-clase
import java.util.Scanner; //Utilizamos la libreria Scanner para poder leer datos
public class operadoresBasicos//Declaramos la clase principal con el nombre operadoresBasicos
{
	public static void main(String[] args) 
	{
		//Declaracion de variables a utilizar
		int cuenta; 
		int resul=0;

		Scanner lee = new Scanner (System.in);//Lo declaramos para poder leer datos ingresados por el usuario

		System.out.println("Ingresa numero de cuenta: ");//Pedimos al usuario su numero de cuenta
		cuenta = lee.nextInt();//Guardamos el numero de cuenta en la variable ya declarada
		//Utilizamos el ciclo while para poder realizar la sumatoria de los numeros de la cuenta
		while(cuenta > 0) 
		{
			//Mediante el residuo y la division haremos la suma de cada digito
			resul += cuenta % 10;
			cuenta = cuenta / 10;
        }
		System.out.println("El resultado es: "+resul);//Imprimimos la suma del numero de cuenta

	}
}
