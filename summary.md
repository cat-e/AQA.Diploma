# Отчет по итогам автоматизации

### Что было запланировано и что было сделано

В ходе автоматизации тестирования веб-сервиса "Путешествие дня" запланировано для автоматизации 20 тестовых сценариев, автоматизировано 26 тестовых сценариев.  
Были дополнительно написаны автотесты для проверки отправки POST-запроса в случае указания некорректного значения для поля Владелец. Пришлось это сделать,
т.к. выяснилось, что для данного поля не установлено никаких ограничений на ввод (в т.ч. на возможность ввода sql-инъекции и т.п.).
Также дополнительно были написаны автотесты для проверки появления предупреждений при заполнении полей некорректными значениями, т.к. для данного фукционала было
выявлено много ошибок.

### Сработавшие риски

Из-за отсутствия ТЗ и какой-либо документации сложно судить, насколько корректно были выбраны сценарии для написания автотестов.
Возникли проблемы с указанием volumes для контейнера postgres.

### Общий итог по времени

Сложно определить точное время, потраченное на автоматизацию, при этом обязательство по итоговым срокам сдачи работ также было выполнено с задержкой из-за неглубокого знания кодинга.
По факту написание тестов заняло меньше времени, чем предполагалось. При этом довольно много времени ушло на то, чтобы разобраться, как необходимо запускать
приложение и как именно нужно передавать параметры при запуске приложения и при запуске автотестов.