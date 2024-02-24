@startuml
left to right direction
skinparam actor {
    BackgroundColor LightBlue
    BorderColor DarkBlue
}

actor "Пользователь" as User

rectangle "Текстовый редактор" {
    User --> (Создать новый файл)
    User --> (Открыть существующий файл)
    User --> (Редактировать файл)
    User --> (Сохранить файл)
    User --> (Печать файла)
    (Открыть существующий файл) --> (Отобразить содержимое файла)
    (Редактировать файл) --> (Ввод текста)
    (Редактировать файл) --> (Подсветка ключевых слов)
}
@enduml

![image](https://github.com/bondarenkosa11/pr1_Uml/assets/161125446/28455a7f-8341-4adf-9c36-6af1f89b3d13)
