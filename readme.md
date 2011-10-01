#秀丸エディタから clang-interpreter を使うマクロ。

作成中。


##概要
秀丸エディタで編集中のソースコードをインタプリタ実行します。
プログラムのコンソール出力(printfなど)を秀丸エディタで表示できます。


##実行前
	#include<stdio.h>

	int main(int argc, char*argv[]){
		for(int i=0; i!=4 ; ++i){
			printf("i=%d\n",i);
		}
		return 0;
	}

##実行後
	i=0
	i=1
	i=2
	i=3

##インストール
	下記2ファイルを秀丸マクロのディレクトリへコピーする。
	hm-clang-interpreter.exe
	hm-clang-interpreter.mac


##補足
- インタプリタにはLLVM/Clangを使用しています。
- hm-clang-interpreter.exeのソースコードはコチラ。
https://github.com/ohtorii/clang_examples_visual_studio/tree/master/clang-interpreter
