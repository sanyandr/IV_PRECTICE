# IV_PRACTICE

Структура и иерархия файлов не была отредактирована до конца </br>
Выполненные задания (насколько посчитал правильным) 

**Создал** БД с таблицей отзывов, ее конфиг файл, объект хранилища отзывов "ReviewObject", </br>
функции для работы с базой (
  * удалить по ID, 
  * получить один по ID, 
  * получить все, 
  * получить ограниченное количество)\
  
**Контроллеры** (
  * HelloWorld, 
  * /Home (все отзывы), 
  * отзыв по ID, 
  * список отзывов с постраничной навигацией, страница прописывается опционально в URL, если = null => 1
  * удаления, ID удаляемого отзыва указывается в URL
  * Add и Update пока не сделал 
возвращают $response с content-type: application/json) \

Защита контроллера удаления (конкретного route) c помощью Tuupola\Middleware\HttpBasicAuthentication (slim BASIC auth) </br>
Сверстал форму, но пока не применял (как я понял это оптимально) render() для отображения и не разбирал JS </br>
Функции, которые должны быть в ReviewObject class я вынес в отдельный dbFunctions class, но понимаю, что они должны быть внутри ReviewObject. 
