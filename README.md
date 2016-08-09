# バックログプラグイン  

##機能
* ログの改行問題に対応しています。
* ルビをログに表示します。
* キャラ名が重複しないようになっています。
* [font]タグの情報を保存するかしないか選択可能。※1
* mtext / ptext / glink はパラメーター指定でログ表示可能。例：[mtext backlog=true]
* [p][er][ct][cm][s]時にログを纏めて別配列に格納する事で、段落毎の表示・管理が可能です。
* CSSで自由に整形できます。
* ブースタープラグインに対応しやすいるよう、text関係は別ファイルに分けてあります。

※1 [font]タグ情報をログに表示する場合、タグの記載方法が限定されます。  
[Font]～[resetfont] 内には[ruby]以外いれられません。  
[p][cm][er][ct][s]を挟む場合は、再度[font]タグを記述しなければなりません。
  
ダメな例  
[font  size="30"  color="0xffffff"]  
＃ゆうこ  
ゲーム制作に[p]  
興味あるの？
[resetfont]  

OKな例  
＃ゆうこ 
[font  size="30"  color="0xffffff"]  
ゲーム制作に  
[resetfont]  
[p]
[font  size="30"  color="0xffffff"]  
興味あるの？ 
[resetfont]
