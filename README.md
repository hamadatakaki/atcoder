你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# AtCoderローカル実行環境 with Docker

## 対応言語(2019/03/11)
* golang:1.6

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
