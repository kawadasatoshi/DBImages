

## commands:コマンド入力


### 1. clone this repo

本リポジトリのソースコードをダウンロードします。

```sh
git clone https://github.com/kawadasatoshi/DBImage.git
```


### 2. move to "mysql" directory

mysqlディレクトリにcdコマンドで移動します。

```sh
cd DBImage/mysql/
```


### 3. build mysql image

mysqlイメージをbuildします。

```sh
docker image build -t mysql .
```


### 4. start mysql server

```sh
docker run -d -v ${PWD}/code:/code --name mysqlcon mysql
```


### 5. run mysqlcon container

```sh
docker exec -it mysqlcon bash
```

```sh
mysql -u root -proot
```


### 6. 
inside container


```sh
docker stop mysqlcon
docker rm mysqlcon
```



