a, b = map(int, input().split())

x, y = 0, 1
res = []

while x <= b:
    if x >= a:
        res.append(x)
    x, y = y, x + y

if res:
    print(*res)
else:
    print("В заданном диапазоне нет чисел Фибоначчи")
