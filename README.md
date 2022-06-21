# Git_hw_2
1. Сделать папку dir_1
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2 (master)
$ mkdir dir_1

2.Зайти в папку dir_1
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2 (master)
$ cd dir_1

 3. Создать папку inner_dir_1
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ mkdir inner_dir_1

 4. Посмотреть где ты находишься
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ pwd
/c/Users/mashi/Documents/git 2/dir_1

 5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ touch tf_1.txt


6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ cat>> tf_2
- the first 1
- the second 2
- the third 3

 7. Зайти в папку inner_dir_1
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ cd inner_dir_1

 8. Через cat сделать текстовый файл tf_3.txt  c любыми строками
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat>> tf_3.txt
1
2


9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat >> tf_3.txt
the second 2

10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat>> tf_3.txt
the sec 2

 11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”
(mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1/inner_dir_1 (main)
$ cat >> ./../tf_2.txt
the sec 3


12.Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat >> tf_3.txt
the SeCoNd 2

13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1/inner_dir_1 (main)
$ cat >> ./../tf_2.txt
the seCond 2


14. Сделать текстовый файл tf_4.txt в котором будет 14 строк.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat>> tf_4.txt
    











15.Сделать текстовый файл tF_5.txt в котором будет 13 строк.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cat>> tF_5.txt









16.Вывести список всех файлов в папке.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ ls -la
total 3
drwxr-xr-x 1 mashi 197609  0 May 27 22:12 ./
drwxr-xr-x 1 mashi 197609  0 May 27 22:07 ../
-rw-r--r-- 1 mashi 197609 36 May 27 22:12 tF_5.txt
-rw-r--r-- 1 mashi 197609 54 May 27 22:09 tf_3.txt
-rw-r--r-- 1 mashi 197609 30 May 27 22:11 tf_4.txt
 
17.Выйти из папки inner_dir_1

mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1/inner_dir_1 (master)
$ cd ..

18. Вывести содержимое файла tf_3.txt в терминал.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ less tf_4.txt ./*
tf_4.txt: No such file or directory
./inner_dir_1 is a directory
./q1 is a directory
Press RETURN to continue



 19. Найти путь к файлу tf_4.txt
$ find . -name '*tf_4.txt*' -print
./inner_dir_1/tf_4.txt

 20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/dir_1 (master)
$ echo  > tf_4.txt



 21. Найти путь к файлам у которых есть  “tf” в названии.
 
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ find . -name '*tf*' -print
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./tf_1.txt
./tf_2.txt




22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.

mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ find . -iname '*tf*' -print
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tF_5.txt
./tf_1.txt
./tf_2.txt




 23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке

mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ grep -RH 'sec' .
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_3.txt:the second 2
./tf_2.txt:- the second 2
./tf_2.txt:- the sec 3





 24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ grep -RiH 'sec' ../dir_1
../dir_1/inner_dir_1/tf_3.txt:the second 2
../dir_1/inner_dir_1/tf_3.txt:the SeCoNd 2
../dir_1/tf_2.txt:- the second 2
../dir_1/tf_2.txt:- the sec 3
../dir_1/tf_2.txt:the seCond 2



 25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -ri -w 'sec' ./../dir_1
./../dir_1/inner_dir_1/tf_3.txt:the sec 2
./../dir_1/tf_2.txt:- the sec 3






 26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -Ri -w 'sec' .
./inner_dir_1/tf_3.txt:the sec 2
./tf_2.txt:- the sec 3





 27. Найти строки в файлах где есть комбинация букв “second” в текущей папке
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -Rw 'second' ./../dir_1
./../dir_1/inner_dir_1/tf_3.txt:the second 2
./../dir_1/tf_2.txt:- the second 2




 28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -Riw 'second' ./../dir_1
./../dir_1/inner_dir_1/tf_3.txt:the second 2
./../dir_1/inner_dir_1/tf_3.txt:the SeCoNd 2
./../dir_1/tf_2.txt:- the second 2
./../dir_1/tf_2.txt:the seCond 2





 29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -rw 'second' ./*
./inner_dir_1/tf_3.txt:the second 2
./tf_2.txt:- the second 2



 30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке

mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -rwl 'second' .
./inner_dir_1/tf_3.txt
./tf_2.txt





 31. Найти все строки во всех файлах где нет комбинации “second”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -R -v 'second' *
11.txt:one
11.txt:two
11.txt:three
inner_dir_1/tf_3.txt:
inner_dir_1/tf_3.txt:the sec 2
inner_dir_1/tf_3.txt:the SeCoNd 2
inner_dir_1/tf_3.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tf_4.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
inner_dir_1/tF_5.txt:
tf_2.txt:- the first 1
tf_2.txt:- the third 3
tf_2.txt:- the sec 3
tf_2.txt:
tf_2.txt:
tf_2.txt:the seCond 2





 32. Найти только название и путь к файлам где нет комбинации “second”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  grep -rv -L 'second' .
./inner_dir_1/git
./tf_1.txt




 33. Вывести в терминал 4 последних строк любого текстового файла
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ tail -n4 tf_2.txt
- the sec 3


the seCond 2

 34. Вывести в терминал 4 первые строки любого текстового файла.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ head -n4 ./*/tf_4.txt




 35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/dir_1 (master)
$ mkdir q1 && cat>> 11.txt
one
two
three



 36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ for file in $(grep 'sec' -rl); do mv "$file" ./q1; done;



 37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”

mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$ for file in $(grep 'sec' -rl); do cp "$file" ./q1; done;
cp: 'q1/tf_2.txt.txt' and './q1/tf_2.txt.txt' are the same file
cp: 'q1/tf_3.txt.txt' and './q1/tf_3.txt.txt' are the same file



 38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл
mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  for file in $(grep 'sec' -rl); do cp -av "$file" ./11.txt; done;
'q1/tf_2.txt.txt' -> './11.txt'
'q1/tf_3.txt.txt' -> './11.txt'



 39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
 mashi@DESKTOP-3PNNHT0 MINGW64 ~/Documents/git 2/Git-2/dir_1 (main)
$  for file in $(grep 'sec' -ril); do rm "$file" ./; done;

