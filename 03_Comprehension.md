# 内包表記

## Dive Into Python 3

下記のURLの内容を理解する．

[http://diveintopython3-ja.rdy.jp/comprehensions.html](http://diveintopython3-ja.rdy.jp/comprehensions.html)

## 概要

Pythonのだいご味の一つなのでしっかり覚えておきたい．  
あとなぜか前半にファイル操作について書かれているが，これも重要なのでついでに見ておく．

## ファイル操作

パスからディレクトリ名・ファイル名・拡張子を抜き出す方法や，ディレクトリ内のファイルを一覧する操作ができればOK．`glob`の他にも再帰的にディレクトリを渡り歩ける`os.walk`も覚えておくと便利．

また`pathlib`という新しいモジュールができていて，`os.path`よりもいいらしい．ぼくはまだ使ってない．

[https://qiita.com/tag1216/items/29bf3b9c3c4b563ff0fe#pathlibは普及しているのか](https://qiita.com/tag1216/items/29bf3b9c3c4b563ff0fe#pathlibは普及しているのか)

## リスト内包表記

選択（SQLならwhere），射影（SQLならselect）などを扱うことができます．これを覚えるとコレクションのデータ操作が簡潔に書けるので，ぜひマスターしたい．

### 選択
```py
[x for x in range(10) if x % 2 == 0]    # 偶数を選択
# [0, 2, 4, 6, 8]
```

### 射影
```py
[x * 2 for x in range(10)]  # 各要素を2倍に
# [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
```

### ちょっとした応用

https://qiita.com/y-tsutsu/items/aa7e8e809d6ac167d6a1#リスト内包表記を使ったあれこれ

## その他の内包表記

リスト以外にも内包評価が使えるので覚えておくとよい．とくに無理にリストで扱うよりも辞書のほうが可読性がよさそうな場合は，辞書内包表記を使っていきたい．

* 辞書（dict）内包表記
* 集合（set）内包表記
* ジェネレータ内包表記
