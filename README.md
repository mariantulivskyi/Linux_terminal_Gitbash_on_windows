
# Linux terminal (GitBash on Windows) commands:
**1) Посмотреть где я.**
```pwd```

**2) Создать папку.**
```mkdir first-folder```

**3) Зайти в папку.**
```cd first-folder```

**4) Создать 3 папки.**
```mkdir folder1 folder2 folder3```

**5) Зайти в любую папку.**
```cd folder1```

**6) Создать 5 файлов: (3 txt, 2 json).**
```touch file{1..3}.txt file2{1..2}.json```

**7) Создать 3 папки.** ```mkdir test-folder{1..3}```

**8) Вывести список содержимого папки.** ```ls / ls -la / ls -l``` 

**9) + Открыть любой txt файл.** ```vim file1.txt```

**10) + написать туда что-нибудь, любой текст.** ```Press "I" and write  «Hello World»``` 

**11) + сохранить и выйти.**```press ESC and write :wq.```

**12) Выйти из папки на уровень выше.** ```cd ..```

**13) переместить любые 2 файла, которые вы создали, в любую другую папку.** ```mv file3.txt file2.txt /lesson-gitbash/test-folder1```

**14) скопировать любые 2 файла, которые вы создали, в любую другую папку.** 
```cp file21.json file22.json /lesson-gitbash/test-folder1```

**15) Найти файл по имени.** ```find -name file2.txt```

**16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.** 
```tail -f file2.txt | grep "s" выдает содержимое файла со строкой содержащей «s».```

**17) вывести несколько первых строк из текстового файла.** ```head file2.txt или если надо только первые 3 строки: head -3 file2.txt```

**18) вывести несколько последних строк из текстового файла.** 
```tail -2 file1.txt1 вывести последние 2 строки или просто tail file1.txt для последних 10 строк```

**19) просмотреть содержимое длинного файла (команда less) изучите как она работает.** ```Less file1.txt```

**20) вывести дату и время.** ```date```


**1) Отправить http запрос на сервер.	http://162.55.220.72:5005/terminal-hw-request**	 ```curl "http://162.55.220.72:5005/get_method?name=Marian&age=25"```

**2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13**  		 ```Создать файл  homework.sh```

 *Внутри файла:	homework.sh*

``` 
#!/bin/bash
#sctript HW-Gitbash
mkdir gitbash-script
cd gitbash-script
mkdir gb-scrpt-here
cd gb-scrpt-here
touch info{1..3}.txt footer.txt title.txt
mkdir background{1..3}
ls -la
mv info1.txt title.txt ~/test-script/gbash
Вводим команду sh homework.sh в Gitbash
