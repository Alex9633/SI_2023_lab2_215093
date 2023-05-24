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
- Тест случај 1: сите се null
- Тест случај 2: user != null, password == null, email == null
- Тест случај 3: user == null, password != null, email == null
- Тест случај 4: user == null, password == null, email != null
- Тест случај 5: user != null, password != null, email == null
- Тест случај 6: user != null, password == null, email != null
- Тест случај 7: user == null, password != null, email != null
- Тест случај 8: сите не се null

Во сите случаеви, освен тест случај 8, ќе биде проверено дали ќе биде фрлен исклучок т.е. ако фали барем една од информациите.
Во тест случај 8 се проверува дали функцијата враќа true кога се присутни сите три задолжителни полиња.
