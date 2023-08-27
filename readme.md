Баг-репорт 1

Название 
# Отсутствует переменная int initialBalance и int rate

# Описание:
В классе SavingAccount.java не заведены переменные int initialBalance и int rate

# Локация деффекта
https://github.com/Vemant/QAMID-66_Java_TeamProject_26.08-04.09/blob/main/src/main/java/ru/netology/javaqadiplom/SavingAccount.java

# Шаги воспроизведения
1. Открыть в проекте класс SavingAccount
2. Прочитать описание сберегательного счета, в котором указано, что счет имеет минимальный и максимальный баланс (такие переменные заведены: int minBalance и int maxBalance), а также процент годовых и остаток, на который начиссляется процент (int rate и int initialBalance соответственно)
3. Далее видим, что переменные int rate и int initialBalance отсутствуют и первоначально упомянаются только в первом методе

   
*Ожидаемый результат: Переменные заведены как protected int initialBalance и protected int rate*

*Фактический результат: Переменные не заведены, и первоначально упомянаются непосредственно в самом методе (в первом)*

# Скриншот
![Баг 1](https://github.com/SofiaKoVRN/AI_12/assets/136505508/ce0f473b-4074-4aea-a7b4-da25ba2f22bf)



# Окружение
Операционная система: Windows 10 Pro
IDEA: IntelliJ IDEA 2023.2 (Community Edition)
Java: OpenJDK 11



Баг-репорт 2

# Некорректно указана часть метода this.balance = initialBalance

# Описание:
В строке 28 написано: this.balance = initialBalance; а должно быть this.initialBalance = initialBalance;

# Локация деффекта
https://github.com/Vemant/QAMID-66_Java_TeamProject_26.08-04.09/blob/main/src/main/java/ru/netology/javaqadiplom/SavingAccount.java

# Шаги воспроизведения
1. Открыть в проекте класс SavingAccount
2. Прочитать описание первого метода и посмотреть все ли в нем указано
3. Далее видим, что в строке 28 написано: this.balance = initialBalance; а должно быть this.initialBalance = initialBalance;

   
*Ожидаемый результат: в строке 28 написано: this.initialBalance = initialBalance;*

*Фактический результат: в строке 28 написано: this.balance = initialBalance;*

# Скриншот
![Баг 2](https://github.com/SofiaKoVRN/AI_12/assets/136505508/7b950c42-deb9-4f46-b8ea-fd3b75601edf)


# Окружение
Операционная система: Windows 10 Pro
IDEA: IntelliJ IDEA 2023.2 (Community Edition)
Java: OpenJDK 11
