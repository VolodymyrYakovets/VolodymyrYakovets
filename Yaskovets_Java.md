```Java
package com.company; // Составить алгоритм: если введенное число больше 7, то вывести “Привет”
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner num = new Scanner(System.in);
        int digit;
        System.out.print("Введите число: ");
        digit = num.nextInt();

        if (digit > 7)
            System.out.print("Привет");

    }
}
```
```Java
package com.company; // Составить алгоритм: если введенное имя совпадает с Вячеслав, то вывести “Привет, Вячеслав”, если нет, то вывести "Нет такого имени"
import java.util.Scanner;

import static java.lang.System.*;

public class Main {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(in);
        System.out.println("Введите свое имя");
        String a = "Вячеслав";
        String b = scanner.nextLine();

        if (a.equals(b)) {
            out.println("Привет, Вячеслав");
        }else{
            out.println("Нет такого имени");
        }
    }
}
```
```Java
package com.company; // Составить алгоритм: на входе есть числовой массив, необходимо вывести элементы массива кратные 3
public class Main{

    public static void main(String[] args) {
        int[] myList = {1, 2, 3, 4, 5, 6, 7, 8, 9};
        for (int i = 0; i < myList.length; i++) {
            if (myList[i] % 3 == 0) {
                System.out.println(myList[i]);
            }
        }
    }
}
```
- [x] Коды были написаны и запускались на IntelliJ IDEA Community Edition 2021.2.2 

## Дана скобочная последовательность: [((())()(())]]
> - Можно ли считать эту последовательность правильной?
>> Я считаю эту последовательность неправильной.
>>> - Если ответ на предыдущий вопрос “нет” - то что необходимо в ней изменить, чтоб она стала правильной? 
>>>> [1  (2  (3  (4)4!  )3!  (5)5!  (6  (7 )7!  )6!  ]2!  ]1!
>>>>> Для наглядности скобки были пронумерованы. Беру во внимание, что общее количество скобок равняется 14.
И з чего следует вывод, что каждой открывающей скобке соответствует скобка закрывающая.
Номерую  скобки, чтобы выделить открывающую и закрывающая скобку.
Последовательность могла бы быть правильной если бы форма скобки номер 2 имела одинаковый вид.
