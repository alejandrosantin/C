#include <stdio.h>
#include <conio.h>

int respu;
int rsum,rrest,rmult,num1,num2;
float rdiv;

int main (void){
	respu=6;
	while(respu !=0){
		printf("============================================ \n");
		printf("MENU PRINCIPAL \n");
		printf("============================================ \n");
		printf("1) SUMA \n");
		printf("2) RESTA \n");
		printf("3) MULTIPLICACION \n");
		printf("4) DIVISION \n");
		printf("0) SALIR \n");
		printf("============================================ \n");
		printf("Elige una opcion: ");
		scanf("%d",&respu);  //Lee la opción seleccionada
		_clrscr(); //Borra todo el menu luego de elegir la opción
		switch(respu){ //Creamos lo que se realizara en cada opción
			case 1:
					printf("Ingrese numero 1: \n");
					scanf("%d",&num1);
					printf("Ingrese numero 2: \n");
					scanf("%d",&num2);
					rsum=num1+num2;
					printf("El resultado es %d",rsum);
					break;
			case 2:
					printf("Ingrese numero 1: \n");
					scanf("%d",&num1);
					printf("Ingrese numero 2: \n");
					scanf("%d",&num2);
					rrest=num1-num2;
					printf("El resultado es %d",rrest);
					break;
			case 3:
					printf("Ingrese numero 1: \n");
					scanf("%d",&num1);
					printf("Ingrese numero 2: \n");
					scanf("%d",&num2);
					rmult=num1*num2;
					printf("El resultado es %d",rmult);
					break;
			case 4:
					printf("Ingrese numero 1: \n");
					scanf("%d",&num1);
					printf("Ingrese numero 2: \n");
					scanf("%d",&num2);
					rdiv=num1/num2;
					printf("El resultado es %.2f",rdiv);
					break;
			case 0:
					printf("Saliendo...");
					break;
			default:
					printf("Numero incorrecto...");
					break;
		}
	_getch (); //Esperamos un ingreso de caracter para poder leer la respuesta del caso
	_clrscr(); //Limpiamos la pantalla para volver a mostrar el menu
}
	return 0;
}
