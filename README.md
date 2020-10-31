# Actividad6CJ
import java.util.Scanner;
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.ArrayList;

public class Act6Java {

    public static Scanner sc= new Scanner(System.in);
    public static void main(String[] args)throws IOException{
        BufferedReader lector = new BufferedReader(new InputStreamReader(System.in));
        ArrayList<Integer> calificaciones= new ArrayList<Integer>();
        String nombre;
        int ave=0;

        System.out.println("Ingrese el nombre del estudiante: ");
        nombre=lector.readLine();
        System.out.println("Ingrese la calificacion 1");
        calificaciones.add(sc.nextInt());
        System.out.println("Ingrese la calificacion 2");
        calificaciones.add(sc.nextInt());
        System.out.println("Ingrese la calificacion 3");
        calificaciones.add(sc.nextInt());
        System.out.println("Ingrese la calificacion 4");
        calificaciones.add(sc.nextInt());
        System.out.println("Ingrese la calificacion 5");
        calificaciones.add(sc.nextInt());

            for(int i : calificaciones){
                ave += i;
            }

            System.out.println("Nombre: " + nombre);
            System.out.println("Promedio: "+(ave/5));
                if((ave/5)<=50){
                    System.out.println("Calificacion: F");
                }
                else if((ave/5)>=51&&(ave/5)<=60){
                    System.out.println("Calificacion: E");
                }
                else if((ave/5)>=61&&(ave/5)<=70){
                    System.out.println("Calificacion: D");
                }else if((ave/5)>=71&&(ave/5)<=80){
                    System.out.println("Calificacion: C");
                }else if((ave/5)>=81&&(ave/5)<=90){
                    System.out.println("Calificacion: B");
                }else if((ave/5)>=91&&(ave/5)<=100){
                    System.out.println("Calificacion: A");
                }


        }
}
