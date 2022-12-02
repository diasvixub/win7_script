# Скрипт по автоматической настройке и установке всего необходимого для Windows 7

## Скрипт для ПК

Запускаем файл `main.cmd`, который произведет подготовку необходимых файлов и откроет конечный каталог посе завершения.

### main.cmd содержит в себе

- Удаляет конечную папку, если она существует
- Создает конечную папку "INST"
- Копирует содержимое папки, в которой находится файл в конечную папку
- Открывает конечную папку после завершения копирования

После открытия папки, запускаем файл "setup.cmd" от имени администратора.

После всех операций, ПК будет перезагружен.

### setup.cmd содержит в себе

- Установку обновлений
- Обновление корневых сертификатов
- Установка библиотек
- Установка базового комлекта ПО
- Оптимизацию Windows

#### Какие обновления включены

- WindowsUpdateAgent
- kb2533552
- kb2545698
- kb2547666
- kb2574819-v2
- kb2603229
- kb2667402-v2
- kb2670838
- kb2676562
- kb2685811
- kb2685813
- kb2698365
- kb2706045
- kb2729094-v2
- kb2732059-v5
- kb2750841
- kb2761217
- kb2773072
- kb2813347
- kb2830477
- kb2834140-v2
- kb2862330-v2
- kb2894844
- kb2900986
- kb2919469
- kb2952664-v25
- kb2970228
- kb2984972
- kb3004375-v3
- kb3006137
- kb3020369
- kb3021917
- kb3046269
- kb3059317
- kb3068708
- kb3080149
- kb3102429-v2
- kb3118401
- kb3123479
- kb3125574-v4
- kb3138612
- kb3140245
- kb3150513
- kb3156016
- kb3159398
- kb3161102
- kb3161949
- kb3172605
- kb3179573
- kb3184143
- kb4019990
- kb4040980
- kb4088878
- kb4099950
- kb4474419-v3
- kb4490628
- kb4524752
- kb5010798
- kb5013637
- kb5017397
- kb5018454
- kb5020000

#### Какие библиотеки включены

- DirectX
- .NET Framework 3.5
- Visual C++ Redistributable 2005-2022

#### Какие программы включены

- 7-Zip
- Google Chrome
- Firefox
- Microsoft Office 2010
- Notepad ++
- GDevelop
- GIMP
- PyCharm Community
- Visual Studio Code
- VLC
- Python 3.7

#### Какие операции оптимизацие произведены

**Отключение ненужных компонентов Windows**

- Платформа гаджетов Windows
- Игры

**Отключение неиспользуемых служб**

- Windows Search
- Архивация Windows
- Служба ввода планшетного ПК
- Служба поддержки Bluetooth
- Служба шифрования дисков BitLocker
- Центр обновления Windows
- Теневое копирование тома
- Смарт-карта
- Защитник Windows

**Настройка файла подкачки (4ГБ)**

**Включение показа расширения файлов**

**Очистка временных файлов**

- C:\Windows\SoftwareDistribution\Download\
- C:\Windows\Prefetch\
- %temp%
- C:\INST

## Скрипт для ноутбуков

Запускаем файл `main.cmd`, который произведет подготовку необходимых файлов и откроет конечный каталог посе завершения.

После открытия папки, запускаем файл `setup_noUpd.cmd` от имени администратора.

После всех операций, ПК будет перезагружен.

`setup_noUpd.cmd` в отличии от `setup.cmd` имеет ту же функциональность, за исключением установки обновлений.

## Скрипты для ручной установки

Скрипты запускать по порядку

1. updates.cmd
2. certs.cmd
3. lib.cmd
4. program.cmd
5. boost.cmd
6. clean.cmd

### Что делают скрипты

Номер соответствует скрипту

1. Устанавливает обновления
2. Обновляет корневые сертификаты
3. Устанавливает библиотеки
4. Устанавливает программы
5. Оптимизирует Windows (за исключением очистки временных файлов)
6. очистка временных файлов
