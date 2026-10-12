import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        int claveSecreta = 7;
        //claveSecreta = 7: Establece el código correcto//

        int intento;
        //intento: Guarda el número introducido//

        System.out.println("¡Bienvenido al sistema de verificación!");

        do {
            //do:  Ejecuta el bloque al menos una vez//

            System.out.print("Introduce el código numérico de acceso (del 1 al 10): ");
            intento = s.nextInt();

            if (intento != claveSecreta) {
                //if: Comprueba si el código es incorrecto//

                System.out.println("Acceso denegado. Intenta de nuevo.");
            }
        } while (intento != claveSecreta);
        //while: Repite hasta introducir el código correcto//

        System.out.println("¡Acceso concedido! Código correcto.");
        s.close();
    }
}
//El programa solicita un código de acceso y continúa preguntándolo hasta que el
// usuario introduce el código correcto/