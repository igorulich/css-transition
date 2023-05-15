# transition
transition CSS-переходу є скороченим властивістю для **transition-property, transition-duration, transition-timing-function, and transition-delay**.
* /* Застосувати до 1 властивості */
* /* назва властивості | тривалість */
* *transition: margin-right 4s*;

* /* назва властивості | тривалість | затримка */
* *transition: margin-right 4s 1s*;

* /* назва властивості | тривалість | функція ослаблення */
* *transition: margin-right 4s ease-in-out*;

* /* назва властивості | тривалість | функція полегшення | затримка */
* *transition: margin-right 4s ease-in-out 1s*;

* /* Apply to 2 properties */
* *transition: margin-right 4s, color 1s*;

* /* Застосувати до всіх змінених властивостей */
* *transition: all 0.5s ease-out*;

* /* Глобальні значення */
* *transition: inherit*;
* *transition: initial*;
* *transition: revert*;
* *transition: revert-layer*;
* *transition: unset*;
* // content: linear-gradient(#fffdfd6e, #f9f9fa54);
*****************************************************************************
/* Ключевые слова, которые нельзя комбинировать с другими значениями */
content: normal;
content: none;

/* значение <url>  */
content: url("http://www.example.com/test.png");

/* значение <image>  */
content: linear-gradient(#e66465, #9198e5);

/* указанные ниже значения могут быть применены только к сгенерированному контенту с использованием ::before и ::after */

/* значение <string>  */
content: "prefix";

/* значения <counter> */
content: counter(chapter_counter);
content: counters(section_counter, ".");

/* значение attr() связано со значением атрибута HTML */
content: attr(value string);

/* языко- и позиция-зависимые ключевые слова */
content: open-quote;
content: close-quote;
content: no-open-quote;
content: no-close-quote;

/* несколько значений могут использоваться вместе */
content: open-quote chapter_counter;

/* глобальные значения */
content: inherit;
content: initial;
content: unset;
