
# NPB_Pennant_race
Japanese professional baseball team's pennant race code by python


# 【野球プログラムの作成】
## y-1:超基本的な野球プログラムの作成
### ■マイルストーン
1. コンソールにプレイボールと表示する

2. 1回表・1回裏のイニングを終わらせる。アウトやヒットの条件はランダムで構わないが、得点が入る可能性はあるようにコーディングすること。

3. 9回裏まで試合を進め、ゲームセットの表示とともに、チームスコアも表示すること

要件は以下のとおりです。
- コンソールでのメッセージ表示で完結するプログラム。
- 代打、代走、ピッチャー交代といった要素はなし。スタメン9人で行うこととする。
- 打席の結果は、ヒットとアウトの2択とする。ヒットはシングルヒットのみ。
- それぞれの回終了時のスコア情報、ゲームセット時の情報も全てコマンドラインに出力する。


## y-2:リファクタリング
### ■宿題のマイルストーン
1. y-1のソースコードに以下のリファクタリングを行うこと
#1.senkou,koukouメソッド内のwhile部分を抜き出して、1つのメソッドにまとめる
#2.1回表～9回裏までのsenkou,koukouメソッドのコールをループ文で実現する


## y-3:要件追加
### y-2で作成したプログラムに対して、以下要件を追加してください。
■詳細要件
- 2ベースヒット、3ベースヒット、ホームランが発生するようにする。
- 5点以上取られたら、ピッチャーを交代する。


## y-4:要件追加
### y-3で作成したプログラムに対して、以下要件を追加してください。
■詳細要件
- 実際のセリーグのチーム名に応じて、全チームをペナントレースさせて優勝チームを決定する処理を書く。
- マジックの概念はなし。140試合終了時点で、最も「勝率」が高いチームを優勝チームと定義する。
- 優勝決定時には、順位表を出力する。順位表の出力カラムは「チーム名」「勝利数」「負け数」「引き分け数」「勝率」「ゲーム差」の6つ。
- 引き分けの定義は「12回終了時に同点」とする。
- 勝率が同じ場合は、勝ち数の多い方とする。それでも同じ場合は1,2位のチーム同士で優勝決定戦する仕様とする。
- 対戦カードは全チームと28戦することとする。対戦順序は任意。


## y-5:要件追加
### y-4で作成したプログラムに対して、以下要件を追加してください。
■詳細要件
- パリーグでもペナントレースを実施する。ペナント実施上の条件は、5-4時点でのセリーグの仕様と全く同じにする。
- 年間140試合中18試合を交流戦とし、セ・パ両方のチームがお互いに3戦*6チーム分対戦する。それに際し、交流戦での優勝チームも決定する。
