import java.util.Scanner;

public class Dados {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Quantidade de dados (Enter para 1): ");
        String entrada = sc.nextLine();

        int quantidade = 1;

        if (!entrada.isEmpty()) {
            quantidade = Integer.parseInt(entrada);
        }

        for (int i = 1; i <= quantidade; i++) {

            int valor = (int) (Math.random() * 6) + 1;

            System.out.println("\nDado " + i + ":");
            desenharDado(valor);
        }

        sc.close();
    }

    public static void desenharDado(int valor) {

        switch (valor) {

            case 1:
                System.out.println("+-------+");
                System.out.println("|       |");
                System.out.println("|   ●   |");
                System.out.println("|       |");
                System.out.println("+-------+");
                break;

            case 2:
                System.out.println("+-------+");
                System.out.println("| ●     |");
                System.out.println("|       |");
                System.out.println("|     ● |");
                System.out.println("+-------+");
                break;

            case 3:
                System.out.println("+-------+");
                System.out.println("| ●     |");
                System.out.println("|   ●   |");
                System.out.println("|     ● |");
                System.out.println("+-------+");
                break;

            case 4:
                System.out.println("+-------+");
                System.out.println("| ●   ● |");
                System.out.println("|       |");
                System.out.println("| ●   ● |");
                System.out.println("+-------+");
                break;

            case 5:
                System.out.println("+-------+");
                System.out.println("| ●   ● |");
                System.out.println("|   ●   |");
                System.out.println("| ●   ● |");
                System.out.println("+-------+");
                break;

            case 6:
                System.out.println("+-------+");
                System.out.println("| ●   ● |");
                System.out.println("| ●   ● |");
                System.out.println("| ●   ● |");
                System.out.println("+-------+");
                break;
        }
    }
}
