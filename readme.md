### Задача 1. Установите golang.  
установил
```
C:\Users\Anton>go version
go version go1.18.3 windows/amd64

```

### Задача 2. Знакомство с gotour.

изучил

### Задача 3. Написание кода.

1. Напишите программу для перевода метров в футы (1 фут = 0.3048 метр). Можно запросить исходные данные у пользователя, а можно статически задать в коде. Для взаимодействия с пользователем можно использовать функцию Scanf:

```
package main

import "fmt"

func main() {
	const convert float32 = 0.3048
	var input float32
	fmt.Println("Введите число, которое хотите преобразовать: ")
	fmt.Scanf("%f", &input)
	fmt.Println(input, " метров сконвертировано в футы", input*convert)
}

```
2. Напишите программу, которая найдет наименьший элемент в любом заданном списке, например:
```
x := []int{48,96,86,68,57,82,63,70,37,34,83,27,19,97,9,17,}
```
```
package main

import "fmt"

func main() {
	x := []int{48, 96, 86, 68, 57, 82, 63, 70, 37, 34, 83, 27, 19, 97, 9, 17}
	fmt.Print("Hello ", len(x))
	min := x[0]
	for i := 0; i < len(x); i++ {
		if x[i] < min {
			min = x[i]
		}
	}
	fmt.Println("минимальное значение в массиве x", min)

}

```

3. Напишите программу, которая выводит числа от 1 до 100, которые делятся на 3. То есть (3, 6, 9, …).

```
package main

import "fmt"

func main() {
	fmt.Println("числа, которые делятся на 3 из диапазона [0..100]: ")

	for i := 1; i <= 100; i++ {
		if i%3 == 0 {
			fmt.Println(i)
		}
	}
}

```