#bài 1 (trên lớp)
import java.util.Scanner;
public class Main
{
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Nhap so nguyen= ");
        int n = scanner.nextInt();
        int check = find_square_number(n);
     
        if( check == 1 ) System.out.println(n + " la so chinh phuong" ) ;
        else System.out.println(n+ " khong phai la so chinh phuong" ) ;
    }
    private static int find_square_number(int n){
        int flag = 0;
        int i = 0;
        while(i <= n){
            if( Math.pow( i, 2) == n ) {   
                flag = 1;
                break;
            }
            i++;
        }

        return flag;
    }
}

# bài 2 (Trên lớp)

import java.util.Scanner;
public class XepHang {
    public static void main(String[] args)
    {
       Scanner input = new Scanner (System.in);
       double score,gioi,kha,trungbinh,kem;
       System.out.print("nhập điểm: ");
       score = input.nextDouble ();
       {
           if (score >=8)
           System.out.print("gioi: ");
           else if ((score >=7) && (score <=8))
           System.out.print("kha: ");
           else if ((score >=5) && (score <=7))
           System.out.print("trungbinh: ");
           else 
           System.out.print("kem: ");
       }
}
}
#bài 3 (Trên lớp)
mport java.util.Scanner;

public class BaiTapJavaCoBan2 {
   public static void main(String[] args)
   {
      int n;
      System.out.println("Nhap vao mot so nguyen:");
      Scanner sc = new Scanner(System.in);

      n = sc.nextInt();

      switch (n)
      {
         case 0: System.out.println("Không"); break;
         case 1: System.out.println("Một"); break;
         case 2: System.out.println("Hai"); break;
         case 3: System.out.println("Ba"); break;
         case 4: System.out.println("Bốn"); break;
         case 5: System.out.println("Năm"); break;
         case 6: System.out.println("Sáu"); break;
         case 7: System.out.println("Bảy"); break;
         case 8: System.out.println("Tám"); break;
         case 9: System.out.println("Chín"); break;
         default:
            System.out.println("Chỉ có 0 - 9 thôi :D");
            break;
      }
   }
}
# bài 4 (Trên lớp)
public static void main(String[] args) {
    int n, i, c;
    Scanner scanner = new Scanner(System.in);
         
    do {
        System.out.println("Nhập vào số phần tử của mảng: ");
        n = scanner.nextInt();
    } while (n <= 0);
         
    int A[] = new int[n];
         
    System.out.println("Nhập các phần tử cho mảng: ");
    for (i = 0; i < n; i++) {
        System.out.print("Nhập phần tử thứ " + i + ": ");
        A[i] = scanner.nextInt();
    }
    System.out.println("Nhập số nguyên k: ");
    int k = scanner.nextInt();
    for (c = i = 0; i < n; i++) {
        if (A[i] != k) {
            A[c] = A[i];
            c++;
        }
    }
         
    n = c; 
    System.out.println("Mảng còn lại sau khi xóa phần tử " + k + " là: ");
    for (i = 0; i < n; i++) {
        System.out.print(A[i] + "\t");
    }
}
