# Laboratory-work-2 variant-2

while True:
    sentence = input("Введіть речення:")

    # Перевірка на валідність даних (наприклад, чи не є порожнім рядок)
    if sentence.strip() == "":
        print("Помилка: Ви ввели порожній рядок. Спробуйте ще раз.")
        continue  # Повторний запит на введення даних

    words = 0
    symbols = 0

    something = False

    # цикл для підрахунку к-ті символів і слів
    for char in sentence:
        symbols += 1
        if char != ' ' and something == False:
            words += 1
            something = True
        elif char == ' ':
            something = False

    # виведення слів і сумволів
    print("Слів:", words)
    print("Символів:", symbols)

    # Вихід з циклу, якщо дані були успішно оброблені
    break

