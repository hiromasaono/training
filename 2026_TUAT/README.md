# Ⅱ-7 データ分析の実例 バイオインフォマティクス, Ⅱ-8 データ分析の実例（演習）

広島大学ゲノム編集イノベーションセンター / プラチナバイオ株式会社  
小野 浩雅 ([X@h_ono](https://twitter.com/h_ono), [researchmap](https://researchmap.jp/hiromasaono))  
onohrms@hiroshima-u.ac.jp

2026年3月3日(火) 小金井キャンパス、2026年3月4日(水) 府中キャンパス
東京農工大学　情報データ科学活用入門Ⅱ

----

これは、2026年度 東京農工大学「情報データ科学活用入門Ⅱ」の小野担当回の講習資料です。
© 2026 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

----

## 概要

ヒトゲノム計画が完了してから約23年(実は、つい最近まで完全には解読されていなかった - [ヒトゲノム計画とヒトゲノム完全解読](https://www.jstage.jst.go.jp/article/jsbibr/3/1/3_jsbibr.2022.primer2/_html/-char/ja))がたち、今や技術革新により日々膨大なデータが産み出され、それらは様々なデータベースに登録され、その多くは公開される時代となっています。そして、生命科学研究を効率よく進めるためには、これらのデータをいかに有効活用するかが鍵になっています。
そこで、全2回の講義では、これから研究室に所属して研究を始める皆さんを対象に、お手元のコンピュータを使ったハンズオン形式で、生命科学系の主要なデータベースとバイオインフォマティクスツールを紹介します。前半の講義（Ⅱ-7）では、統合TV（TogoTV）やNCBIを使った遺伝子情報の検索方法、ゲノムブラウザ（UCSC・Ensembl）によるゲノムデータの閲覧方法を学びます。後半の演習（Ⅱ-8）では、公共データベースから取得した遺伝子発現データを題材に、DAVIDを用いたエンリッチメント解析を通じて、実験結果を生物学的に解釈する方法を実践します。
これらのデータベースやツールは、仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化するための便利な「道具」です。ぜひご自身の手で「使い倒し」てみてください。これから始まる研究生活の中で役に立つこと請け合いです。

----
## 自己紹介
- 小野 浩雅(おの ひろまさ)([researchmap](https://researchmap.jp/hiromasaono/))
  - [TogoTV](https://togotv.dbcls.jp/)の運営・編集者
  - [RefEx](https://refex.dbcls.jp/)の開発者
    - 遺伝子発現解析の基準となる各遺伝子の遺伝子発現量を簡単に検索、閲覧できるウェブツール
  - [TogoID](https://togoid.dbcls.jp/)
    - 生命科学系データベース間のつながりを探索的に確認しながらID変換を行うことができるウェブツール
- 2024年4月から
  - [広島大学ゲノム編集イノベーションセンター](https://www.mls.sci.hiroshima-u.ac.jp/smg/ge-innovation/index.html) 研究員 / [プラチナバイオ株式会社](https://www.pt-bio.com/) 事業推進部 ディレクター
    - さまざまな産業有用生物のゲノム情報の取得や目的機能に関わる遺伝子の特定、ゲノム編集による機能向上までを一貫して実現できるプラットフォームをつくる
      - [Egg for All プロジェクト：世界初のアレルギー対応卵で食の壁を打ち破る](https://www.pt-bio.com/project/egg-for-all)


----

## 講義の流れ(予定)
今回の講義(全2回)では、お手元のコンピュータを使って以下の内容について説明します。

- [【Ⅱ-7】データ分析の実例 バイオインフォマティクス（講義）](#ⅱ-7データ分析の実例-バイオインフォマティクス講義)
  - 研究現場で頻繁に使われるデータベースやツールを知る
    - 統合TV(TogoTV)
  - 生命科学分野の王道データベースNCBIを使って遺伝子について調べる
    - NCBI
    - 遺伝子のID体系
  - ゲノムデータベースとゲノムブラウザ
    - UCSC Genome Browser
    - Ensembl Genome Browser
- [【Ⅱ-8】データ分析の実例（演習）](#ⅱ-8データ分析の実例演習)
  - 公共データベースから利用可能な遺伝子発現データを解析する
    - DAVID
      - DAVIDを用いて、遺伝子発現データの結果を生物学的に解釈する

----

## 講義に際しての注意とお願い
- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます。
    - 資料を見ながら自力で進められそうな方はどんどん先に、そうでない方は講師と一緒にすすめていきましょう。
    - サイトの反応が悪い時はタイミングをずらして実行してみてください。
    - 反応が無いからと言って何度もクリックするとますます繋がらなくなってしまいます。おおらかな気持ちで臨みましょう。

- こんなことは知ってて当たり前だと他の人に思われる質問を歓迎します。質問することのハードルを下げます。
    - 知っている人は講師を助けてください。サポート大歓迎です。
    - あなたが疑問に思ったことは、実は、隣の人やその隣の人もそう思っていることが多いです。
    - 当たり前に感じる質問や一見関係なさそうな質問がでると、「そういう質問をしてもよいのだ」という空気になり、この講義から得られる情報が増え、皆さんの受講満足度が上がります(たぶん)。
    - でも講師も知らないことは(多々)あります。(以下ループ)

----
# 【Ⅱ-7】データ分析の実例 バイオインフォマティクス（講義）
---
## 研究現場で頻繁に使われるデータベースやツールを知る
---
# TogoTV
- https://togotv.dbcls.jp/ 📺
  - 生命科学分野における有用なコンテンツを紹介するウェブサイト
    - データベースやツールの動画マニュアル
    - 講演や講習会動画・資料
    - イラスト
  - 2007年8月サービススタート
  - 2020年11月リニューアル
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220323_01.jpg)
---
# 動画マニュアル
- ウェブサイトへのアクセスの仕方から結果の解釈まで、操作の一挙手一投足がわかる
- 各動画は[YouTubeに上がって](http://www.youtube.com/user/togotv/)いて、環境に応じた解像度、倍速表示等で快適に閲覧可能
- 2,300本に迫る動画が公開されており、338万回以上 再生(2025年3月末現在)
- YouTubeのチャンネル登録をすると新規公開の通知が来て便利です…!
  -　チャンネル登録者数10,700人突破！

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20250626_01.jpg)

---
# [スキル別コース](https://togotv.dbcls.jp/courses.html)
- ある目的に対して、「この順で動画をみていくと、こういうスキルを獲得できる」というような体系的な動画リスト集
![bg right:50% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_02.png)
---

# イラストを探す (Togo picture gallery)
- [「イラストを探す」](https://togotv.dbcls.jp/pics.html)
- 生命科学分野のイラスト(約2,200本)が、誰でも自由に利用可能 (CC-BY-4.0)
- 研究発表のスライド・ポスター作成、資料作成等に､ぜひご活用ください
- [TogoTVのコンテンツを再利用したいのですが、著作権の扱いはどうなっていますか?](https://togotv.dbcls.jp/faq.html)
- 2024年4月末で120件の[引用論文](https://dbcls.rois.ac.jp/references.html#TogoTV)

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20230523_05.png)

---
- データベースやウェブツールで困ったら、まずは「統合TV」で探して・見てみましょう
- お探しの動画マニュアルや画像が見つからない場合は、[統合TV番組リクエストフォーム](https://togotv.dbcls.jp/contact.html)でお気軽にリクエストしてください。

----

## 生命科学分野の王道データベースNCBIを使って遺伝子について調べる
---
## NCBI (National Center for Biotechnology Information)
### [NCBI Databases](https://www.ncbi.nlm.nih.gov/search/?term=)
- 米国 国立生物工学情報センター (National Center for Biotechnology Information: NCBI)
- 文献、遺伝子、遺伝学、タンパク質、ゲノム、化合物といったあらゆるデータベースがあります。
![NCBI top](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220621_1.jpg)
  - **all[filter]** を使って全件数を調べられます。
![NCBI all](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220621_2.jpg)
- [【NCBI】に関係する統合TV動画](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=NCBI)
### NCBIで 遺伝子 を調べる
- <details><summary>そもそも遺伝子(gene)ってなに?　ゲノム(genome)とDNAの違いは?</summary>
    [遺伝子とゲノム](https://www.ddbj.nig.ac.jp/column/genegenome.html) (国立遺伝学研究所 生命情報・DDBJセンター ウェブサイト)</details>

- ALDH2 について調べる
  - [エタノール(エチルアルコール)](https://pubchem.ncbi.nlm.nih.gov/compound/702) の代謝産物である[アセトアルデヒド](https://pubchem.ncbi.nlm.nih.gov/compound/177)をさらに分解する、アセトアルデヒドデヒドロゲナーゼという酵素をコードしている遺伝子で、ヒトでは12番染色体に存在する


1. NCBI のトップページにALDH2と入れてみる
  - ![NCBI search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_01.jpg)
1. 遺伝子について調べたいので、[Gene](https://www.ncbi.nlm.nih.gov/gene/) を選びます
1. ALDH2 という名前の付いた遺伝子が様々な生物種込みで検索されます
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_02.jpg)
1. ヒトのALDH2を調べたいので、ALDH2 homo sapiens　としてみるとどう変わるでしょうか
1. 一番上にでてきた **ALDH2 ID:217** というのがお目当てのもののようなのでクリックします
1. NCBI Gene データベースにおける **ヒトのALDH2 のページ** [https://www.ncbi.nlm.nih.gov/gene/217](https://www.ncbi.nlm.nih.gov/gene/217) が表示されます
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_03.jpg)



#### 遺伝子のID
- Accession Number
- (NCBI) Gene ID
- Gene Symbol(遺伝子名)
- RefSeq ID

##### Accession Number
- GenBank/ENA/DDBJ 国際塩基配列データベースに登録された塩基配列のID
  - 俗にGenBankのAccession番号と呼ばれることもあるが正確ではない。
- **A12345** や **AB123456** のような形をしている
  - アルファベットの割り当てについては、[DDBJのPrefix Letter List](https://www.ddbj.nig.ac.jp/prefix-e.html)に詳細がある
- A12345**.1**のようにバージョンを表示
  - UTRが延長されたりエラーが修正されて、A12345**.2**のようにアップデートされる

##### (NCBI) Gene ID, Gene Symbol
- 遺伝子ごとに付与される番号と遺伝子

|生物種|慣用名(description)|Gene Symbol|Gene ID|
|:--|:--|:--|:--|
|ヒト|aldehyde dehydrogenase 2 family member|ALDH2|217|
|マウス|aldehyde dehydrogenase 2, mitochondrial|Aldh2|11669|
|アフリカツメガエル|aldehyde dehydrogenase 2 family member |aldh2|448267|

- Symbolは慣用名と一致しないこともある
  - [山中因子](https://kotobank.jp/word/%E5%B1%B1%E4%B8%AD%E5%9B%A0%E5%AD%90-682831)の一つで有名なOCT4は、[POU5F1](https://www.ncbi.nlm.nih.gov/gene/5460)がGene Symbol
- 別の生物種で同一のSymbolがついていることもある
- Gene ID は、生物種と遺伝子を特定できる

##### NCBI Reference Sequences (RefSeq) ID
- 国際塩基配列データベースに登録された配列を基に transcriptごと(塩基配列ごと)に1個登録→RefSeqデータベース
  - 遺伝子の百科事典のようなもの
- 選択的スプライシングで生じるvariantには別々のIDが付与されている
- NM_012345.6 の形式をしている
  - 実用上はAccession番号の一種として扱うことができる
  - NG = Genome, NM = mRNA, NP = Protein
- ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_04.jpg)
- FASTA フォーマット
  - FASTA(ファストエーと発音)フォーマットは、塩基配列やアミノ酸配列を解析するためのテキスト形式を基本としたフォーマットである。
    - Python, Ruby, Perl などのスクリプト言語と相性がよい。
    - 以下のように、> で始まる配列の名前、付加情報、改行、配列 から構成される。なお、> のあとにスペースなしで打ち込まれた文字列が配列の名前になり、スペースから改行までが付加情報になる。次の > までが配列とみなされる。
- ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_05.jpg)
- [NCBI RefSeqを使って遺伝子のmRNAやアミノ酸配列を取得する](https://doi.org/10.7875/togotv.2024.058)




#### 塩基配列から遺伝子を探す
- NCBI BLAST
  - [NCBI BLASTの使い方 〜基本編〜 2017](https://togotv.dbcls.jp/20170321.html)
- UCSC BLAT
  - [高速アラインメントツールBLATをプライマー設計支援ツールとして使う 2017](https://togotv.dbcls.jp/20171001.html)


---

## ゲノムデータベースとゲノムブラウザ
### ゲノムデータベースとは？
- ゲノム配列をはじめとした（遺伝）情報を生物種ごとにまとめたデータベース
- 狭義にはゲノム配列のデータベースを指す
### リファレンス(参照)ゲノム配列
- ヒトやその他の生物のゲノム配列は個体ごとに異なる
	- 主な生物のゲノムサイズ（塩基対数）

| 生物                     | ゲノムサイズ                      | 備考                               |
|--------------------------|-----------------------------------|------------------------------------|
| ヒト（Homo sapiens）     | 約31億塩基対（3,100 Mb, 3.1 Gb）  | 典型的な1倍体（haploid）量         |
| 大腸菌（E. coli）        | 450万～550万塩基対（4.5～5.5 Mb） | 株によって差異あり                 |
| 酵母（パン酵母）         | 約1,250万塩基対（12.5 Mb）        | Saccharomyces cerevisiae           |
| ショウジョウバエ         | 約1億3,950万塩基対（139.5 Mb）    | Drosophila melanogaster            |
| シロイヌナズナ           | 約1億3,500万塩基対（135 Mb）      | Arabidopsis thaliana               |
| マウス（ハツカネズミ）   | 約28億塩基対（2,800 Mb, 2.8 Gb）  | Mus musculus                       |

		- Mb: メガベース（100万塩基対）、Gb: ギガベース（10億塩基対）
- 基準となるゲノム配列がなければその｢違い｣を定量的に評価することができない
- 様々なゲノム配列をもとにしてその最大公約数的なゲノム配列を基準ゲノム配列として決めている
	- リファレンス配列と個々の生物のゲノム配列を比較する
	- シーケンシングされたリード配列をリファレンス配列にマッピングすることで発現量を定量する
- 各ゲノムのいわゆる「バージョン」は、アセンブリやビルドと呼ばれる
	- 広く使われているヒトゲノムのリファレンスは、GRCh38 (for Genome Research Consortium human build 38)
		- Hg38 (for Human genome build 38)と呼ばれる場合もある
- 国際基準ゲノム配列の日本人版を作成する取り組みが東北大学東北メディカル・メガバンク機構([ToMMo](https://www.megabank.tohoku.ac.jp/))で行われている
	- [日本人多層オミックス参照パネル\(jMorp\)](https://jmorp.megabank.tohoku.ac.jp/)で閲覧できる
- 2023年5月、[より完全なヒトゲノム参照配列「パンゲノム」公開](https://genetics.qlife.jp/news/20230605-w032)

#### さまざまなゲノムデータベース
- [NCBI Datasets](https://www.ncbi.nlm.nih.gov/datasets/)
    - 統合TV: [NCBI Datasetsを使ってゲノムデータを検索、閲覧、取得する](https://togotv.dbcls.jp/20240328.html)
- [GOLD: Genomes Online Database](https://gold.jgi.doe.gov/index)
	- ゲノム塩基配列解読プロジェクトを集めたデータベース
- [Plant GARDEN](https://plantgarden.jp/)
  - 植物ゲノム
- [Microbiome Datahub](https://mdatahub.org/)
  - 微生物ゲノム

#### コミュニティによるゲノムデータベース

- Mouse Genome Informatics (MGI) - マウス
	- http://www.informatics.jax.org/
- Rat Genome Database (RGD) - ラット
	- https://rgd.mcw.edu/
- WormBase - 線虫
	- https://www.wormbase.org/
- FlyBase - ショウジョウバエ
	- http://flybase.org/
- The Arabidopsis Information Resource (TAIR) - シロイヌナズナ
	- https://www.arabidopsis.org/
- Saccharomyces Genome Database (SGD) - 酵母
	- https://www.yeastgenome.org/
- CyanoBase - シアノバクテリア（光合成細菌）
	- http://genome.microbedb.jp/cyanobase/

---
### ゲノムブラウザとは？

- 塩基配列解読したゲノム配列とそこに付与（アノテーション）された情報を見るための仕組み
  - アノテーション(Annotation: 注釈)
  	-　何も書かれていないとその場所にあるものが何かわからなくなるので、付箋を貼ってあとから誰がみてもわかるように説明を書き⾜すこと
  - 生命科学分野の[Google map](https://www.google.co.jp/maps/place/%E6%9D%B1%E4%BA%AC%E8%BE%B2%E5%B7%A5%E5%A4%A7%E5%AD%A6/@35.6839,139.4807,17z?hl=ja)のようなイメージ
- オンライン型とローカル型
  - オンライン型：ウェブブラウザ上でサーバにあるゲノムデータベースから必要な情報を取り出してこれる
  	- UCSC Genome Browser https://genome.ucsc.edu/
      - 【統合TV】[「UCSC」]([https://togotv.dbcls.jp/tags.html?tag=UCSC](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=UCSC))　　51本
  	- Ensembl Genome Browser https://www.ensembl.org/
      - 【統合TV】[「Ensembl」]([https://togotv.dbcls.jp/tags.html?tag=Ensembl](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=Ensembl)) 46本
  	- NCBI Genome Data Viewer https://www.ncbi.nlm.nih.gov/genome/gdv/
  	- Togogenome http://togogenome.org/
      - 【統合TV】[TogoGenome を使って生物種とゲノムに関する多種多様な情報を統合的に検索する](https://togotv.dbcls.jp/20180726.html)
  - ローカル型：手元のコンピュータにインストールして使用
  	- Integrative Genomics Viewer(IGV) https://software.broadinstitute.org/software/igv/
      - 【統合TV】[Integrative Genomics Viewer IGVを使い倒す 〜基本編〜](https://togotv.dbcls.jp/20140529.html)

---

### 【実習1】UCSC Genome Browser　を使って遺伝子発現データを閲覧してみる
- 【統合TV】: [UCSC Genome Browser を使って様々な組織、細胞における遺伝子発現データをゲノムブラウザで表示する](https://togotv.dbcls.jp/ja/20171116.html)
- 【統合TV】: [GTEx Portalを使ってヒトの各組織での遺伝子発現量や影響するeQTLを調べる](https://togotv.dbcls.jp/20180101.html)
  - [Genotype-Tissue Expression (GTEx)](https://www.gtexportal.org/home/) プロジェクトは米国ブロード研究所(Broad Institute)をはじめとする南北米および欧州の複数の研究機関からなる国際コンソーシアムによる、ヒトの体組織ごと、遺伝子型ごとの遺伝子発現を網羅的に調べたプロジェクトです。 そのポータルサイトであるGTEx Portalでは、GTExプロジェクトで収集・解析された遺伝子の発現量や関連するeQTL(expression Quantitative Trait Locus: 遺伝子の発現量に影響を与える座位)などのデータがまとめられています。

1. 「[UCSC Genome Browser](https://genome.ucsc.edu/)」で、トップページを開きます
1. トップページにはツール名がリストされているので一番上にある「Genome Browser」をクリックします
![UCSCトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_04.png)
1. 最寄りのミラーサイトに接続します
![UCSC mirror](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_05.png)
1. Genome Browserのページが開くので、生物種「Human」と最新のゲノムアセンブリ「Dec. 2013 (GRCh38/hg38)」が選択されていることを確認して、検索語を入力する。ここでは、`ALDH2`と入力します。
![GenomeBrowserトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_06.png)
1. ALDH2遺伝子のゲノム領域が表示されます。
![GenomeBrowserトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220627_01.jpg)
1. 画面上の"zoom out"で"3x"を押してみると、少し引きの画像で見られます。
1.　画面中央のカラフルな棒グラフがGTExで測定された遺伝子発現データです。グラフをクリックすると詳細が見られます。
![GenomeBrowserトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220627_02.jpg)
1. 下の方にスクロールしていくと、"Track"と呼ばれる、ゲノムブラウザで表示できる遺伝子機能情報(アノテーション)が分野別に整理されています。
1. "Expression"の"GTEx RNA-Seq Coverage"の"hide"を"dense"に変えて、"refresh"を押します。
1. 続いて、"full"に変えてみると表示データはどう変わるでしょうか。
2. わからなくなったら、図の下に並んでいるボタンの"default tracks"を押すと最初の状態に戻せます。


#### 【復習】 UCSC Genome Browserの統合TV
- 表示できるアノテーションを調べる 2018 [`https://doi.org/10.7875/togotv.2018.124`](https://doi.org/10.7875/togotv.2018.124)
- 様々な目的の配列を取得する [`https://doi.org/10.7875/togotv.2017.098`](https://doi.org/10.7875/togotv.2017.098)

#### 【発展】 UCSC Genome Browserの統合TV
- UCSC Track Hubs を使って大規模な公共データをゲノムブラウザで閲覧する [`https://doi.org/10.7875/togotv.2019.174`](https://doi.org/10.7875/togotv.2019.174)
- UCSC Table Browserを使って多様なアノテーショントラックからデータを絞り込み閲覧･取得する [`https://doi.org/10.7875/togotv.2021.051`](https://doi.org/10.7875/togotv.2021.051)
- [UCSCゲノムブラウザを活用する @ AJACSオンライン15](https://togotv.dbcls.jp/20230207.html)

### 【実習2】 Ensembl Genome Browser

- [Ensembl Genome Browser](http://asia.ensembl.org/index.html)
   - European Bioinformatics Institute (EMBL-EBI)(欧州バイオインフォマティクス研究所) で開発、維持されているゲノムブラウザ、ゲノムアノテーション閲覧システム
   - あんさんぶる、と読みます。
   - 脊椎動物のゲノムを対象としたゲノムブラウザ
   - 比較ゲノム、進化、配列変異、転写制御などの研究をサポート
   - Ensembl Genome Browser でも上記のALDH2を検索してみましょう。
- EnsemblGenomes [`https://ensemblgenomes.org/`](https://ensemblgenomes.org/)
   - 脊椎動物以外のゲノムDB
       - EnsemblPlants （植物）
       - EnsemblMetazoa （後生動物）
       - EnsemblProtists (原生生物)
       - EnsemblFungi （菌類）
       - EnsemblBacteria （細菌）
- [Ensembl BioMart](http://asia.ensembl.org/biomart/martview/)
  - Ensembl で提供されているゲノムアノテーションを網羅的に取得したり、様々な条件で絞り込んで取得することができます。
  - 遺伝子機能情報だけでなく、塩基配列を取得したり、オーソログ情報を活用して生物種間のID対応表を作成することができるなど多くの場面で活用することができます。
  - 検索結果と同時に発行されるXMLファイルを使えば、ウェブページを経由せずプログラマティックにデータを取得することもできます。
  - 統合TV: [Ensembl BioMart を使って必要な遺伝子機能情報、塩基配列、ID対応表を網羅的に取得する](https://togotv.dbcls.jp/20220324.html)
    - 動画を見ながら、同じようにできるかやってみましょう。


#### 【参考】 Ensembl Genome Browserの統合TV

- 配列を取得する [`https://doi.org/10.7875/togotv.2017.046`](https://doi.org/10.7875/togotv.2017.046)
- 塩基配列のアラインメントを作成し生物種間で比較する 2019 [`https://doi.org/10.7875/togotv.2019.106`](https://doi.org/10.7875/togotv.2019.106)
- 過去のバージョンのゲノムアノテーションを調べる [`https://doi.org/10.7875/togotv.2017.088`](https://doi.org/10.7875/togotv.2017.088)
- 遺伝子の場所や周辺情報を調べる [`https://doi.org/10.7875/togotv.2017.082`](https://doi.org/10.7875/togotv.2017.082)

### ID変換ツール
  - [TogoID](https://togoid.dbcls.jp/)
    - 直感的なインターフェースにより生命科学系データベース(DB)間のつながりを探索的に確認しながらID変換を行うことができるウェブアプリケーションです。
    - 遺伝子、タンパク質、化合物、疾患、遺伝子バリアントといった幅広いカテゴリーに渡る65種(2022年5月時点)のIDを対象としています。
    - 変換されたIDをすぐに他のサービスで利用できるようクリップボードにコピーする機能があるほか、変換されたIDリスト、IDに対応するURL、そして変換経路のすべてのIDを含むデータをCSV形式でダウンロードすることができます。
    - 統合TV: [TogoID ver\. 2\.0を使って生命科学系データベースのさまざまなIDを探索的に変換する](https://togotv.dbcls.jp/20241219.html)
---


# 【Ⅱ-8】データ分析の実例（演習課題）
## 公共データベースから利用可能な遺伝子発現データを解析する
### 遺伝子発現データの機能解析とは
- 実験条件によって得られる遺伝子の発現量を測定する
  - 実験区と対照区
    - がんの肝臓(実験区)と健康な肝臓(対照区)
    - 薬剤投与したマウス(実験区)と生理食塩水を投与したマウス(対照区)
  - 発展編として時系列データ
- 大規模に遺伝子発現量を調べる主な方法
  - マイクロアレイ
  - NGS(Next Generation Sequencer:次世代シーケンサー)
- 発現変動遺伝子(Differentially Expressed Genes: DEGs)
  - 発現量を比較して差があった遺伝子(群)
    - ｢差があった｣の定義もいろいろある
      - n倍変化した、統計的有意に変化した、その両方、など
    - 発現量が顕著に異なる遺伝子=その実験条件に影響を受けた遺伝子
- 遺伝子発現･機能解析
  - 実験条件によって得られた数十～数千のDEGsが生物学的にどういう意味を持つかを考えることが第一歩
  - ![Gyazo](https://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)
- [Gene Ontology(GO)](https://geneontology.org/)
  - 遺伝子の属性を記述する語彙を統一化(GO term)し、種を越えた遺伝子関連情報を記述し構造化することを目的とした国際プロジェクトであり、その成果のこと
  - すべてのGO termは、**biological process（生物学的プロセス）**、**cellular component（細胞の構成要素）**、**molecular function（分子機能）** の3カテゴリーのいずれかに属し、GO term同士の上下関係が一義に決まっている(のでコンピュータで処理しやすい)
  - molecular function＞binding＞protein binding＞receptor binding＞以下、より具体的になる
  - GO term には、その根拠を示す[Evidence code](https://geneontology.org/docs/guide-go-evidence-codes/) が付いている

  - [ALDH2の場合の例](https://www.ncbi.nlm.nih.gov/gene/217#gene-ontology)
  - ![ALDH2 GO](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_1.jpg)
- GO term のエンリッチメント(Enrichment:濃縮)解析
  - 数十〜数千個のDEGsにそれぞれ付与されたGO termに、どのような偏り(=特徴)があるのかを解析することで、その実験条件のもたらす影響を生物学的に解釈をすることができる
  	- 転写因子活性に関する遺伝子が多いのか、細胞周期に関する遺伝子が多いのか､ 受容体に関する遺伝子が多いのか、など



## [DAVID: The Database for Annotation, Visualization and Integrated Discovery](https://davidbioinformatics.nih.gov)
- アメリカ国立アレルギー・感染症研究所が開発･運用 → 2023年に NIH (National Institutes of Health: 米国国立衛生研究所)に移管
- 最新の原著論文 [PMID: 35325185](https://www.ncbi.nlm.nih.gov/pubmed/35325185)
- DEGsのような遺伝子リストをコピペするだけで簡単にエンリッチメント解析 ( GO､KEGG など )することができる
- 対応生物種･遺伝子ID が 豊富｡ ID変換ツールもある
- IDリストしか投げられない (発現量込みやタイムコースデータは不可)


#### マイクロアレイデータの準備
- サンプルデータとして、[NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います。
- このデータは、 **ある実験の前後の2群間で有意に発現減少した遺伝子群** のリストです。

     → [マル秘遺伝子リスト](https://raw.githubusercontent.com/hiromasaono/training/master/2022_NUBS/secret_list.txt)  （右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）

- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！

### DAVIDを用いて、遺伝子発現データの結果を生物学的に解釈する
- 【復習用】[DAVIDを使ってマイクロアレイデータを解析する 2012](https://doi.org/10.7875/togotv.2012.079)
- 【復習用】[DAVIDの使い方 実践編](https://doi.org/10.7875/togotv.2013.033)

1. [DAVID](https://davidbioinformatics.nih.gov)にアクセスし、上部メニューの「Start Analysis」をクリックします。

  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20250630_DAVID_top.jpg)

2. 画面左側バーで、probe IDリストをコピペ or ファイルを指定します。
3. リストのIDの種類タイプを選択します。 … 今回は、「AFFY_ID」と「Gene List」
4. Submit List をクリックするとリストが読み込まれます。

  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_2.jpg)

5. アップロードしたリストは、左側バーの「List Manager」で「Uploaded List_1」として保存されています。削除やrenameもできます。

  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_3.jpg)

6. 解析を続けます。真ん中の「Functional Annotation Tool」をクリックします。
7. 「Gene Ontology」をクリックすると、Gene Ontologyを用いた解析の細かいメニューが表示されます。

  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_4.jpg)

8. 今回は、GOTERM_BP_DIRECT (BP = Biological Process)に注目します。その右の「Chart」をクリックすると結果がポップアップされます。

  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_5.jpg)

9. タイトル行をクリックするとソートできます。
  - RT = Related Terms
  - Genes = そのGO termが付与されていたリスト中の遺伝子
  - Count = そのGO termが付与されていたリスト中の遺伝子の数
  - % = そのGO termが付与されていたリスト中の遺伝子の割合
  - P-value = リスト中の遺伝子がそのGO termに偶然エンリッチする可能性を示す尺度
  - Benjamini = P-value の多重検定補正された値
10. さらに、GOTERM_CC_DIRECT や GOTERM_MF_DIRECT を見て、上位にリストされたGOTermにどのような共通点・相違点があるでしょうか。
 - CC = Cellular Component
  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_6.jpg)
 - MF = Molecular Function
  - ![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_7.jpg)
11. 余裕のある人は、Literature > PubMed なども見てみましょう。GOと違う知見が得られるかも知れません。

12. DAVIDを使って皆さんが得た結果を解析・考察してみましょう。
 - わかっていること
    - マル秘遺伝子リストは「ある実験の前後の2群間で有意に発現減少した遺伝子群のリスト」
    - 生物種はArabidopsis thaliana (シロイヌナズナ)
 - 【演習課題】「マル秘遺伝子リスト」は、 どのような実験をした結果得られたデータだと推測できるのか、あなたの考えを記載してください。

---


## まとめ
- つまみ食い的ではありましたが、全2回の講義・演習で、今日から使える便利な生命科学系公共データベース・バイオインフォマティクスツールについて学びました。
- これらの｢バイオインフォマティクス｣も顕微鏡 や 実験試薬 などと同じ「道具(ツール)」です。
- 便利な「道具」を知って、その使い方が分かれば、あとはみなさん自身の情報分析力と想像力の勝負。
  - 正面からしか見られなかったものが横や後ろやナナメから見ることができて初めて気づくことがあるかもしれません。
- 仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化していきましょう。
- データベースやウェブツールで困ったら、「統合TV」でまず探して・見てみる
- 研究に役立ったら、ぜひ引用・クレジットを!
  - DBCLSの提供するサービス(あるいはそれ以外でも)が、あなたの研究に役立ったら、どんなに些細な事でもぜひ引用(論文、URL等)してください。DBCLSの活動は、提供するサービスがどのくらい活用されたかについて主に引用数などで評価されており、利用者の方の積極的なサポートが必要不可欠です!!
  - [NBDC関連サービスの活用に関する情報提供フォーム](https://form.jst.go.jp/enquetes/nbdcexamples)
