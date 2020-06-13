# Prologue 02 「理由」のコラム

## 「ラプラス変換」と「『空論の魔女』の『マギ時空論』」

### ラプラス変換

百由様がストーリー中で語っている『千代御代』の『マギ時空論』について語ってますが
（一応<a href="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/CharacterProfile.md#%E5%8D%83%E4%BB%A3-%E5%BE%A1%E4%BB%A3%E3%81%9B%E3%82%93%E3%81%A0%E3%81%84-%E3%81%BF%E3%82%88">キャラ紹介</a>中でも軽く触れています）、
そこで出てくる「ラプラス変換」について解説をまず。　＊１）

ラプラス変換は、「制御工学」という分野で一番最初に出てくる式変換（写像）です。

例えば、

式１）　<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_1.jpg" height="50px">

という時間tに関する式があったとします(R、L、Cは定数)。

微分と積分が入り混じって、文系の方に見せたら「目をそらしたくなる」らしいです。（実際に訊きました）

これをラプラス演算子s<span style="color:#ff0000;">(=σ+jω)</span>というもの（薄い字のとこは気にしなくていいですよ～）を使って、

式２）
<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_2.jpg" height="50px">
<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_3.jpg" height="50px">

という時間変数tから、変数sへの関数変換を行うことができます。

上の式１）は、ラプラス演算子sに関する

式３）
<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_4.jpg" height="50px">

というという、微分も積分も出てこない（そこそこ簡単な）式になります。

制御工学では、時間tでなく、このsの世界でいろいろ難しいことを考えます。

例えば、CHARMでいうなら単なるモータのON/OFFで変形を行なってしまうと、毎回ガッチャンガッチャン急な変形になってすぐにギアが傷んでしまいます。
おそらく。

なので、変形の際は、急にモータを動かすのではなく、徐々に回転速度を上げ、変形完了前には徐々に回転速度を落とすことで、ギアにかかる負担を減らし、ギアが欠けたり、破損を防ぎます。またこれはモータにかかる負荷を減らすことにもつながります。

このモータの「制御」を扱うのが「制御工学」という分野（モータに限りませんが）で、
百由様が「周波数の世界」と言っていたのも、周波数の特性を考えたりするのにもこのラプラシアンsの世界を使うためです。

つまり、式２）にコメントを書き込むなら、

<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_5.jpg" height="100px">

という感じでしょうか。

そしてもちろん、sの世界に行きっぱなしでなく、時間tの世界にも帰ってこれます。

実は、式１）はRLC回路という電気回路の入力電圧の式で、Rは抵抗、Lはコイル、Cはコンデンサをそれぞれ表しています。

i(t)は時間tに回路に流れる電流です。

ここで、この回路の入力電圧として時間0から突然大きさ１の電圧を加えます（要はスイッチオンです）。

この操作をラプラス変換すると、F(s) = 1/s で、式３）は、

<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_6.jpg" height="50px">

となり、これをi(s)に関する式に変形すると、

<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_7.jpg" height="50px">

さらに定数R、L、Cを１とすると、

<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_8.jpg" height="50px">

という非常に単純な式になります。

そして、これを逆ラプラス変換（sの世界から時間tの世界へ帰ってくる操作）を行うと、

<img src="https://github.com/kaede3pic/secondary/blob/master/AssualtLilyMECHANICS/image_jpg/00_02/siki_9.jpg" height="50px">

と、時間tに回路に流れる電流の式が微分も積分も使わない形で表現できてしまうのです。

<hr>

＊１）　これがどれだけメジャーな用語かは、それを知っちゃてる私側にはわからないので。

カードゲームでいうと、「マリガン」という用語を知っているかどうかという感じです。

（初めてWSの大会に参加したとき、「マリガン」ってまず言われて、「？？？」となって対戦のお相手に教えてもらった思い出）

### 『空論の魔女』の『マギ時空論』

さて、上で解説した「ラプラス変換」のエッセンスを取り出したのがストーリー中での百由様の解説です。

時間tの世界では複雑なことも、sの世界に飛ばすと簡単に説明できてしまうし、sの世界からtの世界に帰ってくることもできる。

『マギ時空論』ではこのtがマギがエネルギーとして存在する「物理世界」、sがマギが情報体として存在する「情報の世界」（=『マギ時空』）と考えます。

物理世界で不可思議な現象も、情報の世界から見たら実は単純なことで、そこで結論を出し、また物理世界に帰ってくれば、情報世界で起きた結果が物理世界で発現してしまっている。

これが『空論の魔女』の『マギ時空論』です。

プロローグ02では、二川三夜こと、みーちゃんが『縮地』に関してこの説明をしていますね。

『マギ時空論』における『マギ時空』というのは、この物理世界に重なって無数に存在しています。

『鷹の目』の世界だったり、『縮地』の世界だったり、さまざまな『マギ時空』が存在しています。

リリィたちはそれぞれが持つマギの性質に応じて、アクセスできる『マギ時空』が決まっています。

これは変更の利かないラジオの周波数みたいなものだと思ってください。要は、自分が持ってる周波数（固定）に一番近い番組しか聴けないようなものです。

（サブスキルに関しては、持っているマギの波形が他のチャンネルにもアクセスできるような複雑な形をしていると解釈します）

## 千代御代（少女）改め「二川三夜」の戦い方
### 『縮地』の欠点とその対処法に関する一考察　千代御代 著 より抜粋

## GEHENA内における千代御代の立ち位置（『リジェネレーター』研究を例に）

