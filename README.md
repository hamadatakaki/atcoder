# AtCoderローカル実行環境 with Docker

## 対応言語(2019/03/11)
* golang:latest

## setup
```
$ git clone git@github.com:hamadatakaki/atcoder.git
$ cd atcoder
$ sh setup.sh
```

## 各実行環境の動かし方
1. 実行したいファイルを、その言語下の`src`に移す
2. まだコンテナをbuildしてないなら`sh build.sh`を実行
3. `sh runner.sh`を実行
4. コンテナ内に入るので`src/<ファイル名>`を実行
5. 満足したら`exit`

## 例（Golang)
```
$ cd go
$ mv /path/to/target.go ./src
($ sh build.sh)
$ sh runner.sh
> go run src/target.go
> exit
```