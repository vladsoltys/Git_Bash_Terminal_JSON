# JSON

1. Создать внешний репозиторий c названием JSON.
>    Go to home page --> click on the button "New"(on the upper left) --> enter name "JSON" --> at the bottom click "Create repository"    
2. Клонировать репозиторий JSON на локальный компьютер. 
>    git clone https://github.com/vladsoltys/JSON.git --> cd JSON
3. Внутри локального JSON создать файл “new.json”. 
>    touch new.json
4. Добавить файл под гит.
>    git add new.json
5. Закоммитить файл. 
>    git commit -m "add new json file"
6. Отправить файл на внешний GitHub репозиторий. 
>    git push
7. Отредактировать содержание файла “new.json” - написать информацию о себе 
     (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). 
     Всё написать в формате JSON. 
>    - vim new.json  
>    - i ***(insert)***
     
       {
           "Full_name": "Soltys Vladyslav Igorevich",
           "Age": 24,
           "Number_of_pets": 2,
           "Future_desired_salary": "800-1000$"
       }
                                                                                
>    - esc :wq

 8. Отправить изменения на внешний репозиторий. 
>    - git commit -am "fixed syntax errors"
     - git push

 9. Создать файл preferences.json 
>    vim preferences.json
 10. В файл preferences.json добавить информацию о своих предпочтениях 
     (Любимый фильм, любимый сериал, любимая еда, любимое время года, страна которую хотели бы посетить) 
     в формате JSON.
>    - i ***(insert)***

        {
            "Favourite_film": "Contact",
            "Favourite_series": "Breaking Bad",
            "Favorite_food": "Mother's potato pancakes with cheese",
            "Favorite_time_of_year": "Summer",
            "Country_you_would_like_to_visit": "Cuba"
        }
        
>    - esc :wq

 11. Создать файл skills.json,
     добавить информацию о скиллах которые будут изучены на курсе в формате JSON
>    - vim skills.json
>    - i ***(insert)***
     
        {
             "skills_to_be_learned_on_the_course": [
                 "Basic theory (What is testing, bug reports, documentation, types, methods, testing directions, etc.) SDLC, STLC",
                 "What is a client-server architecture",
                 "HTTP Methods of requests to the server",
                 "HTTP server response codes",
                 "Structures of HTTP requests and responses",
                 "What is JSON, XML. Their structure",
                 "API testing via Postman (JS, API autotests)",
                 "Removing and reading logs from an external server",
                 "Sniffing http web traffic via Charles and Fiddler",
                 "Dev Tools of web browsers (Google Chrome, FireFox)",
                 "VPN. (How it works, why you need it, how to use it, tool options)",
                 "Mobile testing",
                 "Feature iOS, Android, guidelines",
                 "Building iOS applications on XCode",
                 "Building Android applications on Android Studio",
                 "ADB (android device management)",
                 "Setting up proxy and vpn on iOS and Android",
                 "Interception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android",
                 "Command line (terminal) Linux (copying, creating, viewing, moving files on servers without a graphical interface)",
                 "Basics of bash scripting, automation of routine tasks on the server",
                 "Access to remote servers",
                 "SQL basics (Create, Delete, Drop, Insert Into, Select, From, Where, Join)",
                 "Postgres database (installation, configuration and use)",
                 "Non-relational database Redis (installation, configuration and use)",
                 "Load testing in Jmeter",
                 "Scrum development methodology",
                 "Python. (Learning the basics. Creating a client-server application)"
             ]
        }

>    - esc :wq

 12. Отправить сразу 2 файла на внешний репозиторий.
>    git add preferences.json skills.json
>    git commit -m "add 2 files"  
>    git push

 13. На веб интерфейсе создать файл bug_report.json. 
>    - click on the button "add file" 
>    - click on the button "create new file" 
>    - in the field "Name your file..." enter the name of the file "bug_report.json"

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
>    at the bottom click "Commite new file"
 15. На веб интерфейсе модифицировать файл bug_report.json, 
     добавить баг репорт в формате JSON.
>    - click on file "bug_report.json"
>    - click on the button "Edit this file" in the lower right
>    - copy description of the bug
   
        {
         "Bug_id": 26,
         "Summary": "Loggin Page. The button 'Sigh in' not responding after clicking on it",
         "STR": {
             "step_1": "Open the login page",
             "step_2": "Enter username and password",
             "step_3": "Click on the button 'Sigh in'"
         },
         "Result": "The button 'Sigh in' not responding after clicking on it",
         "Expected_result": "After clicking the button, the user page opens",
         "Severity": "Major",
         "Priority": "High",
         "Enviroment": {
              "OS": "Windows 10 Pro.64-разрядная операционная система, процессор x64",
              "Browser": "Google Chrome v.98.0.4758.102 (Розробка) (64-розрядна версія)"
         } 
     }


 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе. 
>    at the bottom click "Commite new file"
 17. Синхронизировать внешний и локальный репозиторий JSON
>    git pull
