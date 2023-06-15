---
title: "最近読んだ論文"
---

### Automated Program Repair in the Era of Large Pre-trained Language Models
LLM系APRツールとSOTAなAPRの比較．(ICSE 2023)
* LLMのパラメータ数が多い方が結果良い
* SOTAなAPRでは解決が困難な問題も，自然言語とプログラムコードを学習したLLMなら解決できる
* LLMの学習データの中に評価データが入ってしまっている可能性もあるが，ヒューマンパッチと異なる修正案も提案できることから，そのまま取ってきてるわけじゃなさそう
* 生成したパッチのエントロピーが，plausibleかcorrectか判断する指標になるよ
  * 既存の研究と一緒
* 修正対象のソースコード長い方がうまくいくよ
  * 自動修正適合性の論文で主張されていた内容と一緒
* SOTAなAPRの技術と掛け合わせるとLLM系APRの精度上げられるよ

* *所感*
  * Codexが最強すぎた
  * ChatGPTってちゃんと先頭から文章作ってたんや，という驚き
  * 自然言語系の学習を進めないといけないなという思い

### An Analysis of the Automatic Bug Fixing Performance of ChatGPT

アーカイブ論文．

最近流行りのLLM系APRツール．
ChatGPTを使ったAPRがどの程度バグ修正できるか調査してた．
Deepl系の手法より精度いいらしい．さすがChatGPT．すごい．
修正してたのがQuixBugsに対してのみなので，学習データから正解データ引っ張ってるだけにも見えた．気もした．

ChatGPTってプログラム組むための機構が入ってるって聞いてたけど，どうなんやろう．
