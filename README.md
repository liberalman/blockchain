# blockchain
区块链开发学习，通过修改现有比特币源码，一步步由浅入深学习区块链技术

### 所需环境
gcc 4.8.5
boost-devel-1.53
注意,1.53版本的BOOST.Operator操作符,比如 '=' 等，可能不兼容C++高版本的编译器，会报错，不要使用gcc 9以上的编译器

### 编译前的准备工作
安装 berkeley db
```sh
$ wget http://download.oracle.com/berkeley-db/db-4.8.30.tar.gz
$ tar xvzf db-4.8.30.tar.gz
$ cd db-4.8.30/build_unix/
$ ../dist/configure --prefix=/usr/local --enable-cxx
$ make
$ make install
```

### 编译
编译我们的项目，进入blockchain
```sh
cd blockchain
./autogen.sh
./configure
make
```



