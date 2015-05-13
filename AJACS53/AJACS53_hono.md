# AJACS御茶ノ水　遺伝子発現DB・ウェブツールの使い方　基礎編

情報・システム研究機構  
ライフサイエンス統合データベースセンター  
[小野 浩雅](https://sites.google.com/a/dbcls.rois.ac.jp/hono/) hono@dbcls.rois.ac.jp  
2015年5月21日 AJACS御茶ノ水@東京医科歯科大学  


----

これは統合データベース講習会 AJACS御茶ノ水「遺伝子発現DB・ウェブツールの使い方 基礎編」の資料です。  
講習会全体のプログラムは[こちら](http://events.biosciencedbc.jp/training/ajacs53)です。  

----

## 概要

本講習は、だれでも自由に使うことができる公共データベースやウェブツールを活用して、研究のさまざまな場面で調べることの多い個々の遺伝子発現データを簡単に調べるための方法と基礎知識について学びます。また、自ら行なった大規模発現解析の(あるいは公共データベースから取得・解析した)結果得られた数百〜数千におよぶ遺伝子セットについて、生物学的な解釈をする方法とその結果の考察を実践します。

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

----

##### 講習に際しての注意とお願い

- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます。
    - 資料を見ながら自力で進められそうな方はどんどん先に、そうでない方は講師と一緒にすすめていきましょう。
    - サイトの反応が悪い時はタイミングをずらして実行してみてください。
    - 反応が無いからと言って何度もクリックするとますます繋がらなくなってしまいます。おおらかな気持ちで臨みましょう。
- わからないことがあったら挙手にてスタッフにお知らせください。
    - 遠慮は無用です(そのための講習会です!)。おいてけぼりは楽しくありません。

----

##### いざ講習、その前に 
- 本講習内容をスムーズに理解するために押さえておくとよい基礎知識
    - [「遺伝子のDB・ウェブツールの基礎」(2012年8月AJACS筑波2)](http://motdb.dbcls.jp/?AJACS33%2Fmeso#e3b0f070)
- 非モデル生物のデータをモデル生物のデータに見立てるためのID対応表づくりについて
    - [「コマンドラインで遺伝子配列を解析する」（2012年7月）](http://motdb.dbcls.jp/?AJACS32%2Fbono)
- 次世代シーケンス解析について
    - [「次世代シーケンサー（NGS）と関連するデータベース・ツール」(2014年7月AJACS信州)](http://motdb.dbcls.jp/?AJACS48%2Fnakazato)
    - [「galaxyによるNGS解析」（2015年1月AJACSa三島)](http://togotv.dbcls.jp/20150203.html)
- さらにもっと基礎から次世代シーケンス解析について知りたい方向け
    - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース」の動画](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
  
----

## 研究現場で頻繁に使われるデータベースやツールを知る
### [統合TV](http://togotv.dbcls.jp/ja/)
- 生命科学分野の有用なデータベースやツールの使い方を動画で紹介するウェブサイト
    - http://togotv.dbcls.jp/ja/
[![統合TVトップページ](http://i.gyazo.com/457d7a15c537adc10d9b99596447508f.png)](http://gyazo.com/457d7a15c537adc10d9b99596447508f)

    - YouTube版もあります　http://www.youtube.com/user/togotv/videos
[![統合TVYouTube支店](http://i.gyazo.com/4c4ffa07ba8a0ea1846a2e76be02284e.png)](http://gyazo.com/4c4ffa07ba8a0ea1846a2e76be02284e)
    - ウェブサイトへのアクセスから結果の見方まで、操作の一挙手一投足がわかります。
        - 講義・講習などの参考資料や後輩指導の教材として利用できます。
        - 本講習中、本家サイトが繋がらない時は、統合TVのYouTube版を見ればおおよその内容がわかるようになっています。
        - 今回の講習に関連する内容の多くは、[統合TV の発現制御解析 カテゴリー](http://togotv.dbcls.jp/ja/contents/category/expression)にあります。
        - 過去の講習会の内容はそのほとんどが[統合TVに収録](http://togotv.dbcls.jp/ja/contents/category/dbcls#%E7%B5%B1%E5%90%88%E3%83%87%E3%83%BC%E3%82%BF%E3%83%99%E3%83%BC%E3%82%B9%E8%AC%9B%E7%BF%92%E4%BC%9Aajacs-%E8%AC%9B%E6%BC%94%E3%83%BB%E8%AC%9B%E7%BF%92%E5%8B%95%E7%94%BB)されており、いつでもどこでも繰り返し復習できるようになっています。
    - お探しの動画が見つからない or 統合TV未掲載の場合は、[統合TV番組リクエストフォーム](https://docs.google.com/forms/d/15pxJHnsV_Cu8B55Xy0F3jg5S9FXupkbBqONrZsyUE7k/viewform)へどうぞ!!
    - 統合TVを作ってみたい方、募集中です。

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
         -  [Aberrant IDH3α expression promotes malignant tumor growth by inducing HIF-1-mediated metabolic reprogramming and angiogenesis, Oncogene, (22 December 2014) | doi:10.1038/onc.2014.411](http://www.nature.com/onc/journal/vaop/ncurrent/full/onc2014411a.html)
- このツールでできること
    - 正常組織における遺伝子発現データを調べる
    - 測定手法による遺伝子発現量の差異を比較する
    - 組織特異的遺伝子をワンタッチで検索可能
    - 遺伝子発現解析などで見出された不詳な遺伝子群の機能および関係性を調べる

----

####【実習1】RefExを使って、組織特異的遺伝子を検索する 
- [【復習用】RefExの使い方](http://youtu.be/GC2gLzvF6t0)  

1. http://refex.dbcls.jp/ を開きます。
2. 画面中央の「組織特異的に発現する遺伝子を見る」の臓器アイコンにカーソルを合わせると、更に詳細な部位のアイコンが出るので、調べたい臓器（例として肝臓）をクリックします。  

 [![Gyazo](http://i.gyazo.com/fab7f0ba81afbce32061692c344bf03f.png)](http://gyazo.com/fab7f0ba81afbce32061692c344bf03f)

3. 検索結果一覧が表示されます。検索結果一覧では、「ソート項目の切り替え」や「絞り込み検索」、「リストへの追加」ができます。(手順11以降で解説します。)
4. 各遺伝子の青字の部分（例 [fibrinogen alpha chain](http://refex.dbcls.jp/gene_info.php?lang=ja&db=human&geneID=2243&refseq=NM_000508&unigene=Hs.351593&probe=205649_s_at))をクリックすると詳細情報を閲覧できます。

 [![Gyazo](http://i.gyazo.com/2a250c033aac172fae84b89033e1b225.png)](http://gyazo.com/2a250c033aac172fae84b89033e1b225)

5. 「ヒートマップ on Bodyparts3D」では、表示する部位の切り替え（全身・体幹部・頭部）ができます。「皮膚・骨格筋を表示」もしくは「アニメーション表示」にチェックを入れるとどのように表示されるでしょうか。
6. 「組織40分類別データ」では、バーの上にマウスオーバーすると測定部位と発現値が表示されます。

 [![Gyazo](http://i.gyazo.com/b60518629c6dd0fe8163776cc7824a3c.png)](http://gyazo.com/b60518629c6dd0fe8163776cc7824a3c)

7. 「Download」をクリックすると、表示中の遺伝子の組織40分類別の発現データがタブ区切り形式でダウンロードできます。
8. 「Probe set ID」のリンク先をクリックすると、どういう情報が参照できるでしょうか。

 [![Gyazo](http://i.gyazo.com/78a17e8253cb9ed64f6becf96b5a1e03.png)](http://gyazo.com/78a17e8253cb9ed64f6becf96b5a1e03)

9. 遺伝子オントロジー(GO ID)をクリックすると、そのGO termを持つ他の遺伝子を一括で検索できます。
 - 例として、[GO:0007596](http://refex.dbcls.jp/genelist.php?lang=ja&db=human&idkind=1&ids=GO:0007596)   blood coagulation をクリックしてみましょう。
10. 右側のFANTOM5 CAGEのタブをクリックすると、FANTOM5 CAGEデータのビューアに切り替わります。
 - ビューアは上部が拡大図で、下部が全体表示になっています。
 - 検索窓にキーワードを入れるとサンプル名を検索できます。ヒットしたサンプルはオレンジ色で強調されます。
 - 右側に、サンプル名と発現値、サンプル分類が表示されます。
 - [RefEx用に整理したサンプル情報一覧](http://bit.ly/fantom5cagehuman)も閲覧可能です。
11. 検索結果一覧に戻ります。ソート項目を切り替えて、どのように結果が変わるでしょうか。
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
 - 並列に比較することで見えてくる「違い」はなんでしょうか。

 [![Gyazo](http://i.gyazo.com/f832aab525efcbd99854b8c920be0fcf.png)](http://gyazo.com/f832aab525efcbd99854b8c920be0fcf)  
 [![Gyazo](http://i.gyazo.com/0c604ddeee80bf4adf14ce52876a5744.png)](http://gyazo.com/0c604ddeee80bf4adf14ce52876a5744)

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

####【実習(skip)】BioGPSを使ってある遺伝子の発現プロファイルを調べる 
- [【復習用】遺伝子発現プロファイルデータベースBioGPSを使い倒す2012](http://www.youtube.com/watch?v=X_exdocRIVQ)
- [【以前の講習会動画】遺伝子発現データベースの活用法](http://togotv.dbcls.jp/20100829.html#p01)

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
すぐに自分の興味ある遺伝子が浮かばない場合は、著名な[iPS細胞](http://ja.wikipedia.org/wiki/%E4%BA%BA%E5%B7%A5%E5%A4%9A%E8%83%BD%E6%80%A7%E5%B9%B9%E7%B4%B0%E8%83%9E)を作るために必要な4因子（Oct3/4・Sox2・Klf4・c-Myc）がどの組織で発現しているか、またデータを切り替えて検索してみましょう。

- 【余談】 
[BioGPSのiPhoneアプリ](http://biogps.org/iphone/)が無料で公開されていますので、「あの遺伝子はどの組織で発現してるのかな？」とふと調べたいときにお手持ちのiPhoneで遺伝子発現を調べられます。

---- 

## 数十～数千の遺伝子群の生物学的解釈 
### [DAVID: The Database for Annotation, Visualization and Integrated Discovery](http://david.abcc.ncifcrf.gov/)
- マイクロアレイデータの生物学的な解釈
- マイクロアレイ実験の一般的な目的は、実験条件によって得られた数十～数千の遺伝子群の発現が生物学的にどういう意味を持つかを考えることです。

[![Gyazo](http://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)](http://gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0)

- 今回は、その方法の一つとして、マイクロアレイの結果に[Gene Ontology](http://www.google.co.jp/url?sa=t&source=web&cd=4&ved=0CEEQFjAD&url=http%3A%2F%2Fja.wikipedia.org%2Fwiki%2F%25E9%2581%25BA%25E4%25BC%259D%25E5%25AD%2590%25E3%2582%25AA%25E3%2583%25B3%25E3%2583%2588%25E3%2583%25AD%25E3%2582%25B8%25E3%2583%25BC&ei=ve9QTd6XMtG6cbeW1KUH&usg=AFQjCNF8U-O4ktlMGoR9DNC0wKltmbjtmw)の用語を付与することで、生物学的な解釈を行います。

#### マイクロアレイデータの準備
- サンプルデータとして、[NCBI GEO](http://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います。このデータは、ある実験の前後の2群間で有意に発現減少した遺伝子群のリストです。  
  
     → [マル秘遺伝子リスト](https://raw.githubusercontent.com/hiromasaono/training/master/AJACS53/secret_list.txt)  （右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）
  
- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！  

####【実習2】DAVIDを用いて、発現データの結果を生物学的に解釈する 
- [【復習用】DAVIDを使ってマイクロアレイデータを解析する 2012](http://youtu.be/WIfe7Z_Mvxg)
- [【復習用】DAVIDの使い方 実践編](http://youtu.be/4f1t1ma9IRc)

1. 上部メニューの「Start Analysis」をクリックします。

 [![Gyazo](http://i.gyazo.com/f976f39aeb060a96a790f0e5b281aabe.png)](http://gyazo.com/f976f39aeb060a96a790f0e5b281aabe)

2. 画面左側バーで、probe IDリストをコピペ or ファイルを指定します。
3. リストのIDの種類タイプを選択します。 … 今回は、「AFFY_ID」と「Gene List」
4. Submit List をクリックするとリストが読み込まれます。

 [![Gyazo](http://i.gyazo.com/e8275cf9dbb203b3d8577307b462c783.png)](http://gyazo.com/e8275cf9dbb203b3d8577307b462c783)

5. アップロードしたリストは、左側バーの「List Manager」で「Uploaded List_1」として保存されています。削除やrenameもできます。

 [![Gyazo](http://i.gyazo.com/e8270d82a68decba0249daa49914fba9.png)](http://gyazo.com/e8270d82a68decba0249daa49914fba9)

6. 解析を続けます。真ん中の「Functional Annotation Tool」をクリックします。
7. 「Gene Ontology」をクリックすると、Gene Ontologyを用いた解析の細かいメニューが表示されます。

 [![Gyazo](http://i.gyazo.com/38905ceb16d6b702059667e4fb404531.png)](http://gyazo.com/38905ceb16d6b702059667e4fb404531)

8. 今回は、GOTERM_BP_FAT (BP = Biological Process)に注目します。その右の「Chart」をクリックすると結果がポップアップされます。 

 [![Gyazo](http://i.gyazo.com/78301700c3d952957dd599bbb83c785f.png)](http://gyazo.com/78301700c3d952957dd599bbb83c785f) 

9. タイトル行をクリックするとソートできます。  
10. さらに、GOTERM_CC_FAT や GOTERM_MF_FAT を見て、上位にリストされたGOTermにどのような共通点・相違点があるでしょうか。
 - CC = Cellular Component
 [![Gyazo](http://i.gyazo.com/117720204dfb06a3f3605f4aedec2dba.png)](http://gyazo.com/117720204dfb06a3f3605f4aedec2dba)
 - MF = Molecular Function  
 [![Gyazo](http://i.gyazo.com/6feb8e34beab45769e2d3e66c3c5d570.png)](http://gyazo.com/6feb8e34beab45769e2d3e66c3c5d570)
11. Pathways > KEGG_PATHWAY や Tissue Expression > UP_TISSUE なども見てみましょう。

12. DAVIDで得られた結果を踏まえ、「ある実験」とはどのような実験であったか考察してみましょう。
 - マル秘遺伝子リストは「ある実験の前後の2群間で有意に発現減少した遺伝子群のリスト」  
 - 生物種はArabidopsis thaliana (シロイヌナズナ)  
  
---

[答え合わせ](https://github.com/hiromasaono/training/blob/master/AJACS53/answer.md)
