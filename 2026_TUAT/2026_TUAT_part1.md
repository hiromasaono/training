---
marp: true
theme:
header: "2026/03/03 東京農工大学 情報データ科学活用入門Ⅱ 【Ⅱ-7】データ分析の実例 バイオインフォマティクス"
footer: 2026 小野 浩雅, CC-BY-4.0
paginate: true

---
# Ⅱ-7 データ分析の実例 バイオインフォマティクス
## 情報データ科学活用入門Ⅱ

---
広島大学ゲノム編集イノベーションセンター / プラチナバイオ株式会社
小野 浩雅 ([X@h_ono](https://twitter.com/h_ono), [researchmap](https://researchmap.jp/hiromasaono))
onohrms@hiroshima-u.ac.jp

2026年3月3日(火) 小金井キャンパス
東京農工大学　情報データ科学活用入門Ⅱ

---

これは、2026年度 東京農工大学「情報データ科学活用入門Ⅱ」の小野担当回の講習資料です。
- 資料のダウンロード
  - [https://x.gd/qM5x6](https://x.gd/qM5x6)

© 2026 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)　(出典明記でご自由にお使いください)

---

## 概要

- ヒトゲノム計画完了から約23年。技術革新により膨大なデータが日々産み出されている
- それらは様々なデータベースに登録・公開されている
- 生命科学研究を効率よく進めるために、これらのデータをいかに有効活用するかが鍵

---

## 今回の講義の目的

- 前半の講義（Ⅱ-7）では:
  - 統合TV（TogoTV）やNCBIを使った遺伝子情報の検索方法
  - ゲノムブラウザ（UCSC・Ensembl）によるゲノムデータの閲覧方法
- これらは研究サイクルを加速化・効率化するための便利な「道具」

---

## 自己紹介
- 小野 浩雅(おの ひろまさ)([researchmap](https://researchmap.jp/hiromasaono/))
  - [TogoTV](https://togotv.dbcls.jp/)の運営・編集者
  - [RefEx](https://refex.dbcls.jp/)の開発者
    - 遺伝子発現解析の基準となる各遺伝子の遺伝子発現量を簡単に検索、閲覧できるウェブツール
  - [TogoID](https://togoid.dbcls.jp/)
    - 生命科学系DB間のつながりを探索的に確認しながらID変換を行うことができるウェブツール

![bg right:40% 80%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20240924_selfintro.jpg)

---

## 自己紹介(つづき)
- 2024年4月から
  - [広島大学ゲノム編集イノベーションセンター](https://www.mls.sci.hiroshima-u.ac.jp/smg/ge-innovation/index.html) 研究員 / [プラチナバイオ株式会社](https://www.pt-bio.com/) 事業推進部 ディレクター
    - さまざまな産業有用生物のゲノム情報の取得や目的機能に関わる遺伝子の特定、ゲノム編集による機能向上までを一貫して実現できるプラットフォームをつくる
      - [Egg for All プロジェクト：世界初のアレルギー対応卵で食の壁を打ち破る](https://www.pt-bio.com/project/egg-for-all)

---

## 講義の流れ(予定)

- **【Ⅱ-7】データ分析の実例 バイオインフォマティクス（講義）** ← 今回
  - 研究現場で頻繁に使われるデータベースやツールを知る
    - 統合TV(TogoTV)
  - 生命科学分野の王道データベースNCBIを使って遺伝子について調べる
    - NCBI、遺伝子のID体系
  - ゲノムデータベースとゲノムブラウザ
    - UCSC Genome Browser、Ensembl Genome Browser

---

## 講義に際しての注意とお願い
- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます
    - 資料を見ながら自力で進められそうな方はどんどん先に進めてください
    - サイトの反応が悪い時はタイミングをずらして実行してみてください
    - 何度もクリックするとますます繋がらなくなります。おおらかな気持ちで。

---

## 講義に際しての注意とお願い(つづき)
- こんなことは知ってて当たり前だと他の人に思われる質問を歓迎します
    - 知っている人は講師を助けてください。サポート大歓迎です
    - あなたが疑問に思ったことは、隣の人もそう思っていることが多いです
    - 当たり前に感じる質問がでると、「そういう質問をしてもよいのだ」という空気になり、皆さんの受講満足度が上がります(たぶん)
    - でも講師も知らないことは(多々)あります。(以下ループ)

---

# 研究現場で頻繁に使われるデータベースやツールを知る

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

---

# 生命科学分野の王道データベースNCBIを使って遺伝子について調べる

---

## NCBI (National Center for Biotechnology Information)
### [NCBI Databases](https://www.ncbi.nlm.nih.gov/search/?term=)
- 米国 国立生物工学情報センター
- 文献、遺伝子、遺伝学、タンパク質、ゲノム、化合物といったあらゆるデータベースがあります
![NCBI top](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220621_1.jpg)

---

## NCBI Databases (つづき)

- **all[filter]** を使って全件数を調べられます
![NCBI all](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220621_2.jpg)
- [【NCBI】に関係する統合TV動画](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=NCBI)

---

## NCBIで 遺伝子 を調べる
- そもそも遺伝子(gene)ってなに?　ゲノム(genome)とDNAの違いは?
  - [遺伝子とゲノム](https://www.ddbj.nig.ac.jp/column/genegenome.html) (国立遺伝学研究所 生命情報・DDBJセンター)
- **ALDH2** について調べる
  - [エタノール](https://pubchem.ncbi.nlm.nih.gov/compound/702) の代謝産物である[アセトアルデヒド](https://pubchem.ncbi.nlm.nih.gov/compound/177)をさらに分解する、アセトアルデヒドデヒドロゲナーゼという酵素をコードしている遺伝子
  - ヒトでは12番染色体に存在する

---

## NCBI で ALDH2 を検索する

1. NCBI のトップページにALDH2と入れてみる
![NCBI search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_01.jpg)

---

## NCBI で ALDH2 を検索する (つづき)

2. 遺伝子について調べたいので、[Gene](https://www.ncbi.nlm.nih.gov/gene/) を選びます
3. ALDH2 という名前の付いた遺伝子が様々な生物種込みで検索されます
![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_02.jpg)

---

## NCBI で ALDH2 を検索する (つづき)

4. ヒトのALDH2を調べたいので、**ALDH2 homo sapiens** としてみるとどう変わるでしょうか
5. 一番上にでてきた **ALDH2 ID:217** というのがお目当てのもの
6. NCBI Gene データベースにおける **ヒトのALDH2 のページ** [https://www.ncbi.nlm.nih.gov/gene/217](https://www.ncbi.nlm.nih.gov/gene/217)
![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_03.jpg)

---

## 遺伝子のID

遺伝子を特定するために様々なIDが使われています:

- **Accession Number**
- **(NCBI) Gene ID**
- **Gene Symbol(遺伝子名)**
- **RefSeq ID**

---

## Accession Number
- GenBank/ENA/DDBJ 国際塩基配列データベースに登録された塩基配列のID
  - 俗にGenBankのAccession番号と呼ばれることもあるが正確ではない
- **A12345** や **AB123456** のような形をしている
  - アルファベットの割り当てについては、[DDBJのPrefix Letter List](https://www.ddbj.nig.ac.jp/prefix-e.html)に詳細がある
- A12345**.1**のようにバージョンを表示
  - UTRが延長されたりエラーが修正されて、A12345**.2**のようにアップデートされる

---

## (NCBI) Gene ID, Gene Symbol
- 遺伝子ごとに付与される番号と遺伝子名

|生物種|慣用名(description)|Gene Symbol|Gene ID|
|:--|:--|:--|:--|
|ヒト|aldehyde dehydrogenase 2 family member|ALDH2|217|
|マウス|aldehyde dehydrogenase 2, mitochondrial|Aldh2|11669|
|アフリカツメガエル|aldehyde dehydrogenase 2 family member |aldh2|448267|

- Symbolは慣用名と一致しないこともある
  - [山中因子](https://kotobank.jp/word/%E5%B1%B1%E4%B8%AD%E5%9B%A0%E5%AD%90-682831)の一つで有名なOCT4は、[POU5F1](https://www.ncbi.nlm.nih.gov/gene/5460)がGene Symbol
- Gene ID は、生物種と遺伝子を特定できる

---

## NCBI Reference Sequences (RefSeq) ID
- 国際塩基配列データベースに登録された配列を基に transcriptごとに1個登録→RefSeqデータベース
  - 遺伝子の百科事典のようなもの
- 選択的スプライシングで生じるvariantには別々のIDが付与されている
- **NM_012345.6** の形式
  - NG = Genome, NM = mRNA, NP = Protein
![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_04.jpg)

---

## FASTA フォーマット
- FASTA(ファストエーと発音)フォーマットは、塩基配列やアミノ酸配列を解析するためのテキスト形式を基本としたフォーマット
  - Python, Ruby, Perl などのスクリプト言語と相性がよい
  - `>` で始まる配列の名前、付加情報、改行、配列 から構成される
  - `>` のあとにスペースなしで打ち込まれた文字列が配列の名前
![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220617_05.jpg)
- [NCBI RefSeqを使って遺伝子のmRNAやアミノ酸配列を取得する](https://doi.org/10.7875/togotv.2024.058)

---

## 塩基配列から遺伝子を探す
- NCBI BLAST
  - [NCBI BLASTの使い方 〜基本編〜 2017](https://togotv.dbcls.jp/20170321.html)
- UCSC BLAT
  - [高速アラインメントツールBLATをプライマー設計支援ツールとして使う 2017](https://togotv.dbcls.jp/20171001.html)

---

# ゲノムデータベースとゲノムブラウザ

---

## ゲノムデータベースとは？
- ゲノム配列をはじめとした（遺伝）情報を生物種ごとにまとめたデータベース
- 狭義にはゲノム配列のデータベースを指す

## リファレンス(参照)ゲノム配列
- ヒトやその他の生物のゲノム配列は個体ごとに異なる
- 基準となるゲノム配列がなければその｢違い｣を定量的に評価することができない
- 様々なゲノム配列をもとにして最大公約数的なゲノム配列を基準として決めている

---

## 主な生物のゲノムサイズ（塩基対数）

| 生物                     | ゲノムサイズ                      | 備考                               |
|--------------------------|-----------------------------------|------------------------------------|
| ヒト（Homo sapiens）     | 約31億塩基対（3,100 Mb, 3.1 Gb）  | 典型的な1倍体（haploid）量         |
| 大腸菌（E. coli）        | 450万～550万塩基対（4.5～5.5 Mb） | 株によって差異あり                 |
| 酵母（パン酵母）         | 約1,250万塩基対（12.5 Mb）        | Saccharomyces cerevisiae           |
| ショウジョウバエ         | 約1億3,950万塩基対（139.5 Mb）    | Drosophila melanogaster            |
| シロイヌナズナ           | 約1億3,500万塩基対（135 Mb）      | Arabidopsis thaliana               |
| マウス（ハツカネズミ）   | 約28億塩基対（2,800 Mb, 2.8 Gb）  | Mus musculus                       |

Mb: メガベース（100万塩基対）、Gb: ギガベース（10億塩基対）

---

## リファレンスゲノムの利用

- リファレンス配列と個々の生物のゲノム配列を比較する
- シーケンシングされたリード配列をリファレンス配列にマッピングすることで発現量を定量する
- 各ゲノムのいわゆる「バージョン」は、アセンブリやビルドと呼ばれる
  - 広く使われているヒトゲノムのリファレンスは、GRCh38 (Genome Research Consortium human build 38)
    - Hg38 (Human genome build 38)と呼ばれる場合もある
- [日本人多層オミックス参照パネル(jMorp)](https://jmorp.megabank.tohoku.ac.jp/)
- 2023年5月、[より完全なヒトゲノム参照配列「パンゲノム」公開](https://genetics.qlife.jp/news/20230605-w032)

---

## さまざまなゲノムデータベース

- [NCBI Datasets](https://www.ncbi.nlm.nih.gov/datasets/)
    - 統合TV: [NCBI Datasetsを使ってゲノムデータを検索、閲覧、取得する](https://togotv.dbcls.jp/20240328.html)
- [GOLD: Genomes Online Database](https://gold.jgi.doe.gov/index) - ゲノム塩基配列解読プロジェクトを集めたDB
- [Plant GARDEN](https://plantgarden.jp/) - 植物ゲノム
- [Microbiome Datahub](https://mdatahub.org/) - 微生物ゲノム

---

## コミュニティによるゲノムデータベース

- [Mouse Genome Informatics (MGI)](http://www.informatics.jax.org/) - マウス
- [Rat Genome Database (RGD)](https://rgd.mcw.edu/) - ラット
- [WormBase](https://www.wormbase.org/) - 線虫
- [FlyBase](http://flybase.org/) - ショウジョウバエ
- [The Arabidopsis Information Resource (TAIR)](https://www.arabidopsis.org/) - シロイヌナズナ
- [Saccharomyces Genome Database (SGD)](https://www.yeastgenome.org/) - 酵母
- [CyanoBase](http://genome.microbedb.jp/cyanobase/) - シアノバクテリア（光合成細菌）

---

## ゲノムブラウザとは？

- 塩基配列解読したゲノム配列とそこに付与（アノテーション）された情報を見るための仕組み
  - アノテーション(Annotation: 注釈) = 付箋を貼って説明を書き⾜すこと
  - 生命科学分野の[Google Map](https://www.google.co.jp/maps/place/%E6%9D%B1%E4%BA%AC%E8%BE%B2%E5%B7%A5%E5%A4%A7%E5%AD%A6/@35.6839,139.4807,17z?hl=ja)のようなイメージ

---

## ゲノムブラウザの種類

- **オンライン型**：ウェブブラウザ上でサーバにあるゲノムDBから必要な情報を取り出す
  - [UCSC Genome Browser](https://genome.ucsc.edu/) 【[統合TV](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=UCSC)】51本
  - [Ensembl Genome Browser](https://www.ensembl.org/) 【[統合TV](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=Ensembl)】46本
  - [NCBI Genome Data Viewer](https://www.ncbi.nlm.nih.gov/genome/gdv/)
  - [TogoGenome](http://togogenome.org/) 【[統合TV](https://togotv.dbcls.jp/20180726.html)】
- **ローカル型**：手元のコンピュータにインストールして使用
  - [Integrative Genomics Viewer (IGV)](https://software.broadinstitute.org/software/igv/) 【[統合TV](https://togotv.dbcls.jp/20140529.html)】

---

# 【実習1】UCSC Genome Browser を使って遺伝子発現データを閲覧してみる

- 【統合TV】: [UCSC Genome Browser を使って様々な組織、細胞における遺伝子発現データをゲノムブラウザで表示する](https://togotv.dbcls.jp/ja/20171116.html)
- 【統合TV】: [GTEx Portalを使ってヒトの各組織での遺伝子発現量や影響するeQTLを調べる](https://togotv.dbcls.jp/20180101.html)

---

## GTEx プロジェクト

- [Genotype-Tissue Expression (GTEx)](https://www.gtexportal.org/home/) プロジェクト
  - 米国ブロード研究所をはじめとする国際コンソーシアム
  - ヒトの体組織ごと、遺伝子型ごとの遺伝子発現を網羅的に調べたプロジェクト
  - 遺伝子の発現量や関連するeQTL(expression Quantitative Trait Locus: 遺伝子の発現量に影響を与える座位)などのデータがまとめられている

---

## 実習1の手順 (1/3)

1. 「[UCSC Genome Browser](https://genome.ucsc.edu/)」で、トップページを開きます
2. 「Genome Browser」をクリックします
![UCSCトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_04.png)

---

## 実習1の手順 (2/3)

3. 最寄りのミラーサイトに接続します
4. 生物種「Human」と最新のゲノムアセンブリ「Dec. 2013 (GRCh38/hg38)」が選択されていることを確認して、`ALDH2`と入力します
![GenomeBrowserトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_06.png)

---

## 実習1の手順 (3/3)

5. ALDH2遺伝子のゲノム領域が表示されます
6. "zoom out"で"3x"を押してみると、少し引きの画像で見られます
7. 画面中央のカラフルな棒グラフがGTExで測定された遺伝子発現データ。クリックすると詳細が見られます
![GenomeBrowser](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220627_02.jpg)

---

## 実習1: Track の表示を変更する

8. 下にスクロールすると、"Track"と呼ばれるアノテーションが分野別に整理されています
9. "Expression"の"GTEx RNA-Seq Coverage"の"hide"を"dense"に変えて、"refresh"を押します
10. 続いて、"full"に変えてみると表示データはどう変わるでしょうか
11. わからなくなったら、"default tracks"ボタンを押すと最初の状態に戻せます

---

## 【復習】 UCSC Genome Browserの統合TV
- 表示できるアノテーションを調べる 2018 [`https://doi.org/10.7875/togotv.2018.124`](https://doi.org/10.7875/togotv.2018.124)
- 様々な目的の配列を取得する [`https://doi.org/10.7875/togotv.2017.098`](https://doi.org/10.7875/togotv.2017.098)

## 【発展】 UCSC Genome Browserの統合TV
- UCSC Track Hubs を使って大規模な公共データをゲノムブラウザで閲覧する [`https://doi.org/10.7875/togotv.2019.174`](https://doi.org/10.7875/togotv.2019.174)
- UCSC Table Browserを使って多様なアノテーショントラックからデータを絞り込み閲覧･取得する [`https://doi.org/10.7875/togotv.2021.051`](https://doi.org/10.7875/togotv.2021.051)
- [UCSCゲノムブラウザを活用する @ AJACSオンライン15](https://togotv.dbcls.jp/20230207.html)

---

# 【実習2】 Ensembl Genome Browser

---

## Ensembl Genome Browser
- [Ensembl Genome Browser](http://asia.ensembl.org/index.html)
   - European Bioinformatics Institute (EMBL-EBI) で開発、維持
   - あんさんぶる、と読みます
   - 脊椎動物のゲノムを対象としたゲノムブラウザ
   - 比較ゲノム、進化、配列変異、転写制御などの研究をサポート
   - **Ensembl Genome Browser でも ALDH2 を検索してみましょう**

---

## EnsemblGenomes
- [EnsemblGenomes](https://ensemblgenomes.org/) - 脊椎動物以外のゲノムDB
  - EnsemblPlants （植物）
  - EnsemblMetazoa （後生動物）
  - EnsemblProtists (原生生物)
  - EnsemblFungi （菌類）
  - EnsemblBacteria （細菌）

---

## Ensembl BioMart
- [Ensembl BioMart](http://asia.ensembl.org/biomart/martview/)
  - Ensembl で提供されているゲノムアノテーションを網羅的に取得したり、様々な条件で絞り込んで取得できる
  - 遺伝子機能情報だけでなく、塩基配列を取得したり、オーソログ情報を活用して生物種間のID対応表を作成することもできる
  - 検索結果と同時に発行されるXMLファイルでプログラマティックにデータ取得も可能
  - 統合TV: [Ensembl BioMart を使って必要な遺伝子機能情報、塩基配列、ID対応表を網羅的に取得する](https://togotv.dbcls.jp/20220324.html)
    - **動画を見ながら、同じようにできるかやってみましょう**

---

## 【参考】 Ensembl Genome Browserの統合TV

- 配列を取得する [`https://doi.org/10.7875/togotv.2017.046`](https://doi.org/10.7875/togotv.2017.046)
- 塩基配列のアラインメントを作成し生物種間で比較する 2019 [`https://doi.org/10.7875/togotv.2019.106`](https://doi.org/10.7875/togotv.2019.106)
- 過去のバージョンのゲノムアノテーションを調べる [`https://doi.org/10.7875/togotv.2017.088`](https://doi.org/10.7875/togotv.2017.088)
- 遺伝子の場所や周辺情報を調べる [`https://doi.org/10.7875/togotv.2017.082`](https://doi.org/10.7875/togotv.2017.082)

---

## ID変換ツール: TogoID
- [TogoID](https://togoid.dbcls.jp/)
  - 直感的なインターフェースにより生命科学系データベース(DB)間のつながりを探索的に確認しながらID変換を行うことができるウェブアプリケーション
  - 遺伝子、タンパク質、化合物、疾患、遺伝子バリアントといった幅広いカテゴリーに渡る65種のIDを対象
  - 変換されたIDをすぐにクリップボードにコピー、CSV形式でダウンロード可能
  - 統合TV: [TogoID ver. 2.0を使って生命科学系データベースのさまざまなIDを探索的に変換する](https://togotv.dbcls.jp/20241219.html)

---

## 【Ⅱ-7】まとめ

- 統合TV(TogoTV)は生命科学分野の「道具箱」
  - データベースやウェブツールで困ったら、まず探して・見てみましょう
- NCBIは生命科学分野の王道データベース
  - 遺伝子のIDの種類と使い方を理解しましょう
- ゲノムブラウザ(UCSC, Ensembl)でゲノムデータを閲覧できる
  - さまざまなアノテーション情報を重ねて見ることができる
- 次回（Ⅱ-8）は、公共データベースから取得した遺伝子発現データのエンリッチメント解析を行います
