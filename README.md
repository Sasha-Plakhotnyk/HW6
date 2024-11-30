#HomeWork6

# Вводити потрібно весь вираз. Наприклад 5*5, 6:2
class Calculator:
    def init(self):
        pass

    def to_float(self, value):
        try:
            result = float(value)
        except ValueError:
            print("Помилка! Введіть ціле число")
            result = None
        finally:
            return result

    def add(self, a, b):
        return a + b #Додавання

    def subtract(self, a, b):
        return a - b #Віднімання
    
    def multiply(self, a, b):
        return a * b #Множення

    def divide(self, a, b): #Ділення на 0
        try:
            result = a / b
        except ZeroDivisionError:
            print("Помилка! На нуль ділити не можна!")
            result = None
        finally:
            return result
