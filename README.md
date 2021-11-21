price = []
ticket = int(input("Сколько билетов хотите приобрести:"))
age = int(input("Сколько вам лет:"))
if 0 <= age < 18:
    price.append(0)
elif 18 <= age <= 25:
    price.append(990)
elif 25 <= age <= 140:
    price.append(1390)
if ticket > 3:
    print("Сумма к оплате с учетом скидки за один билет: ", sum(price) - ((sum(price) / 100) * 10), "рублей")
else:
    print("Сумма к оплате: ", sum(price), "рублей")
