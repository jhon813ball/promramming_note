# プログラミングノート
プログラミングに関する備忘録．
## Github
### ファイルの変更を更新する
```
  git add -u
  git commit -m “[comment]”
  git push [remote repository PATH]
```
## Windowsコマンドプロンプト
### 文字コードをUTF-8に変換する
```
chcp65001
```
## C言語
### 単一ファイルのコンパイルと実行
```
gcc main.c -o main
```
'main'という名前の実行ファイルが生成されるので，以下のコマンドで実行する．
```
.\main
```
Windousの場合は.exeファイルが生成されるため，以下のコマンドでも可．
```
main.exe
```
### 複数ファイルのコンパイル
```
gcc sub1.c sub2.c -o main
```
## C++
### 単一ファイルのコンパイルと実行
```
g++ main.cpp -o main
```
'main'という名前の実行ファイルが生成されるので，以下のコマンドで実行する．
```
.\main
```
Windousの場合は.exeファイルが生成されるため，以下のコマンドでも可．
```
main.exe
```
### 複数ファイルのコンパイル
```
g++ sub1.cpp sub2.cpp -o main
```
