# Alternate-sign
import java.util.Scanner;

public class alternatesign {
    public alternatesign() {
    }

    static int go(int n, int i) {
        if (i == n + 1) {
            return 0;
        } else {
            return i % 2 == 0 ? go(n, i + 1) - i : go(n, i + 1) + i;
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.println(go(n, 1));
    }
}
