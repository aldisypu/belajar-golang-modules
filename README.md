### EMBUAT MODULE
- go mod init nama-MODULE

### RILIS MODULE
#### membuat Tag di Git

1. git init
2. git add go.mod
3. git add say_hello.go
4. git status
5. git commit -m 'membuat module say-hello'
6. git remote add origin https://github.com/aldisypu/go-say-hello.git
7. git push origin master

- git tag v1.0.0
- git push origin v1.0.0

### MENAMBAH DEPENDENCY
- go get nama-module

### UPGRADE MODULE
#### membuat tag baru di Git
- git tag v1.5.0
- git push origin v1.5.0

### UPGRADE DEPENDENCY
- mengubah isi go.mod, lalu mengubah tag nya menjadi tag terbaru
- untuk mendownload versi terbaru, gunakan perintah: go get

### MAJOR UPGRADE
- sebaiknya dihindari
- jika tidak bisa dihindari, strategi terbaiknya merubah nama module
- module github.com/aldisypu/go-say-hello/v2
- git tag v2.0.0
- git push origin v2.0.0