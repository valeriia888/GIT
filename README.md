# GIT BASH
Hello user! Here you can see what commands I can use
1) Посмотреть где я: pwd
/g/home_work
Valery@DESKTOP-EEF72K9 MINGW64 /g/home_work

2) Создать папку: mkdir qa
Проверить содержимое: ls -la
total 4
drwxr-xr-x 1 Valery 197609 0 May 20 19:54 ./
drwxr-xr-x 1 Valery 197609 0 May 20 19:51 ../
drwxr-xr-x 1 Valery 197609 0 May 20 19:54 qa/

3) Зайти в папку : cd qa
Valery@DESKTOP-EEF72K9 MINGW64 /g/home_work/qa

4) Создать 3 папки:  mkdir test_3 test_4 test_5
Проверить содержимое: ls -la
total 0
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 ./
drwxr-xr-x 1 Valery 197609 0 May 20 19:54 ../
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 test_3/
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 test_4/
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 test_5/

5) Зайти в любую папку:  /g/home_work/qa/cd test_3

Valery@DESKTOP-EEF72K9 MINGW64 /g/home_work/qa/test_3

6) Создать 5 файлов (3 txt, 2 json) :  touch qq.txt 2qq.txt 3qq.txt fff.json ff.json
Проверить содержимое: ls -la
total 0
drwxr-xr-x 1 Valery 197609 0 May 20 20:14 ./
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 ../
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 2qq.txt
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 3qq.txt
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 ff.json
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 fff.json
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 qq.txt

7) Создать 3 папки: mkdir p_1 p_2 p_3

8. Вывести список содержимого папки: ls -la
total 4
drwxr-xr-x 1 Valery 197609 0 May 20 20:17 ./
drwxr-xr-x 1 Valery 197609 0 May 20 19:57 ../
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 2qq.txt
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 3qq.txt
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 ff.json
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 fff.json
drwxr-xr-x 1 Valery 197609 0 May 20 20:17 p_1/
drwxr-xr-x 1 Valery 197609 0 May 20 20:17 p_2/
drwxr-xr-x 1 Valery 197609 0 May 20 20:17 p_3/
-rw-r--r-- 1 Valery 197609 0 May 20 20:14 qq.txt

9) + Открыть любой txt файл: cat  2qq.txt
10) + написать туда что-нибудь, любой текст: cat >> 2qq.txt
rrrr

tttt
hello
people
123


11) + сохранить и выйти: ctrl+c

12) Выйти из папки на уровень выше: cd ../
Valery@DESKTOP-EEF72K9 MINGW64 /g/home_work/qa

—
13) переместить любые 2 файла, которые вы создали, в любую другую папку:
mv -t test_4 test_3/qq.txt test_3/2qq.txt

проверить папку 4:  ls test_4 
2qq.txt  qq.txt


14) скопировать любые 2 файла, которые вы создали, в любую другую папку: cp -t test_4 test_3/ff.json test_3/fff.json

проверить папку 4 :  ls test_4
4 2qq.txt  ff.json  fff.json  qq.txt

15) Найти файл по имени: find -name 2qq.txt
./test_4/2qq.txt

16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает: tail -f test_4/2qq.txt
rrrr

tttt
hello
people
123

17) вывести несколько первых строк из текстового файла:  head -3 2qq.txt
rrrr

tttt

18) вывести несколько последних строк из текстового файла: tail -2 2qq.txt
people
123

19) просмотреть содержимое длинного файла (команда less) изучите как она работает: less 2qq.txt

20) вывести дату и время:  date 
Sun May 22 15:54:50     2022
=========

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

curl http://162.55.220.72:5005/terminal-hw-request

 % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   283  100   283    0     0   3247      0 --:--:-- --:--:-- --:--:--  3369{
  "Intro": "Hello!! This is your the first response from server",
  "Tasks": {
    "Task_1": "Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)",
    "result": [
      "Your_String",
      "Your_number"
    ]
  }
}

 curl "http://162.55.220.72:5005/get_method?name=valeru&age=8"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    23  100    23    0     0    263      0 --:--:-- --:--:-- --:--:--   267[
  "valeru",
  "8"
]

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

