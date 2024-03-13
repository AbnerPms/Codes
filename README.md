



import java.util.Scanner;
public class AprenderJava {

    public static void main(String[] args) {

      Scanner sc = new Scanner (System.in);

      System.out.println("Insir sua renda mensal para analise de imposto:");

      double salario = sc.nextDouble();
      double imposto;

      if (salario >= 0 & salario <= 2000){
          imposto = 0.0;
          System.out.println("Isento de imposto de renda");

      }else{
          if (salario >= 2000.01 & salario <= 3000){
              imposto = ((salario - 2000) * 8) / 100;
              System.out.println("Imposto a pagar: " + imposto);

          }else{
              if (salario >= 3000.01 & salario <= 4500){
                  imposto = ((salario - 2999.99) * 18) / 100 + 79.99;
                  System.out.println("Imposto a pagar: " + imposto);

              }else{
                  if(salario > 4500){
                      imposto = ((salario - 4499.98) * 28) / 100 + 79.99 + 269.99;
                      System.out.println("Imposto a pagar: " + imposto);

                  }
           
                sc.close;
              }
          }

      }
    }
}
