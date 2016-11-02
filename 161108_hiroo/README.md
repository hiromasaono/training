# AJACSこまち　生物学的解釈をするための遺伝子発現DB・解析ツールの使い方

大学共同利用機関法人 情報・システム研究機構  
データサイエンス共同利用基盤施設  
ライフサイエンス統合データベースセンター    
[小野 浩雅](https://sites.google.com/a/dbcls.rois.ac.jp/hono/)  
hono@dbcls.rois.ac.jp  
2016年8月8日(月)
AJACSこまち@秋田県産業技術センター 高度技術研究館 2階ミーティングルーム  

----

これは統合データベース講習会 AJACS前橋「生物学的解釈をするための遺伝子発現DB・解析ツールの使い方」の講習資料です。  
この内容の続編として、AJACS御茶ノ水(2015年5月)における[応用・実践編](http://doi.org/10.7875/ajacs.2015.007) がありますので、こちらもあわせてご活用ください。  
講習会全体のプログラムは[こちら](http://events.biosciencedbc.jp/training/ajacs61)です。  

----

## 概要

本講習は、だれでも自由に使うことができる公共データベースやウェブツールを活用して、研究のさまざまな場面で調べることの多い個々の遺伝子発現データを簡単に調べるための方法と基礎知識について学びます。  
また、自ら行なった大規模発現解析の(あるいは公共データベースから取得・解析した)結果として得られた数百〜数千におよぶ遺伝子セットについて、生物学的な解釈をする方法とその結果の考察を実践します。  

----

## 講習の流れ
今回の講習では、コンピュータを使って以下の内容について説明します。

- 研究現場で頻繁に使われるデータベースやツールを知る
    - 統合TV
- 個々の遺伝子の発現プロファイルを調べる
    - RefEx
        - 【実習1】RefExを使って、組織特異的遺伝子を検索する
- 数十～数千の遺伝子群の生物学的解釈
    - DAVID
        - 【実習2】DAVIDを用いて、発現データの結果を生物学的に解釈する
- 【実習3】これまで学んだことを踏まえて、発現データの結果を生物学的に解釈する

----

#### 講習に際しての注意とお願い
- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます。
    - 資料を見ながら自力で進められそうな方はどんどん先に、そうでない方は講師と一緒にすすめていきましょう。
    - サイトの反応が悪い時はタイミングをずらして実行してみてください。
    - 反応が無いからと言って何度もクリックするとますます繋がらなくなってしまいます。おおらかな気持ちで臨みましょう。
- わからないことがあったら挙手にてスタッフにお知らせください。
    - 遠慮は無用です(そのための講習会です!)。おいてけぼりは楽しくありません。

----

#### 受講前アンケートにご協力いただき、ありがとうございます (回答数 24)

|統合TVを知っていますか?|人数|割合|
|:--|--:|:--:|
|知らない|14 名|58 %|
|聞いたことがある|0 名|0 %|
|知っている|3 名|13 %|
|使ったことがある|2 名|8 %|
|使っている|1 名|4 %|
|回答なし|4 名|17 %|
---
|自分で実験して得た、数十〜数千の遺伝子からなる<br>「遺伝子リスト」(例: 発現差のあった遺伝子など) を持っていますか?|人数|割合|
|:--|--:|:--:|
|これから実験をする・したい|2 名|8 %|
|公共データを活用する・したい|7 名|29 %|
|既に持っている|4 名|17 %|
|大規模発現解析の予定はない|5 名|21 %|
|回答なし|6 名|25 %|
---

## 研究現場で頻繁に使われるデータベースやツールを知る
### [統合TV](http://togotv.dbcls.jp/ja/)
- 生命科学分野の有用なデータベースやツールの使い方を動画で紹介するウェブサイト
    - http://togotv.dbcls.jp/ja/
    - ![統合TVトップページ](https://i.gyazo.com/dddde578caafeb260abc939bab68adfb.png)

    - YouTube版もあります　http://www.youtube.com/user/togotv/
    - ![統合TV YouTube支店](http://i.gyazo.com/1dce80b0a05a7de372415fa0b42a079c.png)
    - YouTubeのチャンネル登録をすると更新情報がメールで届きます。

- ウェブサイトへのアクセスの仕方から結果の解釈まで、操作の一挙手一投足がわかります。
    - 1100本を超える動画が公開されており、YouTube版だけで のべ 650,000回以上 再生されています。(2016年7月末現在)
    - ![https://gyazo.com/10a9b6f46b82b8442c1dbe61ca521fce](http://i.gyazo.com/10a9b6f46b82b8442c1dbe61ca521fce.png)

- 講義・講習などの参考資料や後輩指導の教材として利用できます。
    - 本講習中、本家サイトが繋がらない時は、統合TVを見ればおおよその内容がわかるようになっています。

    - 今回の講習に関連するデータベースやウェブツールは、[統合TV の「発現解析」タグ](http://togotv.dbcls.jp/ja/tags.html?tag=発現解析)から検索できます。  

- 統合TVに掲載されているコンテンツについてご引用いただく際に、恒久的な URL として [DOI](https://ja.wikipedia.org/wiki/デジタルオブジェクト識別子) (Digital Object Identifier) を使用することができます。

- 2014年8月以降に開催された過去の講習会の資料・テキストと動画が「[AJACS講習会資料](http://togotv.dbcls.jp/ja/ajacs_text.html)」で閲覧できるようになり、受講生の復習のみならず、初学者の学習教材としてご活用いただけます。

- お探しの動画が見つからない or 統合TV未掲載の場合は、[統合TV番組リクエストフォーム](http://togotv.dbcls.jp/ja/contact.html)へどうぞ!!

- 統合TVを作ってみたい方、募集中です。(オンラインでの作成環境を整備しており、遠隔地でもOKです)

----

#### 習熟度ややりたいこと別にご参考ください
- 本講習内容をスムーズに理解するために押さえておくとよい基礎知識
    - [「塩基配列解析のためのデータベース・ウェブツール」(2015年9月AJACS伊予)](http://togotv.dbcls.jp/ja/ajacs2015033.html)

- 遺伝子発現データを公共DBで検索・取得・解析する方法について
    - [「遺伝子発現DB・ウェブツールの使い方 応用・実践編」(2015年5月AJACS御茶ノ水)](http://togotv.dbcls.jp/ja/ajacs2015007.html)

- 非モデル生物のデータをモデル生物のデータに見立てるためのID対応表づくりについて
    - [「コマンドラインで遺伝子配列を解析する」（2012年7月）](http://motdb.dbcls.jp/?AJACS32%2Fbono)

- 次世代シーケンス(NGS)データの解析について
    - [「次世代シーケンサー（NGS）と関連するデータベース・ツール」(2015年9月AJACS伊予)](http://togotv.dbcls.jp/ja/ajacs2015031.html)
    - [「次世代シーケンサー(NGS)データから遺伝子発現を見るためのホップ&ステップ」(2015年9月AJACS伊予)](http://togotv.dbcls.jp/ja/ajacs2015030.html)

- NGS解析について、さらにもっと基礎から応用までを深く学びたい方向け (それぞれ約50時間程度)
    - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース(2014年8月)」のYouTubeリスト](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
    - [「バイオインフォマティクス人材育成カリキュラム 次世代シークエンサ(NGS)ハンズオン講習会(2015年8月)」のYouTubeリスト](https://www.youtube.com/playlist?list=PL0uaKHgcG00Yo0Cn0rcF23xof5hqCzGQb)
    - [上記の動画+講習会資料のまとめページ@統合TV](http://togotv.dbcls.jp/ja/tags.html?tag=NGS速習・ハンズオン)

----

## 個々の遺伝子の発現プロファイルを調べる
### [RefEx (Reference Expression dataset)](http://refex.dbcls.jp/)
- ヒト、マウス、ラットの遺伝子発現情報リファレンスデータセット
- [http://refex.dbcls.jp/](http://refex.dbcls.jp/)
- 4つの異なる実験手法（EST、GeneChip、CAGE、RNA-seq）によって得られた正常組織、初代培養細胞、細胞株における遺伝子発現データを検索、閲覧可能
    - 最近新たに、FANTOM5 CAGEデータが追加(ヒト556種、マウス286種)
    - 掲載しているデータやオリジナルデータなどの詳細については、[RefExについて](http://refex.dbcls.jp/about.php?lang=ja)
- RefExで掲載されているデータはすべて再利用可能
    - 「RefEx analysis」として論文に引用していただいたケースも
         - [Aberrant IDH3α expression promotes malignant tumor growth by inducing HIF-1-mediated metabolic reprogramming and angiogenesis, Oncogene, (22 December 2014) | doi:10.1038/onc.2014.411](http://www.nature.com/onc/journal/vaop/ncurrent/full/onc2014411a.html)
- このツールでできること
    - 正常組織における遺伝子発現データを調べる
    - 測定手法による遺伝子発現量の差異を比較する
    - 組織特異的遺伝子をワンタッチで検索可能
    - 遺伝子発現解析などで見出された不詳な遺伝子群の機能および関係性を調べる

----

#### 【実習1】RefExを使って、組織特異的遺伝子を検索する
- 【復習用】[RefExの使い方](http://doi.org/10.7875/togotv.2014.009)

1. http://refex.dbcls.jp/ を開きます。
2. 画面中央の「組織特異的に発現する遺伝子を見る」の臓器アイコンにカーソルを合わせると、更に詳細な部位のアイコンが出るので、調べたい臓器（例として肝臓）をクリックします。  
  - ![http://gyazo.com/35c8f38340753e8f433cb8c4d8fd812b](http://i.gyazo.com/35c8f38340753e8f433cb8c4d8fd812b.jpg)

3. 検索結果一覧が表示されます。検索結果一覧では、「ソート項目の切り替え」や「絞り込み検索」、「リストへの追加」ができます。(手順11以降で解説します。)
4. 各遺伝子の青字の部分（例 [fibrinogen alpha chain](http://refex.dbcls.jp/gene_info.php?lang=ja&db=human&geneID=2243&refseq=NM_000508&unigene=Hs.351593&probe=205649_s_at))をクリックすると詳細情報を閲覧できます。
5. 「ヒートマップ on Bodyparts3D」では、表示する部位の切り替え（全身・体幹部・頭部）ができます。「皮膚・骨格筋を表示」もしくは「アニメーション表示」にチェックを入れるとどのように表示されるでしょうか。
6. 「組織40分類別データ」では、バーの上にマウスオーバーすると測定部位と発現値が表示されます。
7. 「Download」をクリックすると、表示中の遺伝子の組織40分類別の発現データがタブ区切り形式でダウンロードできます。
8. 「Probe set ID」のリンク先をクリックすると、どういう情報が参照できるでしょうか。
9. 遺伝子オントロジー([Gene Ontology](http://array.cell-innovator.com/?p=1085):GO ID)をクリックすると、そのGO termを持つ他の遺伝子を一括で検索できます。
  - 例として、[GO:0007596](http://refex.dbcls.jp/genelist.php?lang=ja&db=human&idkind=1&ids=GO:0007596)   blood coagulation をクリックしてみましょう。
  - ![遺伝子詳細情報](http://i.gyazo.com/3cca3d33c17e845ad5dae8749d7fbd15.jpg)

10. 右側のFANTOM5 CAGEのタブをクリックすると、FANTOM5 CAGEデータのビューアに切り替わります。
 - ビューアは上部が拡大図で、下部が全体表示になっています。
 - 検索窓にキーワードを入れるとサンプル名を検索できます。ヒットしたサンプルはオレンジ色で強調されます。
 - 右側に、サンプル名と発現値、サンプル分類が表示されます。
 - [RefEx用に整理したサンプル情報一覧](http://bit.ly/fantom5cagehuman)も閲覧可能です。
 - ![FANTOM5 CAGE Viewer](http://i.gyazo.com/51d0b3db07efe64a6fdafb054cd4217f.jpg)
11. 検索結果一覧に戻ります。ソート項目を切り替えて、どのように結果が変わるでしょうか。
 - ![検索結果一覧](http://i.gyazo.com/5e87d20d9b31711e797ef17677be7263.jpg)
12. 様々な条件で検索結果を絞り込むことができます。絞り込み検索は左のバーから行えます。
 - 遺伝子名に「liver」を含むデータは何件あるでしょうか。
 - 「遺伝子名」の下の「条件なし」をクリックして表示されるウインドウに「liver」と入力し、「Include」をクリックし、「この条件で絞り込み」を押します。
 - 「遺伝子名」の項目で「Exclude」に「solute」を加えると、検索結果はどう変わるでしょうか。
 - 「組織」の項目で、データ元をRNA-seqに変更したり、臓器の指定を追加すると検索結果はどう変わるでしょうか。
 - 「必ず含むデータセット」の「ALL」にチェックを入れると、検索結果はどう変わるでしょうか。
13.  個々の遺伝子の詳細情報は、リストに追加することで並列に比較することができます。
 - [肝臓特異的遺伝子の検索結果一覧](http://refex.dbcls.jp/genelist.php?lang=ja&db=human&roku_valid=1&rk[31]=31&order_key=score)に移動して、3つの遺伝子を「リストに追加」してみましょう。
 - 追加した件数は「リストを見る」の横に表示されます。
 - 「リストを見る」をクリックするとリストに移動します。
 - 『並べて表示する』にチェックを入れて、「遺伝子を並べて表示」をクリックします。
 - 遺伝子発現データやGeneOntology情報を並列に比較することで見えてくる「違い」はなんでしょうか。その違いからどういうことが推測できるでしょうか。
 - ![並列比較1](http://i.gyazo.com/ba11e4c7c38a4e78d3a64d7b8b6efee8.jpg)
 - ![並列比較2](http://i.gyazo.com/3f2f9e5cbf135a2c298ae164d6360302.jpg)
14. 自分の研究テーマに関連する、また興味のある遺伝子について検索してみましょう。

----

### [BioGPS](http://biogps.org/)
- ヒト、マウス、ラットのさまざまな組織や細胞(株)における遺伝子発現プロファイルのデータベース

- [BioGPS](http://biogps.org/)はAffymetrix社製のマイクロアレイであるGeneChipを用いたさまざまな組織や細胞(株)遺伝子発現プロファイルのデータベース。
- 検索した遺伝子に対して、種々の外部データベースを横断検索することができるだけでなく、それらの設定を保存したり、表示方法を自由にカスタマイズすることができる「Gene annotation portal」。
- 外部データベースには、Wikipedia(Gene Wiki)、著名な試薬会社の検索窓へのリンク集、pathway、Nature系DB、モデル生物DB、文献DBなど多種多様
- マウスのエキソンアレイのデータから遺伝子のスプライシングバリアント(Splicing variant)の発現状況も調べることが可能。最近ではCircadian関係のデータも。
- さらに最近のアップデートで、NCBI Gene Expression Omnibus (GEO)中から選抜されたデータセットに切り替えて発現状況を調べることが可能に。

----

#### 【実習(skip)】BioGPSを使ってある遺伝子の発現プロファイルを調べる
- 【復習用】[遺伝子発現プロファイルデータベースBioGPSを使い倒す2012](http://doi.org/10.7875/togotv.2012.075)
- [【以前の講習会動画】遺伝子発現データベースの活用法](http://doi.org/10.7875/togotv.2010.109)

1. [http://biogps.org/](http://biogps.org/)を開きます。
2.骨格筋の分化決定遺伝子であるMyogenic differentiation 1(MyoD)の発現プロファイルを調べてみましょう。中央の検索窓に「myod」と入力し、「search」を押します。
3. 表示された検索結果の中から「ID 4654」をクリックします。
4. 最初はヒトのマイクロアレイデータが表示されます。
5. 画面左側の"Current Gene List"は右上の<<アイコンをクリックすると非表示にできます。非表示にすることで画面を広く使うことができます。
6. ページ内のウインドウは通常のウインドウと同じようにドラッグによる移動やサイズの変更などを行うことができます。 歯車マークのメニューから"Open in browser" を選択すると、新しいタブで表示できます。
7. "Search" と書かれた窓に単語(組織名など)を入力すると、その単語の含まれた部分が赤くハイライト表示されます。今回は "Muscle" と入力してみます。
8. "Zoom" のバーを用いることで、グラフの表示範囲を調整することが出来ます。
9. 発現量を示すバーをクリックすると発現強度の値が表示されます。
10. マイクロアレイデータ右上の"Species: Hs"をクリックするとマウスやラットを選択できるので、"M. musculus (Mouse)"をクリックしてマウスのデータを表示できます。
11. MyoDはどの組織、細胞で強く発現しているでしょうか？
12. 場合によっては"Probeset"のプルダウンメニューから複数の項目を選択できる場合があります。これはどのようなケースが考えられるでしょうか？
13. "Static Image" をクリックすると、ズームや検索機能などのついていない、画像だけのグラフで表示されます。低スペックなマシンでは、こちらの方が軽快に動作するでしょう。
14. "Correlation"タブをクリックして検索すると、発現パターンが似ている他の遺伝子を検索できますが、どのような遺伝子が出てくるでしょうか？
15. "Downloads" をクリックすると現在表示している遺伝子の発現データを CSV 形式でダウンロードできます。
16. "Dataset"の右にある'change"をクリックすると、デフォルトで用意されているデータセットやNCBI GEO中のデータセットを検索でき、それらのデータに表示を切り替えることができます。"Species: Hs"に切り替えてから、"change"をクリックしたあと、"Default Datasets"から"Barcode on normal tissues (262 samples)"を選択します。どのようにデータが変わったでしょうか。
17. さらに"Search"からキーワード検索で、GEOのデータを検索してみましょう。"C2C12"と検索するとどのようなデータが選択できるでしょうか。
18. 右上の「default rayout」をクリックすると、検索した遺伝子に関して種々の外部データベースを横断検索できますが、どのようなデータが閲覧できるのか調べてみましょう。
19. 左上の「Search」タグをクリックして検索画面にもどり、自分の興味ある遺伝子について同様に検索してみましょう。
すぐに自分の興味ある遺伝子が浮かばない場合は、著名な[iPS細胞](http://ja.wikipedia.org/wiki/iPS細胞)を作るために必要な4因子（Oct3/4・Sox2・Klf4・c-Myc）がどの組織で発現しているか、またデータを切り替えて検索してみましょう。

- 【余談】
[BioGPSのiPhoneアプリ](http://biogps.org/iphone/)が無料で公開されていますので、「あの遺伝子はどの組織で発現してるのかな？」とふと調べたいときにお手持ちのiPhoneで遺伝子発現を調べられます。

----

## 数十～数千の遺伝子群の生物学的解釈

- マイクロアレイやNGS実験を行うと大量の発現変動遺伝子 (Differentially Expressed Genes: DEGs)が得られます｡
- 一般的な遺伝子発現解析の第一歩は､実験条件によって得られた数十～数千のDEGsが生物学的にどういう意味を持つかを考えることです。
  - ![Gyazo](http://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)
- 今回は、その方法の一つとして、[Gene Ontology (GO)](http://array.cell-innovator.com/?p=1085) の用語を使って､マイクロアレイ実験で得られたDEGsのもつ機能に、どのような特徴があるのか(転写因子活性に関する遺伝子が多いのか、細胞周期に関する遺伝子が多いのか?､ Wntパスウェイに関する遺伝子が多いのか?, など)を解析することで、生物学的解釈をしてみましょう。  

### [DAVID: The Database for Annotation, Visualization and Integrated Discovery](http://david.abcc.ncifcrf.gov/)
- アメリカ国立アレルギー・感染症研究所が開発･運用
- 原著論文 [PMID: 19131956](http://www.ncbi.nlm.nih.gov/pubmed/19131956)
- 遺伝子リストのコピペで簡単にエンリッチメント解析 ( GO､KEGG など )
- 対応生物種･遺伝子ID が 豊富｡ ID変換ツールもある
- IDリストしか投げられない (発現量込みやタイムコースデータは不可)
- 2010年以来データ更新が止まっていたが､最近､アップデートされた｡ [DAVID 6.8 (current beta release) May. 2016](https://david.ncifcrf.gov/content.jsp?file=release.html)  

#### マイクロアレイデータの準備
- サンプルデータとして、[NCBI GEO](http://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います。このデータは、ある実験の前後の2群間で有意に発現減少した遺伝子群のリストです。  

     → [マル秘遺伝子リスト](https://raw.githubusercontent.com/AJACS-training/AJACS59/master/hono/secret_list.txt)  （右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）

- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！  

#### 【実習2】DAVIDを用いて、発現データの結果を生物学的に解釈する
- 【復習用】[DAVIDを使ってマイクロアレイデータを解析する 2012](http://doi.org/10.7875/togotv.2012.079)
- 【復習用】[DAVIDの使い方 実践編](http://doi.org/10.7875/togotv.2013.033)  

1. [DAVID](http://david.abcc.ncifcrf.gov/)にアクセスし、上部メニューの「Start Analysis」をクリックします。

- ![Gyazo](http://i.gyazo.com/f976f39aeb060a96a790f0e5b281aabe.png)

2. 画面左側バーで、probe IDリストをコピペ or ファイルを指定します。
3. リストのIDの種類タイプを選択します。 … 今回は、「AFFY_ID」と「Gene List」
4. Submit List をクリックするとリストが読み込まれます。

- ![Gyazo](http://i.gyazo.com/e8275cf9dbb203b3d8577307b462c783.png)

5. アップロードしたリストは、左側バーの「List Manager」で「Uploaded List_1」として保存されています。削除やrenameもできます。

- ![Gyazo](http://i.gyazo.com/e8270d82a68decba0249daa49914fba9.png)

6. 解析を続けます。真ん中の「Functional Annotation Tool」をクリックします。
7. 「Gene Ontology」をクリックすると、Gene Ontologyを用いた解析の細かいメニューが表示されます。

- ![Gyazo](http://i.gyazo.com/38905ceb16d6b702059667e4fb404531.png)

8. 今回は、GOTERM_BP_FAT (BP = Biological Process)に注目します。その右の「Chart」をクリックすると結果がポップアップされます。

 - ![Gyazo](http://i.gyazo.com/78301700c3d952957dd599bbb83c785f.png)

9. タイトル行をクリックするとソートできます。  
10. さらに、GOTERM_CC_FAT や GOTERM_MF_FAT を見て、上位にリストされたGOTermにどのような共通点・相違点があるでしょうか。
 - CC = Cellular Component
 - ![Gyazo](http://i.gyazo.com/117720204dfb06a3f3605f4aedec2dba.png)
 - MF = Molecular Function  
 - ![Gyazo](http://i.gyazo.com/6feb8e34beab45769e2d3e66c3c5d570.png)
11. Pathways > KEGG_PATHWAY や Tissue Expression > UP_TISSUE なども見てみましょう。

12. DAVIDで得られた結果を踏まえ、「ある実験」とはどのような実験であったか考察してみましょう。
 - マル秘遺伝子リストは「ある実験の前後の2群間で有意に発現減少した遺伝子群のリスト」  
 - 生物種はArabidopsis thaliana (シロイヌナズナ)  

---

[答え合わせ](https://github.com/AJACS-training/AJACS59/blob/master/hono/answer.md)

---

#### 【実習3】これまで学んだことを踏まえて、発現データの結果を生物学的に解釈する
- DAVID の使い方に慣れてきたところで、実戦的な生物学的解釈に挑戦してみましょう。
- 今回は「正解」はありません。情報分析力と想像力が問われます。
- 例題は、[GSE28619](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE28619) をつかいます。
  - 健常者 vs アルコール性肝炎患者 の2群比較です。
  - 多重比較法（Benjamini & Hochberg）を指定して、有意水準1％未満かつ2倍以上発現差のあった遺伝子群のリストをあらかじめ用意しました。
     - 「健常者＞AH患者_遺伝子リスト」[GEO2R_Ctrl.txt](https://raw.githubusercontent.com/AJACS-training/AJACS59/master/hono/GEO2R_Ctrl.txt)
     - 「AH患者＞健常者_遺伝子リスト」[GEO2R_AH.txt](https://raw.githubusercontent.com/AJACS-training/AJACS59/master/hono/GEO2R_AH.txt)
     - (この遺伝子リストの作り方は、[AJACS御茶ノ水の回](http://doi.org/10.7875/ajacs.2015.007) で解説しています。)
- DAVID 以外のツールを使ってみる
  - [GeneTrail2](https://genetrail2.bioinf.uni-sb.de/)
    - 2016年1月公開｡ ザールラント大(独)が開発･運用｡ 原著論文 [PMID: 26787660](http://www.ncbi.nlm.nih.gov/pubmed/26787660)
    - トランスクリプトームのほか､プロテオーム､ miRNA､SNP にも対応
    - GSE 番号 の入力だけで､GEOから直接データ取得が可能
    - IDリストのほか発現量込みリスト､タイムコースデータなども使用可能
    - 主要なモデル生物種に対応
    - 実験系に適した統計解析の選択肢が豊富
    - 同じ生物種間であれば､別の解析結果同士を比較することも可能
    - 統合TV あります → [GeneTrail2を使って、エンリッチメント解析を行う](http://togotv.dbcls.jp/ja/20160616.html)
      - 解析結果セットはダウンロード可能だがアップロードして再表示はできない
      - データセットによってエラーが出て解析できない…(バグ?)
  - [Metascape](http://metascape.org/gp/index.html#/main/step1)
    - 2015年10月スタート｡ 原著論文 [PMID: 26651948](http://www.ncbi.nlm.nih.gov/pubmed/26651948)
    - [｢なぜ､DAVIDはもはや使うべきではないのか｣ 提言](http://metascape.blogspot.jp/2016/02/why-david-should-no-longer-be-used.html) → metascape 使おう
    - 対応ID: Entrez Gene ID, RefSeq, Gene Symbol, Ensembl, UCSC, UniProt.
    - 生物種は､ヒト､マウス､ラットのみ
    - IDリストのほかタイムコースなどの複数リストデータも使用可能
    - 複数リスト間のアノテーションについて差分表示が可能
    - GOのエンリッチメント解析で階層的クラスタリングもできる
    - 統合TV 作成中
      - まだシステムが不安定(?)で大量クエリ投げると結果が帰ってこない場合もある
      - Chromeだとjavascript周りでエラーが出て使えない(?)ことも
  - [GeneSetDB](http://genesetdb.auckland.ac.nz/haeremai.html)
    - 九州大学 荒木さんが開発｡ オークランド大学バイオインフォマティクス研究所が運用｡ 原著論文 [PMID: 23650583](http://www.ncbi.nlm.nih.gov/pubmed/23650583)
    - 医学・薬学分野に特化したデータベースを解析対象にすることができる
    - 統合TV あります → [GeneSetDBで遺伝子解析とエンリッチメント解析を行う](http://doi.org/10.7875/togotv.2016.002)
      - [2:50~ エンリッチメント解析を行う](https://www.youtube.com/watch?v=qqF19PaURsA&feature=youtu.be&t=2m50s)   
- 一応ひとつの答え
  - このデータを使った論文があります。
    - [Transcriptome analysis identifies TNF superfamily receptors as potential therapeutic targets in alcoholic hepatitis.](http://www.ncbi.nlm.nih.gov/pubmed/22637703)
    - Gut. 2013 Mar;62(3):452-60. doi: 10.1136/gutjnl-2011-301146.
  - 似たような結論が導かれましたか? あるいは、著者らが見逃している(かもしれない)着眼点や新たな着想が得られましたか?

## まとめ
- つまみ食い的ではありますが通り一遍の大規模発現データに対する生物学的解釈の方法を学びました。
- 「道具」を知って使い方が分かれば、あとは情報分析力と想像力の勝負。
- ぜひご自身のデータ、あるいはご自身のテーマに関連する公共データの生物学的解釈をしてみましょう。
- 実戦≒実践あるのみ
