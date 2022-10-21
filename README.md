# 21.10.22
## 1. Создайте функцию, вызываемую shortcutдля удаления строчных гласных (a, e, i, o, u) в заданной строке.
[Task link](https://www.codewars.com/kata/5547929140907378f9000039/train/java)
___
### Мое рещение 
```java

public class Kata {
  public static String shortcut(String input) {
     String[] vowels ={"a", "e", "i", "o", "u"};
     for (String sorter:vowels){
               if (input.contains(sorter)){
                    input = input.replace(sorter,"");
               }

       }
    return input;   
  }
}

```

### Понравившееся решение
```java

public class Kata {
  public static String shortcut(String input) {
        String word = input.replaceAll("[aoeiu]", "");
        return word;
    }
}

```
## 2. This Kata is intended as a small challenge for my students
All Star Code Challenge #18
Create a function that accepts 2 string arguments and returns an integer of the count of occurrences the 2nd argument is found in the first one.
If no occurrences can be found, a count of 0 should be returned.
[Task link](https://www.codewars.com/kata/5865918c6b569962950002a1/train/java)
### Мое рещение 
```java

public class CodeWars {
  public static int strCount(String str, char letter) {
    int counter = 0;
    for(char character : str.toCharArray()) {
      if(letter == character) {
        counter++;
      }
    }
    return counter;
  }
}

```

### Понравившееся решение
```java

public class CodeWars {
  public static int strCount(String str, char letter) {
    return (int)str.chars().filter(x -> x == letter).count();
  }
}

```
