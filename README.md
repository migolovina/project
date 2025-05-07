<picture align="center">
  <img alt="Pandas Logo" src="https://shbpacademy.com/wp-content/uploads/2023/01/Depositphotos_475507236_XL-840x450.jpg">
</picture>

-----------------

# Проект: Генератор безопасных паролей

| | |
| --- | --- |
| Мой канал | [[Rutube](https://rutube.ru/plst/909045/)] |
| Мой канал | [[plvideo](https://plvideo.ru/playlist?list=SuymwXRNSHg3)] |
| Мой github | [[GitHub](https://github.com/migolovina/)]|

## Что это?

Мой проект на тему "Генератор безопасных паролей".

## Цель

Написать программу, которая создаёт случайные пароли заданной длины с использованием букв, цифр и спецсимволов.

# Что потребуется

- Язык: **Python** (можно использовать любой онлайн-компилятор или установленный IDE). 
- Библиотеки: `random` (встроенная, ничего дополнительно ставить не нужно). 

# Почему это хороший проект: 
✅ Просто и понятно для новичков. 
✅ Полезно в реальной жизни. 
✅ Можно расширять и усложнять.

# Код программы

```python
import random
import string

def generate_password(length=12):
    # Символы, из которых будет составляться пароль
    characters = string.ascii_letters + string.digits + string.punctuation
    # Генерация пароля
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Основная программа
if __name__ == "__main__":
    print("Генератор безопасных паролей")
    length = int(input("Введите длину пароля: "))
    password = generate_password(length)
    print(f"Ваш пароль: {password}")

