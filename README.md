# UnixToDate
Простая в использовании библиотека Python для преобразования timestamp в дни.
## Оглавление
1. [Для чего эта библиотека?](https://github.com/Demeneff/unixtodate#Для-чего-эта-библиотека)
2. [Функции](https://github.com/Demeneff/unixtodate#Функции)
3. [Примеры использования](https://github.com/Demeneff/unixtodate#Примеры-использования)

## Для чего эта библиотека
Чтобы посчитать, сколько дней прошло между заданным временем в UnixTimeStamp и сегоднешней датой (выдает количество прошедших дней и слово "день" с нужным окончанием)<br>Работает на русском и на английском

## Функции
Все функции находятся в классе ```ToDate```<br><br>
Класс ```ToDate``` принимает параметры:
- **timestamp** (int) - *время в timestamp*
- **lang** (str) (по умолчанию 'ru') - 'ru' или 'en' (*язык в котором нужно вернуть "день" с соответствующим окончанием*)
<br><br>
***
```get_count_days()```:
- Возвращает количество дней прошедших с заданной даты
<br><br>
***
```get_day_word()```:
- **lang** (str) (необязательно) - 'ru' или 'en' (*язык в котором нужно вернуть "день" с соответствующим окончанием*)
- Возвращает слово "день" с нужным окончанием
<br><br>
***
```get_days_and_word()```:
- **lang** (str) (необязательно) - 'ru' или 'en' (*язык в котором нужно вернуть "день" с соответствующим окончанием*)
- Возвращает количество дней со словом "день"

## Примеры использования
```
from unixtodate import ToDate
n = ToDate(1664502002)
print(n.get_count_days())
# 31

print(n.get_day_word(lang='en'))
# days

print(n.get_days_and_word())
# 31 день
```
