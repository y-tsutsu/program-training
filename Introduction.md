# 初めてのPythonプログラム

## 前提知識

本項目を進めるにあたって，以下の内容をおおよそ知っていることを前提とする．

* 変数を知っている
* 関数を知っている
* 条件分岐（if文，switch文）を知っている
* 繰り返し（for文，while文）を知っている

## Dive Into Python 3

下記のURLの内容を理解する．

[http://diveintopython3-ja.rdy.jp/your-first-python-program.html](http://diveintopython3-ja.rdy.jp/your-first-python-program.html)

## コピペしたサンプルコードを実行する

手元の環境でコピペしたコードを実行することに慣れる．

```console
$ python3 spam.py
```

## 変数に慣れる

* 変数の宣言と読み書きができるようになる．
* 変数の型を理解する．（型の詳細は次章で行います）
* 変数の寿命（スコープ）を理解する．

## 関数に慣れる

* 引数に任意の値を渡して，戻り値を受け取れるようになる．
* 標準関数を何個か使ってみる．
* 自作の関数を定義して使ってみる．

## インデントに慣れる

* インデントでブロックを理解する．
* 手元のエディタでスマートインデントとコード成型が手軽に行えるようにする．
* `pass`について理解する．

## 条件分岐について

Pythonでのif文の書き方に慣れる．また，Pythonにはswitch文はない．

```py
if i % 15 == 0:
    print('FizzBuzz')
if i % 3 == 0:
    print('Fizz')
elif i % 5 == 0:
    print('Buzz')
else:
    print(i)
```

## 繰り返しについて

Pythonでのfor文とwhile文の書き方に慣れる．PythonにはC言語のような普通のfor文はなく，範囲for（foreach）となる．

```py
for i in range(100):
    print(i)

i = 0
while i < 100:
    print(i)
    i += 1
```

## 例外について

例外については簡単に理解しておく程度で，今はOK．

## その他

`if __name__ == '__main__':`について簡単に理解しておく．
