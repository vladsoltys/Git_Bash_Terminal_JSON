1) Посмотреть где я  
> pwd 
2) Создать папку 
> mkdir folder_1
3) Зайти в папку 
> cd folder_1
4) Создать 3 папки 
> mkdir p_1 p_2 p_3
5) Зайти в любоую папку 
> cd p_1
6) Создать 5 файлов (3 txt, 2 json) 
> touch note1.txt note2.txt note3.txt object1.json object2.json
7) Создать 3 папки 
> mkdir l_1 l_2 l_3
8) Вывести список содержимого папки 
> ls ,(ls -la)
9) + Открыть любой txt файл 
> vim note1.txt
10) + написать туда что-нибудь, любой текст. 
> i(insert) I am studying git bush right now
11) + сохранить и выйти. 
> esc :wq
12) Выйти из папки на уровень выше 
> cd ..
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку. 
> mv p_1/{note2.txt,object2.json} p_1/l_3/
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. 
> cp p_1/l_3/{note2.txt,object2.json} p_1/
15) Найти файл по имени 
> find . -name note1.txt
16) просмотреть содержимое в реальном времени изучите как она работает. 
> tail -f p_1/l_1/note1.txt
17) вывести несколько первых строк из текстового файла 
> head -n 2 note1.txt
18) вывести несколько последних строк из текстового файла 
> tail -n 3 note1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. 
> less note_filled.txt
20) вывести дату и время 
> date

**Задание**
1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request 
> - curl http://162.55.220.72:5005/terminal-hw-request
```
                                                 % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                                                                Dload  Upload   Total   Spent    Left  Speed
                                               100   237  100   237    0     0   3251      0 --:--:-- --:--:-- --:--:--  3291{"
                                               Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"
                                               Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_yo
                                               ur_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}
```

> - curl  "http://162.55.220.72:5005/get_method?name="Vlad"&age=24"
                                                
                                                 % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                                                                 Dload  Upload   Total   Spent    Left  Speed
                                            100    14  100    14    0     0    193      0 --:--:-- --:--:-- --:--:--   197["Vlad","24"]

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 

> - touch my_script.txt
                                                                                 
> - vim my_script.txt
```                                                                                 
#!/bin/bash
mkdir new_folder_1
cd new_folder_1
mkdir np_1 np_2 np_3
cd np_1
touch n_note1.txt n_note2.txt n_note3.txt n_object1.json n_object2.
mkdir nl_1 nl_2 nl_3
ls -la
mv n_note2.txt n_object2.json nl_3
esc :wq
```
> - ./my_script.txt

