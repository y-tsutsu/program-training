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

良記事：  
[https://qiita.com/KoyanagiHitoshi/items/318d4b8ef3b4e5b87390](https://qiita.com/KoyanagiHitoshi/items/318d4b8ef3b4e5b87390)

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

※ただしvi（Vim）についてはメインエディタにしなくても基本操作は覚えておくとよい．ボード上のファイルをssh経由で編集するときなどに必要．

良記事：  
[https://qiita.com/KoyanagiHitoshi/items/82ef910432552d0a4553](https://qiita.com/KoyanagiHitoshi/items/82ef910432552d0a4553)

## Gitクライアント

Gitコマンドを直接使うなり，エディタのプラグインを使うなり，何か別のGUIクライアントを使うなり，自分に合った環境を用意する．ぼくはGitKraken使ってる．  
ひとまずは新人研修で行った操作が理解できて，実際に操作できればOK.

新人研修：  
[https://qiita.com/y-tsutsu/items/2ba96b16b220fb5913be](https://qiita.com/y-tsutsu/items/2ba96b16b220fb5913be)  
[https://qiita.com/y-tsutsu/items/98fc75b8814c99619cf4](https://qiita.com/y-tsutsu/items/98fc75b8814c99619cf4)

## その他参考URL：

[https://qiita.com/y-tsutsu/items/61dd0bc60838c10b963b](https://qiita.com/y-tsutsu/items/61dd0bc60838c10b963b)  
[https://github.com/y-tsutsu/dotfiles](https://github.com/y-tsutsu/dotfiles)

# プログラムのコンパイル，実行環境（C/C++，Python）

## C/C++

とりあえずビルドできる環境が入っていればOK．  
Ubuntu，Debianなら下記でインストール．

```console
$ sudo apt install build-essential
```

## Python

Linuxならはじめから入っているはず．下記コマンドでバージョンが表示されればOK．  
※Pythonはバージョンが2系と3系に分かれるが，今は3系が主流なので3系の環境を整える．

```console
$ python3 --version
Python 3.7.3
```

ぼくはpyenvでインストールしている

[https://qiita.com/SUZUKI_Masaya/items/7ba3fef9eb7c9603762a](https://qiita.com/SUZUKI_Masaya/items/7ba3fef9eb7c9603762a)  
[https://karaage.hatenadiary.jp/entry/2015/11/26/073000](https://karaage.hatenadiary.jp/entry/2015/11/26/073000)（proxy設定）

# その他Linuxに慣れる

徐々に読むでOK．いきなり全てを覚えていく必要はない．

参考URL

* [https://www.garunimo.com/program/linux/linux5.php](https://www.garunimo.com/program/linux/linux5.php)  
ここの項目8までは早めに読んでおくことがおすすめ
* [https://eng-entrance.com/category/linux](https://eng-entrance.com/category/linux)  
パーミッション，viなどはすぐに必要となってくるので読んでおくとよい

参考書籍（私物ですが会社にあります）

* [http://msyksphinz.hatenablog.com/entry/2018/03/02/040000](http://msyksphinz.hatenablog.com/entry/2018/03/02/040000)  
LinuxだけでなOSについての知識が自分で書ける簡単なコードで身に付く
* [https://system-admin-girl.com](https://system-admin-girl.com)  
みんとちゃんかわいい（内容も実践的）
