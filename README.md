### Hesap Makinesi İle Dört İşlem:

```java
import java.util.Scanner;

public class calculator {
    public static void main(String[] args) {
        int n1, n2;
        int select;

        Scanner input = new Scanner(System.in);
        System.out.print("İlk Sayıyı Giriniz :");
        n1 = input.nextInt();
        System.out.print("İkinci Sayıyı Giriniz :");
        n2 = input.nextInt();

        System.out.println("1-Toplam\n2-Çıkarma\n3-Çarpma\n4-Bölme");
        System.out.println("Seçiminiz :");
        select = input.nextInt();

        switch (select) {
            case 1:
                System.out.print("Toplam :" + (n1 + n2));
                break;

            case 2:
                System.out.print("Çıkarma Sonucu :" + (n1 - n2));
                break;

            case 3:
                System.out.print("Çarpım Sonucu :" + (n1 * n2));
                break;

            case 4:
                switch (n2) {
                    case 0:
                        System.out.println("Bölen sıfır olamaz!");
                        break;
                    default:
                        System.out.print("Bölme Sonucu :" + (n1 / n2) + "  Kalan :" + (n1 % n2));
                        break;
                }
            default:

        }
    }

}

```

