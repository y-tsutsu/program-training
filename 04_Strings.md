# 文字列

## Dive Into Python 3

下記のURLの内容を理解する．

[http://diveintopython3-ja.rdy.jp/strings.html](http://diveintopython3-ja.rdy.jp/strings.html)

## 概要

文字列操作は製品アプリの開発から書き捨てのコードまで，幅広く使える潰しのきく知識なので，ぜひしっかりと習得しておきたい．

## Unicode

前半にUnicodeについて書かれているが，現状は簡単に読んでおく程度でOK．ちなみにPython3では文字列はデフォルトでUnicode文字列で扱われます．（`u'spam'`という表現はPython2なので古いです．）

## 基本操作

文字列の基本的な操作はlistと同じように操作できる．

```py
s = 'こんにちは，世界'
l = len(s)          # 文字列の長さを取得
print(s[0])         # こ 配列と同じように[n]でn番目の文字にアクセスできる
print(s + '!!')     # 文字列の連結もリストと同様にできる
```

## 文字列のフォーマット

文字列のフォーマットはとれもよく使うので，しっかりと覚えておきたい．またPython3.6以上では，フォーマット済み文字列リテラル（f-string）が便利なので，覚えておくとよい．（Dive Into Python ｎにはf-stringについては書かれていない．）

```py
a = 'one'
b = 1
print('{0}: {1}'.format(a, b))  # one: 1
print(f'{a}: {b}')              # one: 1（上と同じ）
print(f'{a}: {b:05}')           # one: 00001（桁数指定なども可能）
```

## その他の文字列メソッド

大文字・小文字への変換や，区切り文字での分割などは頻繁に使うので覚えておくとよい．また部分文字列の取得などはリストと同様にスライスを使用すると便利．またスライスを利用すると文字列の反転なども簡単に可能．

```py
from string import ascii_lowercase
print(ascii_lowercase)          # abcdefghijklmnopqrstuvwxyz
print(ascii_lowercase[::-1])    # zyxwvutsrqponmlkjihgfedcba
```

## 文字列とバイト列

少し難しい内容だが，テキストファイルの読み書きや，通信などひ必要な知識なので理解しておきたい．とりあえずはエンコーディングを指定してのエンコードとでコードが理解できていればOK．文字列とバイト列は混ぜて使うことができないので，型をしっかりと意識すること．

```py
x = 'Hello, World!'
print(x, type(x))       # Hello, World! <class 'str'>
b = x.encode('utf-8')
print(b, type(b))       # b'Hello, World!' <class 'bytes'>
s = b.decode('utf-8')
print(s, type(s))       # Hello, World! <class 'str'>
```

# 正規表現

文字列といえば正規表現が重要なので，正規表現についても簡単に理解とPythonでの使い方を把握しておきたい．Pythonでは`re`モジュールを使用する．  
基本は下記のURLを理解しておけばOK．  
また，正規表現は自分なりのチートシートを何らか持っておくとよい．（ぼくはテキストエディタの検索機能で正規表現のパターンが確認できる．）

[http://diveintopython3-ja.rdy.jp/regular-expressions.html](http://diveintopython3-ja.rdy.jp/regular-expressions.html)
