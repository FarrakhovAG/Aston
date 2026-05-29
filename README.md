# Aston
Решение задания на стажировку в Aston

Задача №1

Написать программу, которая принимает на вход два целых числа (a и b) и совершает с ними следующие действия:
- сравнивает эти два числа и возвращает результат сравнения путем вывода в консоль одного из вариантов: "a > b", "a < b" или "a = b";
- совершает с этими числами операции сложения, вычитания, деления и умножения и результат выводит в консоль

public class World {
   public static void main(String[] args) {
      Scanner console = new Scanner(System.in);
       System.out.println("Введите число а: ");
       int a = console.nextInt();

       System.out.println("Введите число b: ");
       int b = console.nextInt();

       if (a > b){
           System.out.println("a > b");
       } else if (a < b) {
           System.out.println("a < b");
       } else {
           System.out.println("a = b");
       }
       System.out.println("Сложение: " + (a + b));
       System.out.println("Вычитание: " + (a -b));
       System.out.println("Умножение:" + (a * b));

       if (b != 0){
           System.out.println("Деление: " + (a / (double)b));
       }else{
           System.out.println("Деление: невозможно ( деление на 0");
       }
   }
}

Задача №2

Написать программу, которая принимает на вход две строки (a и b) и сравнивает их. В результате сравнения в консоль должно быть выведено одно из сообщений: "Строки неидентичны" или "Строки идентичны"

public class Aston {

    public static void main(String[] args) {

        Scanner sr = new Scanner(System.in);
        System.out.println("Введите строку a: ");
        String a = sr.nextLine();

        System.out.println("Введите строку b: ");
        String b = sr.nextLine();

        if (a.equals(b)){
            System.out.println("Строки идентичны");
        }else{
            System.out.println("Строки неидентичны");
        }
    }
}

Задча №3

Задан массив целых чисел: [1, 2, 3, 4, 5, 6, 7, 8, 9,10]  необходимо написать программу, которая выведет в консоль все чётные числа.

public class Aston {
    public static void main(String[] args) {
       int[] array = {1,2,3,4,5,6,7,8,9,10};
            for (int i = 0; i < array.length; i++) {
                if (array[i] % 2 == 0){
                    System.out.println(array[i]);
                }
            }
        }
        }
