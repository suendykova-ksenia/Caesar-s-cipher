# **Шифр Цезаря. Автор Ксения Суендыкова**
____
### *Первое изменение*

## **Краткое описание программы на шаге 1:**

Написала программу шифрования букв латинского алфавита A-Z (a-z) и цифр 0-9. Введенные пользователем иные символы (< / - , и тд) остаются неизменными после шифрования (в том числе и пробелы)     
Начала писать функции программы, предварительно их будет 4:   
1. Шифрование  текста    
2. Расшифровка текста    
3. Показать "Таблицу шифра"    
4. Выйти из программы    
Кроме этого нужно:
- дополнить программу как минимум расшифровкой текста
- ввести ограничения на ввод данных допустимого формата, чтобы программа не ломалась
- (в перспективе) расширить программу вводом текста на русском языке    
p.s. Сейчас при вводе текста на русском языке программа выдает кракозябры :D 
    
## **Результат работы программы(скриншоты):**

### *С положительным шагом кодировки:*    
![Alt-текст](https://skr.sh/i/011120/rKoM95YP.jpg?download=1&name=Скриншот%2001-11-2020%2013:51:43.jpg)

### *С отрицательным шагом кодировки:*    
![Alt-текст](https://skr.sh/i/011120/0mnc0mtX.jpg?download=1&name=Скриншот%2001-11-2020%2014:18:16.jpg)

### *Шаг кодировки равен нулю:*    
![Alt-текст](https://skr.sh/i/011120/UqZMfrsN.jpg?download=1&name=Скриншот%2001-11-2020%2014:23:34.jpg)

## **Где и как открыть проект?**

Программа написана на языке программирования С++.    
Проект можно открыть в среде программирования Visual Studio 2019.    
Открытие проекта: репозиторий "Caesar-s-cipher";commit "Пишу шифр Цезаря. Шаг 1";файл "Шаг 1. Шифр Цезаря.cpp" (скопировать код и скомпилировать в Visual Studio 2019)    
Пользуясь локальным отладчиком Windows можно запустить программу    
Далее в консоли появится сообщение, разъясняющее, что это за программа и каким должен быть следующий шаг.    

## **Код программы после первого изменения**   
Можно посмотреть, открыв файл "Шифр Цезаря.cpp" в коммите "Пишу шифр Цезаря. Шаг 1"    
____
### *Второе изменение*

## **Краткое описание программы на шаге 2:**    

Теперь можно шифровать текст на русском языке (А-Я, а-я), только для этого при компиляции необходимо:
нажать п.к.м на окно консоли; выбрать "Свойства"; "Шрифт"; Изменить шрифт на "Lucida Console"; закрыть окно "Свойства"
p.s. При этом по-прежнему шифруются буквы A-Z, a-z и цифры 0-9

## **Результат работы программы(скриншот):**

### *С положительным шагом кодировки:*    
![Alt-текст](https://sun9-31.userapi.com/impf/3vBV9ftjNXv3zqaW2q_u9bTU2UoAtSA0KiPV0Q/er8jm3JqIgk.jpg?size=590x335&quality=96&proxy=1&sign=b59b75ca4bbf51b14b44a4e65a72ae44)    
Так же все работает и для отрицательного шага кодировки, и для нулевого    

## **Код программы после второго изменения**   
Можно посмотреть, открыв файл "Шифр Цезаря.cpp" в коммите "Пишу шифр Цезаря. Шаг 2"    
____
### *Третье изменение*

## **Краткое описание программы на шаге 3:**    

-Доработала диалоговый режим с пользователем
-Проработала 4 основные функции:
    1. Шифрование текста
    2. Расшифровка текста
    3. Что такое "Шифр Цезаря"? (справка)
    4. Выйти из программы
-Вынесла отдельно функцию шифрования/расшифровки текста(не в main() теперь происходит преобразование текста, а в basprog(int hk))
(все это сопровождается подобными комментариями созданных функций и блоков действий)

## **Результат работы программы(скриншот):**

### *С положительным шагом кодировки:*    
![Alt-текст](https://skr.sh/i/021120/0HRWpe3g.jpg?download=1&name=Скриншот%2002-11-2020%2021:25:58.jpg)    
![Alt-текст](https://skr.sh/i/021120/WEllVfu8.jpg?download=1&name=Скриншот%2002-11-2020%2021:26:25.jpg)    
Так же все работает и для отрицательного шага кодировки, и для нулевого    

## **Код программы после третьего изменения**   
Можно посмотреть, открыв файл "Шифр Цезаря.cpp" в коммите "Пишу шифр Цезаря. Шаг 3"
____
### *Четвертое изменение*

## **Краткое описание программы на шаге 4:**    

Добавила обработку ошибок ввода. Теперь программа не ломается при вводе данных недопустимого формата, а выдает сообщение об ошибке и предлагает осуществить ввод заново.
Проверка сделана для ввода номера функции и шага для кодировки. На ввод текста, по идее, ограничений нет. Посмотим, что будет при серьезном тестировании пограммы. Может какие-нибудь спец.символы сломают пограмму.
На перспективу: можно выявить символы, которые могут привеси к сбоям, и исключить их в качества ввода 

## **Результат работы программы(скриншоты):**

### *Проверка на ввод номера функции:*    
![Alt-текст](https://skr.sh/i/021120/yyTzcEZg.jpg?download=1&name=Скриншот%2002-11-2020%2022:32:43.jpg)    
![Alt-текст](https://skr.sh/i/021120/RFmJSOrG.jpg?download=1&name=Скриншот%2002-11-2020%2022:33:02.jpg)    

### *Проверка на ввод шага для кодировки:*    
![Alt-текст](https://skr.sh/i/021120/cLdJVHn7.jpg?download=1&name=Скриншот%2002-11-2020%2023:36:34.jpg)    
![Alt-текст](https://skr.sh/i/021120/NK7d0DKp.jpg?download=1&name=Скриншот%2002-11-2020%2023:40:13.jpg)   

## **Код программы после четвертого изменения**    
Можно посмотреть, открыв файл "Шифр Цезаря.cpp" в коммите "Пишу шифр Цезаря. Шаг 4"
