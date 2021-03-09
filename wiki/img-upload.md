# Загрузка изображений в файловую систему МК

1. Скачайте плагин для работы с файловой системой микроконтроллера из Arduino IDE

- Для микроконтроллера **ESP8266**
https://github.com/earlephilhower/arduino-esp8266littlefs-plugin

- Для микроконтроллера **ESP32**
https://github.com/lorol/arduino-esp32littlefs-plugin

2. Установите плагин в Arduino IDE:  
 a. Перейдите в папку, где установлена Arduino IDE (обычно `"C:\Program Files (x86)\Arduino\"`)  
 b. Если в папке нет подпапки **tools** - создайте ее, если есть - перейдите в эту папку  
 с. Распакуйте архив **ESP8266LittleFS-2.6.0.zip** для ***ESP8266*** или **ESP32LittleFS.zip** для ***ESP32*** в папку tools - 
    в ней будет создана соответствующая подпапка **ESP8266LittleFS** или **ESP32LittleFS** с файлами плагина  
 d. Перезагрузите Arduino IDE  

3. В папке скетча создайте подпапку **data**

4. В созданной папке data создайте подпапку с именем, соответствующим размерам вашей матрицы. 
   Например для матрицы **16x16** создайте папку **16p16**

5. В созданную папку **16р16** скопируйте файлы картинок из папки **pics/16p16** проекта

6. В Arduino IDE в меню **"Инструменты"** выберите пункт **"ESP8266 LittleFS Data Upload"**

7. Наблюдайте в ArduinoIDE области сообщений ход загрузки файлов, дождитесь сообщения о завершении загрузке и
   о перезагрузке микроконтроллеоа

8. Загрузка файлов завершена.

После выполнения этих действий в приложении на смартфоне ***WiFiPlayer*** будет доступна возможность работы с сохраненными
в файловой системе микроконтроллера картинками.