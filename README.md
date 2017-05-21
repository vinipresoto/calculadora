# calculadora
exemploprofessor

import java.util.Scanner;

public class DesafioCalculadora {

    static Scanner input = new Scanner(System.in);

    static int menu() {
        int opcao;
        System.out.println("Menu");
        System.out.println("1 - ** Adição **");
        System.out.println("2 - ** Subtração **");
        System.out.println("3 - ** Multiplicação **");
        System.out.println("4 - ** Divisão **");
        System.out.println("Opção: ");
        opcao = input.nextInt();
        return opcao;
    }

    static int add(int x, int y) {
        System.out.println("**Adição**");
        int resultado = x + y;
        return resultado;
    }

    static int entradaDados() {
        System.out.println("**Entrada**");
        int n = input.nextInt();
        return n;
    }

    static void imprimir(double n) {
        System.out.println("**Imprimir**");
        System.out.println("Resultado: " + n);
    }

    static double controle(int opcao, int x, int y) {
        System.out.println("Controle");
        double r = 0;
        switch (opcao) {
            case 1:
                r = add(x, y);
                break;

        }
        return r;
    }

    public static void main(String[] args) {
        int opcao = menu();
            int x = entradaDados();
            int y = entradaDados();
            double r = controle(opcao, x, y);
            imprimir(r);
    }
}
