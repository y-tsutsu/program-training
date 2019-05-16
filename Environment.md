# Linux環境のインストール

## ディストリビューション

TS部ではUbuntu，Debianあたりが多い．ぼくはDebian．

[https://eng-entrance.com/linux_beginner_distribution](https://eng-entrance.com/linux_beginner_distribution)

## 仮想マシン

TS部ではVirtualBox，VMwareあたりが多い．ぼくはVMware．

[https://eng-entrance.com/vm-list](https://eng-entrance.com/vm-list)

## 仮想マシンにLinuxをインストール

使用するLinuxディストリビューションや仮想マシンに合わせて，参考記事を探してインストールする．

参考URL

* [http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToUbuntu.html](http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToUbuntu.html)
* [https://eng-entrance.com/category/linux](https://eng-entrance.com/category/linux)


# Linuxに開発環境を入れる

開発に必要なツール類をインストールする．各種ツールの設定を自分オリジナルでつくりこむとよい．

* ターミナル
* シェル
* テキストエディタ
* Gitクライアント

## ターミナル

環境に標準で入っているものでも別途インストールするでも使いやすければOK．透過させるとカッコいい．ぼくはTerminatorを使っているけど，それほど大きな意味はない．

### tmux

ターミナルマルチプレクサとか呼ばれているターミナルの仮想化とかするやつ．有名なので調べてよければ使ってみるといい．ぼくは使ってる．

## シェル

標準のbashやzsh，fishとか．補完機能や見た目でお気に入りの環境を作ればいい．ぼくはzsh使ってる．

## テキストエディタ

プログラミング用のエディタを，まずは一つ用意する．機能やカスタマイズ性，見た目などでお気に入りを見つけるといい．

TS部だと次のうち，とくに上位3つを使っている人が多い．ぼくはVSCode使ってる．

* Vim
* Emacs
* Visual Studio Code（VSCode）
* Atom
* Sublime Text

これについては人にお勧めされるだけでなく，とにかく自分で使ってみてお気に入りのものを見つけてほしい．

## Gitクライアント

Gitコマンドを直接使うなり，エディタのプラグインを使うなり，何か別のGUIクライアントを使うなり，自分に合った環境を用意する．ぼくはGitKraken使ってる．  
ひとまずは新人研修で行った操作が理解できて，実際に操作できればOK.

新人研修：  
[https://qiita.com/y-tsutsu/items/2ba96b16b220fb5913be](https://qiita.com/y-tsutsu/items/2ba96b16b220fb5913be)

## その他参考URL：

[https://qiita.com/y-tsutsu/items/61dd0bc60838c10b963b](https://qiita.com/y-tsutsu/items/61dd0bc60838c10b963b)

# プログラムのコンパイル，実行環境（C/C++，Python）

## C/C++

とりあえずビルドできる環境が入っていればOK．  
Ubuntu，Debianなら下記でインストール．

```console
$ sudo apt install build-essential
```

## Python

Linuxならはじめから入っているはず．下記コマンドでバージョンが表示されればOK．

```console
$ python3 --version
```

ぼくはpyenvでインストールしている．

[https://qiita.com/SUZUKI_Masaya/items/7ba3fef9eb7c9603762a](https://qiita.com/SUZUKI_Masaya/items/7ba3fef9eb7c9603762a)

# その他Linuxに慣れる

徐々に読むでOK．いきなり全てを覚えていく必要はない．

参考URL

* [https://www.garunimo.com/program/linux/linux5.php](https://www.garunimo.com/program/linux/linux5.php)
* [https://eng-entrance.com/category/linux](https://eng-entrance.com/category/linux)

参考書籍（私物ですが会社にあります）

* [http://msyksphinz.hatenablog.com/entry/2018/03/02/040000](http://msyksphinz.hatenablog.com/entry/2018/03/02/040000)
* [https://system-admin-girl.com](https://system-admin-girl.com)
