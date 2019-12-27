# ここにある自作コマンドについて
## 導入法
1.コードをダウンロードします。<br>
2.シンボリックリンクをはります。
```
ln -si /[コマンドがあるディレクトリへのパス]/[コマンド名] /usr/local/bin
```
3.スクリプトに権限を付与
```
chmod 777 /[コマンドがあるディレクトリへのパス]/[コマンド名]
```

## atcoder

Atcoderで、全体の提出をターミナルから検索できるようにしたコマンドです。

### 使用法
例えば、ABC123の問題Dを、Python3でACした提出を検索するには以下のように打ちます。

```
atcoder -c abc123 -t d -l Python3 -s AC
```
これを打つことで、標準のWebブラウザで検索結果画面が開かれます。

### オプション-c
**必須コマンドです！！**
検索するコンテストを指定します。<br>
コンテストトップページの「https://atcoder.jp/contests/XXX」のXXXをここのオプションの値に使います。<br>
例えば、ABC001 → abc001<br>
　　　　ARC001 → arc001<br>
　　　　AGC001 → agc001<br>
　　　　大手前プロコン 2019 → otemae2019<br>
    
### オプション-t
検索するコンテスト中の問題を小文字で指定します。<br>
例えば、A問題を指定したいなら、-t a と指定します。

### オプション-l
検索する使用言語を指定します。<br>
例えば、Python3での提出を検索したいなら、-l Python3 と指定します。<br>
使用できる値は以下の通りです。
- bash
- Cgcc
- C++14gcc
- Cclang
- C++14clang
- C#
- Clojure
- CommonLisp
- DDMD
- DLDC
- DGDC
- Fortran
- Go
- Haskell
- Java7
- Java8
- JavaScript
- OCaml
- Pascal
- Perl
- PHP
- Python2
- Python3
- Ruby
- Scala
- Scheme
- Text
- VisualBasic
- C++gcc
- C++clang
- C++clang
- Objective-Cgcc
- Objective-Cclang
- Swift
- Rust
- Sed
- Awk
- Brainfuck
- StandardML
- PyPy2
- PyPy3
- Crystal
- F#
- Unlambda
- Lua
- LuaJIT
- MoonScript
- Ceylon
- Julia
- Octave
- Nim
- TypeScript
- Perl6
- Kotlin
- PHP7
- COBOLFixed
- COBOLFree

### オプション-s
検索するコンテスト中の問題を小文字で指定します。<br>
例えば、ACしたコードを指定したいなら、-s AC と指定します。
