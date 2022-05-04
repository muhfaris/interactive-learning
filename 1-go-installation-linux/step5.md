Langkah selanjutnya adalah setup environment untuk GoLangnya. Jalankan perintah berikut satu persatu.

`export GOROOT="$HOME/go"`

`export GOPATH="$HOME/workspace"`

`export GOBIN=$GOPATH/bin`

`export PATH=$PATH:$GOROOT/bin:$GOPATH/bin`

Jika sudah, kamu dapat melakukan pengecekan dengan menjalankan perintah `go version` di terminal. Jika installasi berhasil maka akan ditampilkan versi dari Golangnya.

``` 
go version go1.18.1 linux/amd64
```
