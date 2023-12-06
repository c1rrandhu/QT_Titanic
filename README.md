Проект может быть использован в бизнес сфере для быстрого получения информации о конкретном человеке, чтобы произвести с ним сделку. 
В моей базе данных в качестве примера используются пассажиры Титаника, в базе данных хранятся их персональные данные: имя, возраст, пол, кол-во детей итд. 
Приложение универсально, и с незначительными изменениями "под капотом" может функционировать для любой базы данных.

#######################################################################################################

Для работы с кодом поместите requirements.txt, .py файлы с фронтэндом (названы main_design.py, editWindow_design.py и photo_design.py) и .py файл с 
бэкендом (назван main.py), базу данных "database", а также .jpg и .png изображения (названы anonymus.png, cat.png, anonym.jpg, dog.jpg, flowers.jpg) в текущую директорию. 
В консоли IDE запустите команду:

pip install -r /*Путь до файла*

#######################################################################################################

Инструкция по работе:

а) При запуске откроется главное окно, в котором непосредственно делается запрос к базе данных.

б) Для осуществления запроса в соответствующее поле вводится текст и нажимается кнопка "Найти в БД".
Осуществлять запрос можно по маске, где "_" – любой один символ; "%" – любое количество любых символов. 
Или при помощи логических операций AND и OR.

в) Полученный запрос можно выгрузить в виде .csv или .txt файла, нажав на кнопку "Выгрузить запрос".
Обратите внимание, если запрос пустой, т. е. в базе данных нет такой информации, или Вы нажали кнопку,
не установив значения в ячейки, система предупредит Вас об этом.

г) В базу данных можно внести свои корректировки: нажав на кнопку "Внести правки", откроется диалоговое окно, с помощью
которого можно удалить, обновить или вставить значения в базу данных.

    в.1) Чтобы удалить значения необходимо ввести id соответствующего человека и критерий, т. е. название ячейки, которую
    необходимо удалить. При этом, если не указать id, запрос будет выполнен, однако удалится вся информация по данному
    человеку. Если не указать критерий, система оповестит вас об ошибке.
    
    в.2) Чтобы обновить/изменить значения в ячейке необходимо так же указать id, но необязательно указывать критерий.
    Необходимые значения следует записать в соответствующие строки ввода. Обратите внимание, если оставить строку пустой,
    значение в соответствующей ячейке удалится из базы данных.
    
    в.3) Чтобы вставить информацию, необходимо указать требуемые значения в строки ввода. Критерий и id указывать
    не нужно. Новая информация будет помещена в конец базы данных.
    
д) Для поиска фотографии человека необходимо нажать на кнопку "Найти фото" и в открывшемся окне указать id человека. Затем нажать кнопку "Найти".

e) Также в приложение встроена функция горячих клавиш: при сочетании "ALT + SHIFT + S" можно произвести быструю выгрузку CSV-файла.