touch skript.sh
ls -la
total 4
drwxr-xr-x 1 Valery 197609 0 May 22 19:53 ./
drwxr-xr-x 1 Valery 197609 0 May 20 19:51 ../
-rw-r--r-- 1 Valery 197609 0 May 22 19:53 skript.sh

cat >> skript.sh
pwd
mkdir QA
cd QA
pwd
mkdir test_6 test_7 test_8
cd test_6
pwd
touch QQ.txt 2QQ.txt 3QQ.txt FFF.json FF.json
ls -la
mkdir h_1 h_2 h_3
ls -la

cat skript.sh
pwd
mkdir QA
cd QA
pwd
mkdir test_6 test_7 test_8
cd test_6
pwd
touch QQ.txt 2QQ.txt 3QQ.txt FFF.json FF.json
ls -la
mv -t test_4 test_3/qq.txt test_3/2qq.txt

chmod +x skript.sh


 ./skript.sh
/g/home_work
/g/home_work/QA
/g/home_work/QA/test_6
total 0
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 .
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 ..
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 2QQ.txt
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 3QQ.txt
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 FF.json
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 FFF.json
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 QQ.txt
total 4
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 .
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 ..
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 2QQ.txt
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 3QQ.txt
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 FF.json
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 FFF.json
-rw-r--r-- 1 Valery 197609 0 May 22 20:00 QQ.txt
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 h_1
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 h_2
drwxr-xr-x 1 Valery 197609 0 May 22 20:00 h_3



1. Сделать папку dir_1:   mkdir dir_1
 2. Зайти в папку dir_1: cd dir_1
 3. Создать папку inner_dir_1: mkdir inner_dir_1
 4. Посмотреть где ты находишься:  pwd
/g/work/dir_1

 5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt : touch tf_1.txt
 6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:
- the first 1
- the second 2
- the third 3
команда: : cat > tf_2.txt
- the first 1
- the second 2
- the third 3
CRTL+D


 7. Зайти в папку inner_dir_1: cd inner_dir_1
 8. Через cat сделать текстовый файл tf_3.txt  c любыми строками 
 cat > tf_3.txt
hellow
CRTL+D
 9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”  cat >> tf_3.txt + сохранить и выйти: ctrl+c
 10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”: cat >> tf_3.txt + сохранить и выйти: ctrl+c
 11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”:
 cd ../ && cat >> tf_2.txt
 12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”: 
  cd inner_dir_1 && cat >> tf_3.txt
 13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”
cd ../ && cat >> tf_2.txt
 14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.
cat >  tf_4.txt 
 15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.
cat >  tF_5.txt
 16. Вывести список всех файлов в папке : find . -maxdepth 1 -type f
 17. Выйти из папки inner_dir_1 :  cd ../
 18. Вывести содержимое файла tf_3.txt в терминал: cd inner_dir_1 && cat tf_3.txt
19. Найти путь к файлу tf_4.txt : realpath tf_4.txt 
 20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.
 cd ../ && echo > tf_4.txt

 21. Найти путь к файлам у которых есть  “tf” в названии:  find . -name "tf*"

 22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре. :   find . -iname "tf*"
 23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке:
grep sec *

 24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке: grep -i sec *

 25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
 grep -w sec *
 26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке grep -i -w sec *

 27. Найти строки в файлах где есть комбинация букв “second” в текущей папке:  
grep second *
 28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке : grep -i second *
 29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем grep -r second
 30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке : grep -l second *


 31. Найти все строки во всех файлах где нет комбинации “second”: grep -v -r  "second"

 32. Найти только название и путь к файлам где нет комбинации “second” :
 grep -r -v -l second

 33. Вывести в терминал 4 последних строк любого текстового файла tail -4 tf_2.txt
 34. Вывести в терминал 4 первые строки любого текстового файла.: head -4 tf_2.txt

 35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым
mkdir new && cd new && cat >> new_1.txt

 36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
grep -rl "sec" | xargs mv -t new

 37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
grep -rl "sec" | xargs cp -t inner_dir_1

 38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
grep -r -h sec | xargs echo > inner_dir_1.txt

 39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
grep -lr " sec " * | xargs rm

 40. Просто вывести в терминал строку “Good job!!” : echo 'Good job!!'
