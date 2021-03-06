前編 -> https://squeeze.kibe.la/notes/11371

## overview
後編ではいよいよタイトルのクネビンフレームワークが出てきます。
ただ、正直クネビンフレームワークに関しては実践しているというわけではないので、実際使ってみてどうだったか的な考察は発表しません。

## クネビンフレームワークとは
![](https://successpoint.co.jp/wp/wp-content/uploads/2016/06/cynefin.jpg)

クネビンフレームワークは、1999年にIBM Global Servicesのデイブ・スノーデン(Dave Snowden)らが提唱したもので、**世の中にある問題**を不確実性の高さを元にSimple（単純）、Complicated（煩雑）、 Complex（複雑）、Chaotic（カオス）、Disorder（無秩序）というドメインに分類した意思決定のためのフレームワークです。(上部参照)

### Simple（単純）
問題の因果関係などが誰が見てもはっきり分かるもので、ベストプラクティスを適用して解決を図ります。

対処の順序
1. 知覚
2. 分類
3. 対応

**例:**

知覚 | 分類 | 対応
--- | --- | ---
スマホが動かなくなった | 電池の容量がない | 充電する
蛍光灯がつかなくなった | 蛍光灯が切れている | 蛍光灯を変える

### Complicated（煩雑）
因果関係が複雑ですが、専門家の分析によってグッドプラクティスを得られるような問題。

対処の順序
1. 知覚
2. 分析
3. 対応

**例:**

知覚 | 分析 | 対応
--- | --- | ---
リリース後にサーバー異常が発生した | ログやリリース履歴を分析した結果、デグレードが原因だとわかった | ホットフィックスをリリース
クレジットカードに利用したことのない履歴がある | クレジット会社がデータを分析したところ、不正利用されていたことがわかった | カードを停止し、チャージバック対応

### Complex（複雑）
因果関係が複雑で、さらに分析では解があるかどうかも不明な問題(いわゆるやってみないとわからない問題)
探査をすることで問題の性質を知り対応を考えていかなければいけないため、最終的に実施した対応としてプラクティスが得られることになります。

対処の順序
1. 探査
2. 知覚
3. 対応

**例:**

探査 | 知覚 | 対応
--- | --- | ---
チームのモチベーションor生産性減少の原因を探るため1on1を実施 | 待遇面や人間関係など、多くの潜在的問題が浮上した | 優先順位をつけ、改善していく
自社のSaaSに需要があるか不明なため、MVPを開発し顧客へモニターを依頼 | 改善案や要望が多く上がり、ブラッシュアップすれば需要が見込めそうなことがわかった | 開発していく

### Chaotic（カオス）

因果関係が複雑で分析や調査の方針すら立てるのが困難な問題、または突発的に発生して、すぐに何らかの対応をする必要がある問題。
この場合はまず行動した結果をみることで安定している部分、不安定な部分を理解し、問題を複雑のレベルに落とし込む方法を考えていくことになります。

対処の順序
1. 行動
2. 知覚
3. 対応

**例:**


問題:
未知のウィルス「COVID-19」により世界的なパンデミックが発生。

行動 | 知覚 | 対応
--- | --- | ---
緊急事態宣言の発布 | 日本だとあくまで要請にとどまるため、言うことを聞かない店が出てくる | ニュースや官報で通告、または法改正に踏みこむべきか
マスクや消毒の徹底 | 感染率の大きな低下(副次的にインフルエンザ患者の激減) | 規則の制定や３密回避の共有
助成金や給付金の配布 | 経済の回復が見えたが、一時的なものだった | Gotoなどの計画
オリンピックの開催 | とりあえず2020年は延期 | 2021年は開催するか？その上で色々と取り決めが出てくる

### Disorder（無秩序）

Disorder（無秩序）に関しては体系立った対応方法がないため、、実際には他４種類の問題に対してどう対応すべきかが定義されています。

## クネビンフレームワークのOODAループ適応

という見出しですが、SimpleとComplicatedに関しては答えが存在しているということから、
問題によってはOODAよりPDCAが向いている場合があります。

![](https://i.pinimg.com/originals/85/e4/0c/85e40c52664be6f94568412c3bacb225.png)

## VUCA(ブカ)フレームワークとは

VUCA（ブカ）とは、今我々がいる混沌とした世界をあらわす言葉で、OODAを調べている中でよく目にします。
聴き馴染みはあまりありませんでしたがが、今を「VUCAの時代」「VUCAワールド」と呼んでいる参考文献が多いです。

VUCAは
**V**olatile        =  変動
**U**ncertain    =  不確実
**C**omplex      =  複雑  
**A**mbiguous  =  曖昧
という4つのキーワードの頭文字から取った言葉です

VUCAの意味、VUCAの世界とはどういうものか、そこでどのようにしたらいいかを示してくれるのがVUCAフレームワークとOODAループになります。

ただVUCAについて調べてくると色々と難解な表現が多かったため

```例
熱力学第二法則に基づくと、世界は何もしないと混沌と無秩序 Disorderになっていきます。これはエントロピーが増大していくことを示しています。

エントロピーの増大の段階にしたがい、安定状態のレベル０から曖昧なレベル４そして無秩序のレベル５まで定義できます。

レベル ０：安定　 Stable
レベル １：変動     Volatile
レベル ２：不確実 Uncertain
レベル ３：複雑　 Complex
レベル ４：曖昧　 Ambiguous
レベル ５：無秩序 Disorder
```

クネビンフレームワークはあくまで状況・問題を大きく４つのドメインに分類するフレームワークでしたが、
VUCAフレームワークは **状況**と**状況に対応した行動**が明確に表現されています

また、VUCAフレームワークはクネビンフレームワークと違いOODAループでしか対応ができないため、
OODA思考の重要性が問われます。

![](https://i0.wp.com/iandco.jp/wp/wp-content/uploads/2020/10/VUCA-Framework-1.png?w=1433&ssl=1)

## 参考文献

* [カネビン・フレームワークで問題解決策を見極める](https://successpoint.co.jp/portfolio-view/cynefin)
* [複雑な世界を捉えるためのカネヴィンフレームワーク](https://heart-quake.com/article.php?p=9185)
* [VUCAフレームワーク ：OODAループ臨機応変の適応法](https://iandco.jp/ooda/vuca/)
* [クネビンフレームワークで丸投げアンチパターンの酷さに気づいた](https://www.monokuma12.com/entry/2018/12/18/%E3%82%AF%E3%83%8D%E3%83%93%E3%83%B3%E3%83%95%E3%83%AC%E3%83%BC%E3%83%A0%E3%83%AF%E3%83%BC%E3%82%AF%E3%81%A7%E4%B8%B8%E6%8A%95%E3%81%92%E3%82%A2%E3%83%B3%E3%83%81%E3%83%91%E3%82%BF%E3%83%BC%E3%83%B3)
* [不確実な世の中に立ち向かうためのナレッジマネジメント](https://qiita.com/hsekiya/items/b782edaa9375d90b59e7)
* [｢すぐ決まる組織｣のつくり方 ー OODAマネジメント」](https://www.amazon.co.jp/dp/4866800097/ref=asc_df_48668000972543599/?tag=jpgo-22&creative=9303&creativeASIN=4866800097&linkCode=df0&hvadid=296235215685&hvpos=1o1&hvnetw=g&hvrand=17323909057742258888&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1028853&hvtargid=pla-539970729520&th=1&psc=1)

## 改めて色々調べてみての感想

VUCAの世界といった単語が出てきた時点でコスモを感じ着地点を見失いかけましたが、
俯瞰的に事例とあわせてイメージしてみると混沌とした状況に光明が差す感覚がわかりました。(何から手をつけてよいのかわからない、という状況からの脱却)

私見として、スクラムが有効なクネビンフレームワークのドメインは、 **Complex（複雑）**
が一番効果的だと考えます。
理由としては
* スクラムは検査と適応を行うため、問題への対応が早い
* この問題は先が予測できないため、短いスプリントで探査を行いレトロスペクティブを実施することでプラクティスとなることが多い。

ということが挙げられるためです。
他3つは以下の考えで落ち着きました。
* Simple（単純）- > 手順化してタスクとして処理してしまった方が良い
* Complicated（煩雑） -> 問題によっては有効かもしれない
* Chaotic（カオス）-> スクラム組んでる余裕がないため有効的ではない

クネビンフレームワークを利用することで「スクラムで開発すれば素早くリリースできるんだ！」といった短絡的思考から「今抱えている問題/課題をクネビンフレームワークで分類して考えてみると、手法としてはスクラムが有効だな」という論理的思考で方向性の意思決定が可能になるのは改めて良く出来てるな、と感じた次第。

ちなみにエンジニアリング組織論への招待の広木さんが「CTO/VPoE/TechLead(スペシャリスト)の仕事って一体どう言う役割分担なの？」という問題について、クネビンフレームワークで捉えていました。

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">CTO/VPoE/TechLead(スペシャリスト)の仕事って一体どう言う役割分担なの？みたいなことを聞かれる。<br><br>これはクネビンフレームワークで捉えるとわかりやすい<br><br>CTO は Chaoticな問題 -&gt; Complex <br>VPoE/EMは Complexな問題 -&gt; Complicated<br>TechLeadは Complicatedな問題 -&gt; Simple<br><br>不確実性が減っていく <a href="https://t.co/un1FX3QQ53">pic.twitter.com/un1FX3QQ53</a></p>&mdash; 広木 大地/ エンジニアリング組織論への招待 (@hiroki_daichi) <a href="https://twitter.com/hiroki_daichi/status/1050671531288752130?ref_src=twsrc%5Etfw">October 12, 2018</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

