Dalam Bahasa Golang sendiri pada dasarnya kita dibebaskan untuk menaruh projek dimana saja, akan tetapi disini kita akan membuat folder khusus untuk
menyimpan semua projek Golang.

Beberapa alasan kenapa kita buat folder khusus:
1. Memudahkan kita dalam mencari projek
2. Memudahkan kita dalam development.
3. Memudahkan dalam menejemen dependency menggunakan Go Module.

Sebelum ke struktur folder kita akan bahas sedikit environment-environment dari Golang yang akan kita gunakan:

`GOROOT` adalah environemtn untuk menyimpan lokasi dari bahasa Go sendiri.

`GOPATH` adalah environment untuk menyimpan lokasi dari berbagai projek Go. 

`GOBIN` adalah environment untuk menyimpan semua binary hasil build dari Go.

Environment diatas akan kita set setelah installasi selesai. Selain itu jika kamu sudah paham tentang environment-environemnt ini kamu bisa merubah
lokasi foldernya sesuai kebutuhan.

Struktur folder yang akan kita gunakan adalah seperti berikut:
``` 
/home/muhfaris/workspace
├── bin
├── gomod
├── pkg
└── src # untuk menyimpan semua project
```
