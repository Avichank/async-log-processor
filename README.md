Задача: "Асинхронный обработчик логов"
Ты пишешь программу, которая должна асинхронно обрабатывать логи из нескольких файлов. Каждый файл содержит строки с логами, и программа должна:

Читать логи из файлов.

Обрабатывать каждую строку лога (например, извлекать определённую информацию).

Сохранять результаты обработки в новый файл.

Использовать горутины и каналы для параллельной обработки файлов.

Требования:
Создай интерфейс LogProcessor, который будет иметь метод ProcessLog(line string) string.

Реализуй структуру ErrorLogProcessor, которая будет извлекать из лога сообщения об ошибках (например, строки, содержащие слово "ERROR").

Реализуй структуру InfoLogProcessor, которая будет извлекать информационные сообщения (например, строки, содержащие слово "INFO").

Напиши функцию ProcessFile, которая:

Принимает имя файла и LogProcessor.

Читает файл построчно.

Обрабатывает каждую строку с помощью LogProcessor.

Записывает результат в новый файл (например, имя_файла_processed.txt).

Используй горутины и каналы для параллельной обработки нескольких файлов.

В функции main создай несколько файлов с логами и продемонстрируй работу программы.