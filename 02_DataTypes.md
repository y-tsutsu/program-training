# ネイティブデータ型

## Dive Into Python 3

下記のURLの内容を理解する．

[http://diveintopython3-ja.rdy.jp/native-datatypes.html](http://diveintopython3-ja.rdy.jp/native-datatypes.html)

## 概要

ひとまず，次の型について簡単に知っておけばOK．

* bool
* int，float
* string
* list
* tuple
* set
* dict

## bool

比較演算子の結果などがbool型だということを理解しておくといい．

```py
a = 1
x = True if a < 2 else False    # 冗長な書き方
x = a < 2                       # xはbool型
```

またboolではないがPythonはいろいろなものが真・偽として扱われるの知っておくとよい．

```py
x = []
if x:
    print('True')
else:
    print('False')  # こちらが通る
```

## int，float

基本的な数値演算あたりを理解しておけばOK．Pythonの整数型は基本的にサイズを気にする必要がない．
割り算の演算子には注意が必要．`/`の結果はfloatになる．整数同士での`//`は整数．

```py
4 / 2       # 2.0
4 // 2      # 2
5 / 2       # 2.5
5 // 2      # 2
```

またPythonはべき乗も`**`演算子が存在するので覚えておくとよい．

```py
2 ** 10     # 1024
```

## string

文字列操作は必須なのでしっかり覚えておきたい．文字列の詳細はstringの章で行うので，ここでは簡単に理解する程度OK．  
Python3.6からf-strings（フォーマット済み文字列リテラル）が使えるので覚えておくとよい．  
[https://note.nkmk.me/python-f-strings/](https://note.nkmk.me/python-f-strings/)

## list（配列）

文字列同様，リスト操作は必須なので覚えておきたい．追加・削除などの基本操作の他，スライスを覚えておくとよい．スライスは文字列に対しても同様に使えるので便利．  
リテラルは`[]`を使用する．

リストに関する覚えておくとよい操作は以下を参照．  
[https://qiita.com/y-tsutsu/items/aa7e8e809d6ac167d6a1#その他のリストまわりの操作](https://qiita.com/y-tsutsu/items/aa7e8e809d6ac167d6a1#その他のリストまわりの操作)

その他，リスト内包表記も必須．こちらは内包表記の章で詳しく．

## tuple

listとの使い分けをイメージしておくとよい．  
Pythonの場合イミュータブルなlistとの説明も多いが，どちらかというと簡易的な無名構造体のイメージで使うことが多い．（listでも可能だが）異なる方のインスタンスを入れることも．  
下記は複数の値を戻り値で返す例．受け取り側ではアンパック代入を使っている．  
リテラルは`()`を使用する．（というか本質的にはカンマが重要）

```py
def do_something():
    return 'Manatsu', 'Nogisaka', 1         # かっこなしでもtuple

name, group, generation = do_something()    # アンパック代入
```

## set

和集合・積集合・差集合といった集合関連の操作を行う場合に使用する．listだけで自前で処理を書くのではなく，基本的な集合演算を覚えておくと，少し難しめの操作を簡単に効率的な処理で動かすことができる．ちなみに，listとsetの変換は簡単に可能．  
リテラルは`{}`を使用する．

[https://qiita.com/y-tsutsu/items/aa7e8e809d6ac167d6a1#和集合と積集合](https://qiita.com/y-tsutsu/items/aa7e8e809d6ac167d6a1#和集合と積集合)

## dict

listと同様によく使うので覚えておくとよい．実践的なコードを書くときによく使うはず．何でもかんでもlistを使うのではなく，dictを使ったほうが可読性などよくなる場合は使用すべき．  
リテラルは`{}`を使用する．キーと値の区切りに`:`を使用する．
