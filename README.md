# actividad2_punto5_poo
package matriculaestudiante;
import java.util.Scanner;
public class Matriculaestudiante {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        double  numero,patrimonio,estrato;
        double pago=50000;
        String nombres;
        Scanner ingresotecl = new Scanner (System.in);
        
        System.out.println("Ingrese el numero de inscripcion:  ");
        numero = ingresotecl.nextDouble();
        
        System.out.println("Ingrese los nombres:  ");
        nombres = ingresotecl.next();
        
        System.out.println("Ingrese el patrimonio:  ");
        patrimonio = ingresotecl.nextDouble();
        
        System.out.println("Ingrese el estrato:  ");
        estrato = ingresotecl.nextDouble();
        
        if ((patrimonio>2000000) && (estrato>3)){
            pago= pago + (0.03*patrimonio);
        }
        System.out.println(" el estudiante con numero de inscripcion: " +numero +" y nombre: " +nombres +" debe pagar: "+ pago);
        
    }
    
}
