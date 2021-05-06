# mycat

ファイルを出力するコマンドを作成しなさい．

1. 引数に与えられたファイルの内容を全て標準出力に出力しなさい．  
2. コマンドライン引数に何も与えられなかった場合，標準入力から受け取ったデータを標準出力に出力しなさい．
3. オプションを実装しなさい．
   * `-h`, `--help` オプションが与えられた場合は，ヘルプメッセージを出力しなさい．
   * `-n`, `--numbers` オプションが与えられた場合は，内容を行番号とともに出力しなさい．

## ステップ1

引数に与えられたファイルの内容を全て標準出力に出力しなさい．  

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
file1
file1file1
file1file1file1
$ mycat # このステップでは何も行わない．
```

## ステップ2

コマンドライン引数に何も与えられなかった場合，標準入力から受け取ったデータを標準出力に出力しなさい．

### 入出力例

ステップ1での入出力例の一番最後（コマンドライン引数が与えられなかった場合）以外は同じ出力結果になるようにしてください．

```sh
$ cat file2.txt | mycat
file2file2
file2file2
file2file2
```



## ステップ3

オプションを実装しなさい．

* `-h`, `--help` オプションが与えられた場合は，ヘルプメッセージを出力しなさい．
* `-n`, `--numbers` オプションが与えられた場合は，内容を行番号とともに出力しなさい．

### 入出力例

```sh
$ ./mycat --help # mycat -h も同じ出力結果になるように実装してください．
mycat [OPTIONS] [FILEs...]
OPTIONS
    -h, --help       prints this message.
    -n, --numbers    prints contents with the line numbers.
$ mycat file1.txt file2.txt
    1: file1
    2: file1file1
    3: file1file1file1
    1: file2file2
    2: file2file2
    3: file2file2
```

