# BigData
Big file sort

Тестовое задание от Altium Limited, которое я когда-то выполнял..

На входе есть большой текстовый файл, где каждая строка имеет вид Number. String 
Например:
415.Apple
30432.Something something something
1.Apple
32.Cherry is the best
2.Banana is yellow

Обе части могут в пределах файла повторяться. Необходимо получить на выходе другой файл, где все строки отсортированы.Критерий сортировки: сначала сравнивается часть String, если она совпадает, тогда Number.

Т.е.в примере выше должно получиться
1.Apple
415.Apple
2.Banana is yellow
32.Cherry is the best
30432.Something something something

Требуется написать две программы:
1.Утилита для создания тестового файла заданного размера. Результатом работы должен быть текстовый файл описанного выше вида.Должно быть какое - то количество строк с одинаковой частью String.

2.Собственно сортировщик.Важный момент, файл может быть очень большой. Для тестирования будет использоваться размер ~100Gb.

Выполнение в данной программе:
1) Загружаем словарь, содержащий слова, которые будем использовать для создания большого файла.
Для этого жмем на кнопку Read dictionary, находим файл Adictionary.txt в папке Dictionary программы и выбираем его.
Видим сколько загрузилось слов. Можно, конечно и свой файл словаря создать.
2) Теперь можно нажать кнопку Create big file, предварительно задав параметры:
какое количество слов из словаря использовать Start and End words index;
какое количество слов будет в каждой строчке файла Words in record;
сколько строк будет в файле Records in file.
3) Создав файл, можем его теперь сортировать. Но сначала выставляем максимальный размер файла, который позволит сортировать ОЗУ Maximum size of file to sort in bytes.
А затем нажимаем кнопку Divide file и выбираем файл. Файл для сортировки надо поместить в пустую папку, так как программа автоматически будет создавать и удалять файлы в этой папке.
4) Как только процесс разбиение файла на мелкие файлы завершиться, переходим ко второму этапу - сортировке записей, нажав на кнопку Sort.
5) После завершения сортировки собираем все в один файл, нажав на кнопку Merge to file и указав название и папку, можно в этой же папке.
Сортировка выполнена.
