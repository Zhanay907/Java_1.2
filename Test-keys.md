																									
ID	Название (Title):	Описание( Summary):	Приоритет (Priority)	Шаги (Steps to reproduce):	Ожидаемый результат (Expected result):	Комментарии к тесту																			
1	Запуск приложения <Credit Card Number Validator> разными данными  	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Открыть вебсайт по ссылке: https://www.freeformatter.com/credit-card-number-generator-validator.html.  Создать гугл-таблицу для записи тест кейсов.	высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
  System.out.println (""Hello programming"");

  }
}"	"1. В результате работы вывод приложения будет выглядеть следующим образом:

""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=54990:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Hello programming

Process finished with exit code 0
"																				
				"2. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""5351719427810741"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"2. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55020:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"																				
2	Запуск приложения <Credit Card Number Validator> разными данными 	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Создать гугл-таблицу для записи тест кейсов.	Высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""4485930843970181"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"1. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55038:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"																				
3	Запуск приложения <Credit Card Number Validator> разными данными 	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Создать гугл-таблицу для записи тест кейсов.	Высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""6011749487144863"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"1. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55038:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"																				
4	Запуск приложения <Credit Card Number Validator> разными данными 	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Создать гугл-таблицу для записи тест кейсов.	Высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""30106313883067"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"1. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55038:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"	"""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=54556:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is FAIL

Process finished with exit code 0
"																			
5	Запуск приложения <Credit Card Number Validator> разными данными 	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Создать гугл-таблицу для записи тест кейсов.	Высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""4913628963948951"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"1. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55038:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"																				
6	Запуск приложения <Credit Card Number Validator> разными данными 	По ссылке https://github.com/netology-code/javaqa-homeworks/tree/master/intro открыть приложение "Credit Card Number Validator". Открыть редактор кода"Intellij IDEA". Создать гугл-таблицу для записи тест кейсов.	Высокий	"1. Ввести в редактор кода""Intellij IDEA"" и осуществить запуск:
public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = ""5392304522358804"";
    System.out.println(String.format(""Result is %s"", isValidCardNumber(number) ? ""OK"" : ""FAIL""));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + """");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}"	"1. ""C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin\java.exe"" ""-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\lib\idea_rt.jar=55038:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2020.3.2\bin"" -Dfile.encoding=UTF-8 -classpath C:\Users\user\Desktop\projects\untitled1\out\production\untitled1 Main
Result is OK

Process finished with exit code 0"																				
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									
																									