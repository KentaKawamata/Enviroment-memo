# Ubuntu環境構築

Ubuntu環境構築の備忘録.

# 設定

**キーボード設定**

JIS規格にキーボード設定を変更

```
$ sudo dpkg-reconfigure keyboard-configuration
```



**言語設定**

```
$ sudo apt-get install ibus-mozc
$ killall ibus-daemon
$ ibus-daemon -d -x &
```

システム設定->テキスト入力->使用する入力ソースに「日本語(Mozc)」を追加
システム設定->言語サポート->「日本語」を一番上にする

**suのパスワード設定**

```
$ sudo passwd root
```

**amazonの削除**

```
$ sudo apt remove unity-webapps-common
```

**サスペンドとロックの無効化**

システム設定->電源->サスペンドしない
システム設定->画面の明るさとロック->ロックしない

**起動時のパスワード要求無効化**

システム設定->ユーザーアカウント->自動ログインオン

# インストールするもの



**vim**

```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install vim
```

**Git**

```
$ sudo apt-get git
```

**vivaldi**

サイトからvivaldi-snapshotをダウンロード,インストール

![vivaldi-snapshot](https://jp.vivaldi.net/category/snapshot/)
