# mycat（練習プロジェクト）

ファイルの内容を標準出力に出力するコマンド `mycat` を作成しなさい．

* `main.c`が与えられます．
* 25行目にファイルを開く処理を適切に実装しなさい．
* 実装が終われば，正しく実装できたかを確認しましょう．
* 正しく実装できたことを確認できれば，GitHub に更新内容を push してください．

### 入出力例

```sh
$ ls
file1.txt   file2.txt   file3.txt
$ mycat file1.txt
file1
file1file1
file1file1file1
$ mycat file3.txt file1.txt
file3file3file3
file3file3
file3
file1
file1file1
file1file1file1
```

### 作業の手順

1. プロジェクトをクローンします．
    * `git clone git@github.com/tmdlab2020TestTeam/pre_experiment-????.git` 
    * 具体的な URL はこのページの上部にある「Code」ボタンをクリックして確認してください．
2. クローンされたディレクトリに移動します．
    * `cd pre_experiment-????`
3. kani を有効化します．
    * `kani init`
4. プログラム（`main.c`）を編集します．
5. 動作確認を行いましょう．
    * 動作確認ができれば次のステップに進みましょう．
6. git add, git commit, git pushを行い，変更を GitHub に送信しましょう．
7. それができれば，一つ上のディレクトリに移動し，次の実験1に進んでください．

### 修正の方針

* 25行目に，`file_name`を開く処理（`fopen`）を追加しましょう．

