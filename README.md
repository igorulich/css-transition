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
