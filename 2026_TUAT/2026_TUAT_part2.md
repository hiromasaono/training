---
marp: true
theme:
header: "2026/03/04 東京農工大学 情報データ科学活用入門Ⅱ 【Ⅱ-8】データ分析の実例（演習）"
footer: 2026 小野 浩雅, CC-BY-4.0
paginate: true

---
# Ⅱ-8 データ分析の実例（演習）
## 情報データ科学活用入門Ⅱ

---
広島大学ゲノム編集イノベーションセンター / プラチナバイオ株式会社
小野 浩雅 ([X@h_ono](https://twitter.com/h_ono), [researchmap](https://researchmap.jp/hiromasaono))
onohrms@hiroshima-u.ac.jp

2026年3月4日(水) 府中キャンパス
東京農工大学　情報データ科学活用入門Ⅱ

---

これは、2026年度 東京農工大学「情報データ科学活用入門Ⅱ」の小野担当回の講習資料です。
- 資料のダウンロード
  - [https://x.gd/qM5x6](https://x.gd/qM5x6)

© 2026 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)　(出典明記でご自由にお使いください)

---

## 前回（Ⅱ-7）の振り返り

- 統合TV(TogoTV) - 生命科学分野のデータベース・ツールの動画マニュアル
- NCBI - 生命科学分野の王道データベース、遺伝子IDの体系
- ゲノムブラウザ(UCSC, Ensembl) - ゲノムデータの閲覧

## 今回（Ⅱ-8）の内容

- 公共データベースから利用可能な遺伝子発現データを解析する
- **DAVID** を用いたエンリッチメント解析で、実験結果を生物学的に解釈する

---

# 公共データベースから利用可能な遺伝子発現データを解析する

---

## 遺伝子発現データの機能解析とは

- 実験条件によって得られる遺伝子の発現量を測定する
  - **実験区と対照区**
    - がんの肝臓(実験区)と健康な肝臓(対照区)
    - 薬剤投与したマウス(実験区)と生理食塩水を投与したマウス(対照区)
  - 発展編として時系列データ

---

## 大規模に遺伝子発現量を調べる主な方法

- **マイクロアレイ**
  - DNAチップ上にプローブを配置し、蛍光強度で発現量を測定
- **NGS(Next Generation Sequencer:次世代シーケンサー)**
  - RNA-seq: mRNAの配列を直接読み取り、マッピング数で発現量を定量

---

## 発現変動遺伝子(DEGs)

- **Differentially Expressed Genes (DEGs)**
  - 発現量を比較して差があった遺伝子(群)
  - ｢差があった｣の定義もいろいろある
    - n倍変化した、統計的有意に変化した、その両方、など
  - 発現量が顕著に異なる遺伝子 = その実験条件に影響を受けた遺伝子

---

## 遺伝子発現・機能解析

- 実験条件によって得られた数十～数千のDEGsが生物学的にどういう意味を持つかを考えることが第一歩

![Gyazo](https://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)

---

## Gene Ontology(GO)

- [Gene Ontology(GO)](https://geneontology.org/)
  - 遺伝子の属性を記述する語彙を統一化(GO term)し、種を越えた遺伝子関連情報を記述し構造化することを目的とした国際プロジェクト
- すべてのGO termは3カテゴリーのいずれかに属する:
  - **Biological Process（生物学的プロセス）**
  - **Cellular Component（細胞の構成要素）**
  - **Molecular Function（分子機能）**
- GO term同士の上下関係が一義に決まっている(コンピュータで処理しやすい)

---

## Gene Ontology の構造

- molecular function ＞ binding ＞ protein binding ＞ receptor binding ＞ 以下、より具体的になる
- GO term には、その根拠を示す[Evidence code](https://geneontology.org/docs/guide-go-evidence-codes/) が付いている
- [ALDH2の場合の例](https://www.ncbi.nlm.nih.gov/gene/217#gene-ontology)
![ALDH2 GO](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_1.jpg)

---

## GO term のエンリッチメント(Enrichment:濃縮)解析

- 数十〜数千個のDEGsにそれぞれ付与されたGO termに、どのような偏り(=特徴)があるのかを解析する
  - その実験条件のもたらす影響を生物学的に解釈することができる
  - 転写因子活性に関する遺伝子が多いのか
  - 細胞周期に関する遺伝子が多いのか
  - 受容体に関する遺伝子が多いのか、など

---

# DAVID を用いた遺伝子発現データの解析

---

## DAVID: The Database for Annotation, Visualization and Integrated Discovery
- [https://davidbioinformatics.nih.gov](https://davidbioinformatics.nih.gov)
- アメリカ国立アレルギー・感染症研究所が開発･運用 → 2023年にNIHに移管
- 最新の原著論文 [PMID: 35325185](https://www.ncbi.nlm.nih.gov/pubmed/35325185)

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20250630_DAVID_top.jpg)

---

## DAVIDの特徴

- DEGsのような遺伝子リストをコピペするだけで簡単にエンリッチメント解析 ( GO､KEGG など )することができる
- 対応生物種･遺伝子ID が豊富。ID変換ツールもある
- IDリストしか投げられない (発現量込みやタイムコースデータは不可)

---

## マイクロアレイデータの準備

- サンプルデータとして、[NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います
- このデータは、 **ある実験の前後の2群間で有意に発現減少した遺伝子群** のリストです

→ [マル秘遺伝子リスト](https://raw.githubusercontent.com/hiromasaono/training/master/2022_NUBS/secret_list.txt)
（右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）

- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！

---

## DAVID を使ってみよう
- 【復習用】[DAVIDを使ってマイクロアレイデータを解析する 2012](https://doi.org/10.7875/togotv.2012.079)
- 【復習用】[DAVIDの使い方 実践編](https://doi.org/10.7875/togotv.2013.033)

---

## 実習の手順 (1/4)

1. [DAVID](https://davidbioinformatics.nih.gov)にアクセスし、上部メニューの「Start Analysis」をクリックします

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20250630_DAVID_top.jpg)

---

## 実習の手順 (2/4)

2. 画面左側バーで、probe IDリストをコピペ or ファイルを指定します
3. リストのIDの種類タイプを選択します。 … 今回は、「**AFFY_ID**」と「**Gene List**」
4. Submit List をクリックするとリストが読み込まれます

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_2.jpg)

---

## 実習の手順 (3/4)

5. アップロードしたリストは、左側バーの「List Manager」で「Uploaded List_1」として保存されています

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_3.jpg)

6. 解析を続けます。真ん中の「**Functional Annotation Tool**」をクリックします

---

## 実習の手順 (4/4)

7. 「**Gene Ontology**」をクリックすると、Gene Ontologyを用いた解析の細かいメニューが表示されます

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_4.jpg)

8. 今回は、**GOTERM_BP_DIRECT** (BP = Biological Process)に注目します。その右の「Chart」をクリックすると結果がポップアップされます

---

## 結果の見方

![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_5.jpg)

- タイトル行をクリックするとソートできます
  - **RT** = Related Terms
  - **Genes** = そのGO termが付与されていたリスト中の遺伝子
  - **Count** = そのGO termが付与されていたリスト中の遺伝子の数
  - **%** = そのGO termが付与されていたリスト中の遺伝子の割合

---

## 結果の見方 (つづき)

- **P-value** = リスト中の遺伝子がそのGO termに偶然エンリッチする可能性を示す尺度
- **Benjamini** = P-value の多重検定補正された値

---

## 他のカテゴリーも見てみましょう

- **GOTERM_CC_DIRECT** (CC = Cellular Component)
![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_6.jpg)

---

## 他のカテゴリーも見てみましょう (つづき)

- **GOTERM_MF_DIRECT** (MF = Molecular Function)
![DAVID](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_7.jpg)

- 上位にリストされたGO Termにどのような共通点・相違点があるでしょうか

---

## さらに深く解析する

- 余裕のある人は、**Literature > PubMed** なども見てみましょう
  - GOと違う知見が得られるかも知れません

---

## 考察してみましょう

DAVIDを使って皆さんが得た結果を解析・考察してみましょう。

- わかっていること
  - マル秘遺伝子リストは「**ある実験の前後の2群間で有意に発現減少した遺伝子群のリスト**」
  - 生物種は **Arabidopsis thaliana (シロイヌナズナ)**

**「マル秘遺伝子リスト」は、どのような実験をした結果得られたデータだと推測できるのか、考えてみましょう。**

---

## 答え合わせ

- マル秘遺伝子リストは、以下の比較実験をして得たマイクロアレイデータの発現減少遺伝子群でした
  - **植物細胞**と**細胞壁分解酵素を用いて取り除いた植物細胞（プロトプラスト)** との比較
  - ＝植物細胞のカルス作成前・後
- オリジナルデータ取得元 [GSE15515](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE15515)

---

## 生物学的解釈の一例

- カルス = 植物の脱分化された細胞
  - 分化した植物細胞は、G0期という特別な細胞周期に入り、細胞分裂を行わずに休止
  - 植物細胞は分化全能性を保持しているため、未分化の状態に戻せば再分化させることができる
- 脱分化が分化した機能の消失を招くならば:
  - 植物細胞が機能をしている ≒ **光合成をする**
  - GOエンリッチメント解析で｢**光合成**｣や｢**クロロプラスト**｣が極めて低いP-valueを示し上位に並んだこととと一致する

---

## 考察についての補足

- 植物や細胞生物学の背景知識が必要なので、正解できなくても落ち込む必要はありません
- 研究は答えのない問いの｢答え｣を自分で作り他人に納得してもらうような作業
  - その練習をしてもらいました
  - かなり難しかったと思いますが、プロの研究者でもそう感じる内容ですのでご安心ください
- 正解がわかった上で、もう一度講義資料を見返してみると新たな見方ができるかもしれません

---

# 全2回のまとめ

---

## まとめ

- 今日から使える便利な生命科学系公共データベース・バイオインフォマティクスツールについて学びました
- ｢バイオインフォマティクス｣も顕微鏡や実験試薬と同じ「**道具(ツール)**」です
- 便利な「道具」を知って、使い方が分かれば、あとは皆さん自身の **情報分析力と想像力** の勝負
  - 正面からしか見られなかったものが横や後ろやナナメから見ることができて初めて気づくことがあるかもしれません

---

## まとめ (つづき)

- 仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という **研究サイクルを加速化・効率化** していきましょう
- データベースやウェブツールで困ったら、「**統合TV**」でまず探して・見てみる
- 研究に役立ったら、ぜひ **引用・クレジット** を!
  - DBCLSの提供するサービスが、あなたの研究に役立ったら、どんなに些細な事でもぜひ引用してください
  - [NBDC関連サービスの活用に関する情報提供フォーム](https://form.jst.go.jp/enquetes/nbdcexamples)
