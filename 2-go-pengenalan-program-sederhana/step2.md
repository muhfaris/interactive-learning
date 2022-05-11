Untuk memahami lebih dalam tentang program dan fungsi di Golang, Kita akan belajar dengan studi kasus membuat program sederhana perhitungan atau
kalkulator sederhana. Sebelum lanjut, kita definisikan terlebih dahulu batasan-batasan program yang akan kita buat:
- penjumlahan 2 angka
- pengurangan 2 angka

Langkah pertama buat file terlebih dahulu dengan nama `main.go`, perintah yang dijalankan adalah `touch main.go`.

Kemudian setelah file berhasil dibuat, ketik kode berikut ke `main.go` via editor:

```
package main

import "fmt"

func main() {
	var number1 = 10
	var number2 = 10

	total := addition(number1, number2)
	fmt.Printf("%d + %d = %d\n", number1, number2, total)

	total = subtraction(number1, number2)
	fmt.Printf("%d - %d = %d\n", number1, number2, total)
}

func addition(number1, number2 int) int {
	return number1 + number2
}

func subtraction(number1, number2 int) int {
	return number1 - number2
}

```

Setelah itu jalankan program, dengan menjalankan perintah `go run main.go` di terminal.

Ekpektasi hasil dari program di atas adalah:
``` 
10 + 10 = 20
10 - 10 = 0
```

Hal yang baru dari kode diatas adalah `fmt.Printf`, sedangkan pada contoh sebelumya kita menggunakan `fmt.Println`. Kita memanfaatkan fungsi `fmt.Printf` karena kita bisa membuat sebuah template text tertentu beserta mengirimkan value yang diperlukan.

Pada dasarnya kita juga bisa menggunakan perintah `fmt.Println`, tapi kode yang dihasilkan akan kurang rapi. Berikut perbandingan antara menggunakan
perintah `fmt.Printf` atau `fmt.Println`

``` 
// fmt.Printf

    fmt.Printf("%d - %d = %d\n", number1, number2, total)
```

``` 
// fmt.Println

    fmt.Println(number1, "+", number2, "=", total)
```

Lebih rapi yang menggunakan `fmt.Printf`, bukan?

Bayangkan jika kalimat yang harus disusun panjang dan value yang harus digunakan juga banyak, kemungkinan human error ketika menggunakan perintah
`fmt.Println` lebih besar. Ingat ketika kita membuat suatu program, sebisa mungkin kode yang dibuat itu mudah dibaca oleh orang lain juga.
