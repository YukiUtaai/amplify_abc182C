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

オール9のケース（handmade_00.txt）で間違ってしまっているので、計算時間を増やせば改善するか確認します。
→改善しました。

```shell
all_00.txt Amplify結果 = 0 正解 = 0
all_01.txt Amplify結果 = -1 正解 = -1
all_02.txt Amplify結果 = 1 正解 = 1
all_03.txt Amplify結果 = -1 正解 = -1
all_04.txt Amplify結果 = 2 正解 = 2
all_05.txt Amplify結果 = -1 正解 = -1
all_06.txt Amplify結果 = 1 正解 = 1
all_07.txt Amplify結果 = 0 正解 = 0
all_08.txt Amplify結果 = 0 正解 = 0
all_09.txt Amplify結果 = 1 正解 = 1
all_10.txt Amplify結果 = 1 正解 = 1
all_11.txt Amplify結果 = -1 正解 = -1
all_12.txt Amplify結果 = 2 正解 = 2
all_13.txt Amplify結果 = 1 正解 = 1
all_14.txt Amplify結果 = 1 正解 = 1
all_15.txt Amplify結果 = 0 正解 = 0
all_16.txt Amplify結果 = 0 正解 = 0
handmade_00.txt Amplify結果 = 0 正解 = 0
random_00.txt Amplify結果 = 1 正解 = 1
random_01.txt Amplify結果 = -1 正解 = -1
random_02.txt Amplify結果 = 1 正解 = 1
random_03.txt Amplify結果 = 0 正解 = 0
random_04.txt Amplify結果 = 0 正解 = 0
sample_01.txt Amplify結果 = 1 正解 = 1
sample_02.txt Amplify結果 = 0 正解 = 0
sample_03.txt Amplify結果 = 1 正解 = 1
sample_04.txt Amplify結果 = -1 正解 = -1
```

## 考え方

各桁の値を係数とするlen(n)のqubitと係数-3の3*18のqubitで和が0

(equal_to関数をあまり信じていないので、2乗して定数をかけてペナルティを表現)

消す桁は少ない方が良いので、len(n)のqubitにマイナスの係数をかけてΣすればよいです。

## 使用したアニーリングマシン

Fixstars Amplify AE

https://amplify.fixstars.com/

## 使用した問題

https://atcoder.jp/contests/abc182/tasks/abc182_c
