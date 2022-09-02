# typing

Typing.js
javascript で簡単にタイピングゲームのようなものを実現するライブラリ
ie9, ie10, chrome, firefox での動作を確認しました

Typing.register(string)
string に問題文を指定する
使用できる文字はひらがな,一部記号

Typing.answer(char)
1 文字回答する正解していた場合は true,間違っていた場合は false を返す

Typing.getQuestion()
変換された文字列を返す

Typing.getOriginalQuestion()
register で設定された文字列を返す

Typing.getAbsoluteAnswered()
今まで何文字正解したかを返す(打キー数ではなく文字数, 「きゃ」なら 2 文字)

Typing.isFinish()
設定した問題を回答し終えている場合は true を返す

Typing.getFault()
answer で間違えていた回数を返す

Typing.getNextKey()
次の正しいキー入力を返す

使い方
var temp = new Typing();
temp.register("もんだい");
temp.answer("m");

詳細は sample.html 参照
