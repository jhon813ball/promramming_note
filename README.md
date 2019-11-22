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
## Java
### パッケージ管理を考慮したコンパイル
以下のディレクトリ構造を仮定する．
```
  root/
　  ├ bin/
　  └ src/
　    　└ sample/Main.java
```
srcディレクトリで以下のコマンドを入力する．
```
  javac -d ..\bin sample\Main.java
```
エンコーディングの問題がある場合は，次のコマンド．
```
  javac -encoding UTF-8 -d ..\bin sample\Main.java
```
classファイルはbinディレクトリ内に生成され，ディレクトリ構造は次のようになる．
```
  root/
  　├ bin/
　  │　└ sample/Main.class
　  └ src/
　    　└ sample/Main.java
```
ちなみに，Main.javaの枕には以下のように記述されているとする．
```java
  package sample;
```
binディレクトリ内で以下のコマンドにより実行できる．
```
  java sample.Main
```
## C#
### プロジェクトの生成
```
  dotnet new console
```
### 実行
```
  dotnet run
```
## TeX
### Windowsで日本語論文をコンパイルしてPDFに出力する
w32texが導入されていることとする．
```
  uplatex main.tex  // 全体のコンパイル
  uplatex main.tex  // 目次などのコンパイル
  dvipdfmx main.dvi  // PDFに出力
```
