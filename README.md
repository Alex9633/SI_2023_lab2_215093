# Втора лабораториска вежба по Софтверско инженерство

# Александар Миланов 215093


## Control Flow Graph
(бројките ми се означени во кодот прикачен во репозиториумот)
![cfd](https://github.com/Alex9633/SI_2023_lab2_215093/assets/120327803/2676bc94-d704-44ae-b4fe-cd43797e3cc4)



## Цикломатска комплексност
Цикломатската комплексност на кодот е [број на региони] = 11.



## Тест случаи според критериумот Every Branch
- Тест случај за задолжителни информации што недостасуваат - да бидат доделени user, password и email
- За валидација на е-пошта каде што е-поштата не содржи „@“ или „.“
- За валидација на е-пошта каде што е-поштата содржи „@“ и „.“
- За валидација на лозинка каде лозинката го содржи корисничкото име
- За валидација на лозинка каде што должината на лозинката е помала од 8
- За валидација на лозинка каде лозинката не содржи никакви специјални знаци
- За валидација на лозинка каде лозинката содржи специјални знаци, но е-поштата веќе ја користи друг корисник



## Тест случаи според критериумот Multiple Condition за (user==null || user.getPassword()==null || user.getEmail()==null)
- Тест случај 1: user == null, password X null, email X null
- Тест случај 2: user != null, password == null, email X null
- Тест случај 3: user != null, password != null, email == null
- Тест случај 4: user != null, password != null, email != null

Бидејќи имаме логичко or секаде, ако наидеме на true statement нема врска другите што се, програмата нема да провери. (X -> или != или ==)
Кај првите три ќе фрли exception, кај четвртиот ќе продолжи понатаму.
