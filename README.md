# amplify_abc182C

## 実行方法

1. プログラムと同じ階層にAmplifyのアクセストークンを記載した`tokenfile.txt`を作成する。

（もしくは直接`client.token`にアクセストークンを入力する）

2. テストケースをダウンロードする。
https://www.dropbox.com/sh/nx3tnilzqz7df8a/AAB330_m_UmEFwd07geuDtTga/ABC182/C?dl=0&subfolder_nav_tracking=1

3. テストケースを置いたフォルダを指定する
```shell
folder = "ABC182C/"
```        
        
4. プログラムをを実行する

現在Amplifyが重くて計算に時間がかかっていますので、後日結果を貼ります。
多分大丈夫なはずです。

```shell

```

## 考え方

各桁の値×定数（強い制約をかけるため）を係数とするlen(n)のqubitと係数-3の3*18のqubitで和が0
消す桁は少ない方が良いので、len(n)のqubitにマイナスの係数をかけてΣすればよいです。

## 使用したアニーリングマシン

Fixstars Amplify AE

https://amplify.fixstars.com/

## 使用した問題

https://atcoder.jp/contests/abc182/tasks/abc182_c
