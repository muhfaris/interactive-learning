Pada kesempatan kali ini kita akan belajar mengenal program di Golang itu seperti apa?

Perlu kita ketahui bahwa setiap bahasa pemograman itu punya struktur penulisan yang berbeda-beda, Begitu juga dengan Go.


Berikut contoh program sederhana, yang akan kita bahas.

``` 
package main 

import "fmt"

func main(){
    fmt.Println("Hello Gopher")
}
```

Dari program diatas dapat kita ketahui ada 3 keyword, yaitu `package`, `import`, `func`.

#### package
adalah keyword yang digunakan untuk mengidentifikasi nama paket dari suatu kode. Package di Golang itu sebuah kewajiban, jadi kita
tidak bisa membuat suatu kode tanpa mendefinisikan nama `package` atau menghilangkannya, selain itu ketika kita membuat program diharuskan memiliki nama package `main`. Hal
ini dikarenakan Golang akan menjalankan program yang pertama kali dari package `main`.

Kenapa package `main` harus ada disuatu program yang dibuat menggunakan Golang?

> Alasannya karena Golang sendiri akan membaca program itu dimulai dari package `main` terlebih dahulu. Maka ketika suatu program tidak memiliki package `main` yang akan terjadi adalah program tidak akan jalan dan muncul error.


#### import
adalah suatu keyword yang digunakan untuk menampung library-library yang digunakan. Penulisan `import` disini bisa menggunakan format single line untuk satu library atau menggunakan bracket jika library yang digunakan banyak.

Contoh penggunakan import:
```
// single line
// single library

import "fmt"
```

```
// multiple library

import (
    "fmt"
    "time"
    "github.com/google/uuid"
)
```

#### func
Seperti namanya, keyword `func` adalah keyword yang digunakan untuk membuat suatu fungsi / method. Berikut beberapa format dan contoh penggunakan dari fungsi di Golang:

Format penulisan fungsi di Golang:

`func <nama fungsi>() {}`

`func <nama fungsi>() <return type> {return <data>}`

`func <nama fungsi>(<param name> <param type>) <return type> {return <data>}`


Contoh:

Fungsi untuk menghitung penjumlahan antara 2 variabel angka dengan mengembalikan hasil penjumlahan.

```
func Sum(numberA, numberB int) int{
    return numberA + numberB
}
```

Fungsi main diatas memiliki parameter `numberA` dan `numberB`, tipe data dari parameter ini adalah integer(`int`) dan akan mengembalikan nilai dari penjumlahan bertipe integer juga.

