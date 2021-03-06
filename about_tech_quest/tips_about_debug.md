# デバッグのコツ

以下の1~3まではあまり時間を掛けずに簡単に確認する。

パッと見で問題がなさそうなら、 **「1つ上の行」が原因のときも多い** ので、そちらで同様に1~3の手順を確認する。

1. まずエラーが出ている行、もしくはうまくいっていない部分のプログラムをチェックする。
1. そこで「打ち間違い」がないかをチェックする。
1. 参考にしたプログラムとの「写し間違い」がないかをチェックする。
1. そこに問題がなければ、エラーが出ている行より上を `var_dump();` と `die();` を使い、 **"プログラムを止めながら"、"変数の中身"を一行ずつチェック** していく。

- 原因がひと目でわからなくても、いろいろプログラムを書き換えては実行を繰り返し、どこが原因かを突き止める。
- エラーが出た箇所に似ているプログラムがあれば、すでにうまくいっているプログラムと「何が違うのか」をよく見比べてみる。
