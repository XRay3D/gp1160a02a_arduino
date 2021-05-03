# Простая библиотека для работы с gp1160a02a на arduino
Проект с простой библиотекой для работы с VFD экраном GP1160A02A

**Внимание!** Экран потребляет довольно много тока по линии +5 вольт (при полном заполнении и максимальной яркости 1.3 А) поэтому советую запитать дисплей отдельно от arduinо при прошивке или, подключать arduino к компьютеру после подачи питания на схему.

Для установки используйте zip архив с вкладки релиз.

В тестовом скетче sketch.ino можно посмотреть как работать с библиотекой.

## список реализованных функций

* clear - очистка экрана
* send_mode - установка режима вывода текста (размер шрифта)
* send_str - выводит текст (с поддержкой кирилицы) со сдвигом курсора
* set_dimming - настройка яркости (5 уровней от 0 до 5)
* set_scroll - вывод бегущей строки
* print_graph - вывод изображения из flash памяти

Изображения можно  подготовить с помощью следующего сервиса: <https://javl.github.io/image2cpp/>

При установке 1 режима работы экрана, когда текст выводиться шрифтом с размером 5 на 7 кириллица не доступна!