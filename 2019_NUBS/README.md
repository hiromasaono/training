# これから研究室に入る初学者のための便利な生命科学系公共データベースとウェブツールハンズオン
## [bit.ly/1906NUBS](http://bit.ly/1906NUBS)
### 課題提出用Googleフォームはこちら(予定地)

大学共同利用機関法人 情報・システム研究機構  
データサイエンス共同利用基盤施設  
[ライフサイエンス統合データベースセンター (DBCLS)](https://dbcls.rois.ac.jp/)   
小野 浩雅 ([Twitter](https://twitter.com/h_ono), [個人サイト](https://sites.google.com/dbcls.rois.ac.jp/hono/))  
hono@dbcls.rois.ac.jp  

2019年6月4、11、18日(火曜日4限（14:40-16:10))  
日本大学 生物資源学部 応用生物科学科 3年次開講科目「生命情報科学（必修）」

----

これは、2019年度 日本大学 生物資源学部 応用生物科学科 3年次開講科目「生命情報科学（必修）」の小野担当回の講習資料です。SNSによる情報拡散 **大歓迎** です。  
© 2019 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

----

## 概要

ヒトゲノム計画が完了してから15年がたち、今や技術革新により日々膨大なデータが産み出され、公共データベースに登録される時代となりました。そして、これらの有用なデータは、生命科学研究を効率よく進めるためには避けて通れない時代になっています。  
そこで、本講習では、これから研究室に所属して研究を始める皆さんを対象に、誰でも自由に使える便利な生命科学系のデータベースやウェブツールをご自分のコンピュータを使ったハンズオン形式で紹介します。
仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化するための便利な「道具」を、ぜひご自身の手で「使い倒し」てみてください。これから始まる研究生活の中で役に立つこと請け合いです。

----

## 講義の流れ
今回の講義(全3回)では、お手元のコンピュータを使って以下の内容について説明します。

- 研究現場で頻繁に使われるデータベースやツールを知る
    - 統合TV
- 学術論文を効率的に検索する
    - PubMed
    - 新着論文レビュー
    - 領域融合レビュー
- 生命科学系の文献に頻出する英語表現を高速に検索する
    - inMeXes
- 生命科学分野の略語・展開形を検索する
    - Allie
- 類似したテキストの差分を検索・表示する
    - difff(ﾃﾞｭﾌﾌ)
- 生命科学分野のデータベース
  - NCBI
- 遺伝子やゲノム配列を高速に検索する
    - GGRNA
    - GGGenome
    - CRISPRdirect
- 公共データベースから利用可能な遺伝子発現データを解析する
    - RefEx
      - 【実習】RefExを使って、組織特異的遺伝子を検索する
    - ChIP-Atlas
      - 【実習】ChIP-AtlasのEnrichment Analysis を使って、興味ある遺伝子リストを制御する可能性の高い転写因子を調べる

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

## 研究現場で頻繁に使われるデータベースやツールを知る
### [統合TV](https://togotv.dbcls.jp/)
#### 生命科学分野の有用なデータベースやツールの使い方を動画で紹介するウェブサイト
- https://togotv.dbcls.jp/
- ![統合TVトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_01.png)
- 各動画は[YouTubeに上がって](https://www.youtube.com/user/togotv/)おり、おなじみの再生画面で快適にご覧いただけます。(環境に応じた解像度、倍速表示等)
- 1600本を超える動画が公開されており、YouTube版だけで のべ 1,300,000回以上 再生されています。(2019年4月末現在)
- ![YouTube統計](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_03.png)
- ![統合TV 再生画面](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_02.png)
  - ウェブサイトへのアクセスの仕方から結果の解釈まで、操作の一挙手一投足がわかります。
  - 動画ファイルのみのダウンロードも可能で、オフライン視聴もできます。
  - 動画の概要を示すダイジェスト見出し
  - 各動画には、恒久的な URL として利用されている [DOI](https://ja.wikipedia.org/wiki/デジタルオブジェクト識別子) (Digital Object Identifier) が付与されています(引用可能)。
  - 講義・講習などの参考資料や後輩指導の教材として利用できます。
    - 本講義中、本家サイトが繋がらない時は、統合TVを見ればおおよその内容がわかるようになっています。

#### 動画以外のコンテンツも拡充中
- [AJACS講習会資料](https://togotv.dbcls.jp/ja/ajacs_text.html)
  - 2014年8月以降に開催された過去の講習会の資料・テキストと動画が同時閲覧できます。
  - 受講生の復習のみならず、初学者の学習教材として活用できます。
- [Togo Picture Gallery(静止画)](https://togotv.dbcls.jp/ja/pics.html)
  - 誰でも自由に利用可能なライフサイエンス分野のイラストが､統合TVから閲覧､利用することができるようになりました。[「自由に使える画像を探す」](https://togotv.dbcls.jp/ja/pics.html)
  - Togo picture galleryと[生物アイコン](https://togodb.biosciencedbc.jp/togodb/view/taxonomy_icon)の全画像500点以上を一覧できます。
  - 研究発表のスライド作成や資料作成等に､ぜひお使いください。
  - ![自由に使える画像を探す](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_04.png)

#### 募集と宣伝
- お探しの動画・静止画が見つからない場合は、[統合TV番組リクエストフォーム](https://togotv.dbcls.jp/contact.html)でお気軽にリクエストを。
- 統合TVでコンテンツを作ってみたい方も募集中です。
  - オンラインで完結する作成環境を整備しており、遠隔地でもOKです。謝金あり。)
  - 興味ある方は小野(hono@dbcls.rois.ac.jp)までご一報を。
- 統合TVを効果的に利用するためのガイドブックが出版されました。(2018年12月)
  - 生命科学データベース・ウェブツール  － 図解と動画で使い方がわかる！ 研究がはかどる定番18選 －
  - 「定番」として何がよく使われているのかを知り、その使い方を学び、どう使うと便利なのかについて、体系的にまとめて俯瞰的に捉えられるように編集されています。
  - 「この順で動画をみていくと、こういうスキルを獲得できる」というような体系的な教材です。
  - [https://www.amazon.co.jp/dp/4815701431/](https://www.amazon.co.jp/dp/4815701431/)
  - [https://www.medsi.co.jp/books/products/detail.php?product_id=3665](https://www.medsi.co.jp/books/products/detail.php?product_id=3665)

----
#### 習熟度ややりたいこと別にご参考ください
- 塩基配列解析に関わる基礎知識について
    - [「塩基配列解析のためのデータベース・ウェブツールとCRISPRガイドRNA設計 @ AJACSこまち」(2016年8月)](https://doi.org/10.7875/togotv.2016.122)

- 遺伝子発現データを公共DBで検索・取得・解析する方法について
    - [「遺伝子発現DB・ウェブツールの使い方 応用・実践編」(2015年5月AJACS御茶ノ水)](https://togotv.dbcls.jp/ja/ajacs2015007.html)

- 文献検索のプロが教えるPubMedの使い方
    - [文献情報を用いたサービスを活用する @ AJACS越後 (2018年6月)](https://togotv.dbcls.jp/20180815.html)

- 次世代シーケンス(NGS)データの解析について
    - [【NGS】に関係する動画・講習会資料・新着論文レビュー](https://togotv.dbcls.jp/tags.html?tag=NGS)

- NGS解析について、さらにもっと基礎から応用までを深く学びたい方向け (それぞれ約50時間程度)
    - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース(2014年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
    - [「バイオインフォマティクス人材育成カリキュラム 次世代シークエンサ(NGS)ハンズオン講習会(2015年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00Yo0Cn0rcF23xof5hqCzGQb)
    - [NGSハンズオン講習会2016](https://www.youtube.com/watch?v=TSa1yPy_sdM&list=PL0uaKHgcG00ZNpICun17CEAFpV_5Q6GCA)
    - [NGSハンズオン講習会2017](https://www.youtube.com/watch?v=6Fzvl_I48tM&list=PL0uaKHgcG00YDmBXYWOgkmfeURjc8BZkk)
    - [上記の動画+講習会資料のまとめページ@統合TV](http://togotv.dbcls.jp/ja/tags.html?tag=NGS速習・ハンズオン)

----
## 学術論文を効率よく検索する
###  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/)
#### 泣く子も黙る文献・論文検索の総本山
 -  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) (パブメド) は、米国立医学図書館(National Library of Medicine: NLM)が運営している文献情報データベースです。
    - 1997年6月のサービス開始以来、2019年4月時点で5200件を超える学術誌を対象に、およそ 2,900万件超の文献情報を提供しています。
    - 2015年の一年だけで110万件超 (約3,000件/1日)の論文が追加され、その数はさらに増加しています。
    - 一日あたりの検索がおよそ250万件、160万人の利用者、830万件の書誌情報閲覧回数と、生命科学分野で最も利用されているウェブサービスの一つです。
- [PubMed Central (PMC)](https://www.ncbi.nlm.nih.gov/pmc/)は、書誌情報、アブストラクトに加えて全文が無料（オープンアクセス）で公開されている論文を収録・提供しています。
    - PMCの件数でおよそ 540 万件、論文誌のウェブサイトで全文が提供されているものも含めると600万件以上の論文で全文を読むことができます。
    - 最近では、研究予算配分機関の指定で、成果をオープンアクセス誌で公表することを義務付けていることもあるので、閲覧できる論文が増えてきています。

##### 論文を検索する

 1. Google検索で「PubMed」と検索します。
    1. トップに出てくる「Home - PubMed - NCBI」[https://www.ncbi.nlm.nih.gov/pubmed/](https://www.ncbi.nlm.nih.gov/pubmed/) をクリックします。あるいは、ウェブブラウザのアドレスバーに直接「pubmed.gov」と入力しても自動でリダイレクトされます。
 1. 検索窓にキーワードを入力し始めると、関連語がサジェストされます。
    1. [Hiromasa Ono](https://www.ncbi.nlm.nih.gov/pubmed/?term=Hiromasa+Ono) で検索してみます。
    1. ちなみに、検索窓に「All[filter]」と入力し検索すると、検索時点におけるPubMedに収載されている全論文数を調べることができます。
 1. 初期設定では、検索結果は、最新のものから順に表示されます。
    1. 最近、検索語との「Best Match」順に並び替える機能が実装されたため、現在は目立つようにハイライトされています。
    1. 画面左側には検索用のフィルタが用意されており、論文の種類や全文を購読できるか否か、出版日の指定、対象とする生物種などで絞り込むことができます。
    1. 画面右側には、検索語にヒットした論文の年度別統計値が棒グラフで示されており、マウスオーバーするとその件数が表示され、そのままクリックするとその年度で絞り込みができます。
 1. 検索結果一覧に「Free PMC Article」や「Free Article」の表示がある場合は、全文を読むことができるオープンアクセスの論文であることを示しています。
    1. 前者はPMCのウェブサイトで全文閲覧ができ、後者は論文誌のウェブサイトで全文閲覧ができます。
    1. PMCへのリンクをクリックすると、PMCが提供する様々な形式で全文を読むことができます。
        1. 論文PDFのダウンロードはもちろん可能です。
        1. 引用文献へのリンクが動的に表示されるなどウェブサイトでの表示に適したスタイルのほか、近年利用が増えているタブレット端末での表示に最適化された「PubReader」の機能が提供されています。

##### 自分の探している論文が見つからないときは検索式を見直す

 1. 検索結果が思ったように得られない、あるいは、数が多すぎて絞りきれない場合は、実際にどのような検索式でPubMed検索が行われているのかを調べて修正することができます。
 1. 検索結果一覧の右カラムにある「Search details」に入力されているのが実際に検索されている検索語です。
 1. たとえば、「iPS cells」でキーワード検索してみると、期待する「induced pluripotent stem cells」以外にも、多くの検索語が入力されていることがわかります。
 1. これは、PubMedが入力語を自動的に適切な単語に変換(Query Translation)しているためで、論文を効率的に検索するためには適切な検索式を与えることが重要です。
 1. 一番簡単にできることは、複合語の検索の場合に二重引用符(")で囲むことです。
    1. 一般的に、複合語で検索したほうがミスマッチする論文が減り、目的の論文を探しやすくなります。
 1. 検索効率化のためのもう一つの手段は、MeSH Termsを有効活用することが挙げられます。
    1. PubMedでは各論文にMeSH Termsが検索用の「タグ」のように付与されています。
        1. 「iPS cells」の検索語に対して「"induced pluripotent stem cells"[MeSH Terms]」が最初に変換されていることがわかります。このように、MeSH TermsはPubMed検索の中で重要な意味を持っています。
            1. MeSH Terms とは、
                1. MeSHは、Medical Subject Headings の略で、階層構造を持つ統制された概念・語彙集として主に医学関係の用語を整理したものです。語彙数は約2万9千ほどあり、毎年更新されています。PubMedに収録された全論文に対して専門のスタッフがMeSHタームを用いて注釈付けを行っています。


##### PubMedの検索結果を定点観測する

 1. 自分の興味関心に合った検索語(式)を作成することができたら、あとは、更新があったら通知するようにすると便利です。
 1. それらの自動化はRSS通知による方法とメールによる通知による方法の二種類が用意されています。
    1. RSS通知
        1. 検索語(式)を検索窓に入力した状態で、その下の「Create RSS」を押すとリンクURLが生成されます。更新情報を何件通知するかを設定することができ、最大で100件分まで指定可能です。生成されたリンクURLをRSSリーダーに登録して利用します。
            1. RSS(Really Simple Syndication)とはウェブサイトの要約や記事の見出しなどを配信するための仕組みです。
            1. 無料で使えるRSSリーダーとして、[Inoreader](https://jp.inoreader.com/) や [feedly](https://feedly.com) が有名です。
    1. メール通知
        1. まず先に「My NCBI」という個人別カスタマイズ機能にサインインします。
        1. ページ右上の「Sign in to NCBI」からサインインできます。サインインが済んでいれば、検索語(式)を検索窓に入力した状態で、「Create alert」をクリックするとその設定画面が表示されます。
        1. メールによる通知では、アラートの配信スケジュールや形式、数などを指定すれば、サインインに使用したメールアドレスにメールが届きます。
 1. キーワード検索以外にも自分の論文が引用された場合に通知するなど、いずれかの方法を目的に応じて使い分けると良いです。

##### 統合TVでPubMedの使いかたを学ぶ
 - PubMedで論文を検索する [https://doi.org/10.7875/togotv.2012.073](http://doi.org/10.7875/togotv.2012.073)
 - PMC (PubMedCentral) の使い方 2017　 [https://doi.org/10.7875/togotv.2017.122](https://doi.org/10.7875/togotv.2017.122)  
 - 文献情報を用いたサービスを活用する @ AJACS越後 [https://doi.org/10.7875/ajacs.2018.011](https://doi.org/10.7875/ajacs.2018.011)


----

### 新着論文レビュー
トップジャーナルに掲載された日本人を著者とする生命科学分野の論文について、論文の著者自身の執筆による日本語のレビューを、だれでも自由に閲覧・利用できるよう、いち早く公開するサービスです。  
( https://first.lifesciencedb.jp/ )

![FA1](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_FA1.png)
![FA2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_FA2.png)

#### ライフサイエンス 新着論文レビューの特徴

* Nature、Science、Cellなどに代表されるトップジャーナルに掲載された生命科学分野の原著論文のうち、筆頭著者が日本人である論文をいち早くとりあげます。論文の出版から1か月以内の公開を目標とし、遅くとも2か月以内には公開します。2010年9月のサービス開始からこれまでに約1,000本のレビューを公開しています。

##### 生命科学における専門分野が異なる人を対象

* 広く生命科学全般にかかわる教員・研究者および大学院生・学生を対象とし、専門の異なる読者にも論文の先進性およびおもしろさがわかるよう、結果・結論ばかりでなく、前提となる研究の経緯・バックグラウンド、将来の展望などもあわせて示すようにしています。

##### とにかく、わかりやすく読みやすい

* 原稿そのままではなく、生命科学を専門とする編集者がきちんとした編集作業を行っています。

##### コンテンツの自由な引用・転載・再利用

* サイエンスコミュニティの共有物として、クレジットの明記を条件に、転載・改変・再利用（営利目的での二次利用も含め）を自由に行えます。高解像度の図をJPEGファイルとしてダウンロードでき、講義や講演、論文などの著作物に自由に利用することができます。

#### 利用例

* 生命科学の加速度的な発展や研究分野の細分化が進むなか、最新の知見・情報を得る。
* 講義や講演、あるいは、論文などの著作物の資料とする。


#### 参考文献

* 統合TV「ライフサイエンス新着論文レビュー FirstAuthor's を使い倒す」[DOI: 10.7875/togotv.2011.037](https://doi.org/10.7875/togotv.2011.037)


### 領域融合レビュー
生命科学において注目される分野・学問領域における最新の研究成果について、第一線の研究者の執筆による日本語のレビューを、だれでも自由に閲覧・利用できるよう、無料で公開するサービスです。  
( https://leading.lifesciencedb.jp/ )

![LA1](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_LA1.png)
![LA2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_LA2.png)

#### ライフサイエンス 領域融合レビューの特徴

* 日本分子生物学会、日本蛋白質科学会、日本細胞生物学会、日本植物生理学会 との協力のもと、ある学問分野・領域を広く総合的にとりあげる比較的長いレビューを公開・出版するものです。執筆者・執筆テーマの選定は、それぞれの学会から推薦された編集委員により構成される編集委員会において行います。原稿は、編集委員会の指名した1名以上の査読者により査読をうけ、必要に応じ加筆あるいは改稿のうえ原稿受理とします。2012年9月のサービス開始からこれまでに約60本のレビューを公開しています。

##### 生命科学における専門分野が異なる人を対象

* 広く生命科学全般にかかわる教員・研究者および大学院生・学生を対象とし、専門の異なる読者にも論文の先進性およびおもしろさがわかるよう、結果・結論ばかりでなく、前提となる研究の経緯・バックグラウンド、将来の展望などもあわせて示すようにしています。

##### とにかく、わかりやすく読みやすい

* 原稿そのままではなく、生命科学を専門とする編集者がきちんとした編集作業を行っています。

##### コンテンツの自由な引用・転載・再利用

* サイエンスコミュニティの共有物として、クレジットの明記を条件に、転載・改変・再利用（営利目的での二次利用も含め）を自由に行えます。高解像度の図をJPEGファイルとしてダウンロードでき、講義や講演、論文などの著作物に自由に利用することができます。

#### 利用例

* 生命科学の加速度的な発展や研究分野の細分化が進むなか、最新の知見・情報を得る。
* 講義や講演、あるいは、論文などの著作物の資料とする。


#### 参考文献

* 統合TV「ライフサイエンス領域融合レビューLeadingAuthor'sを使い倒す」[DOI: 10.7875/togotv.2012.088](https://doi.org/10.7875/togotv.2012.088)

---

## 生命科学系の文献に頻出する英語表現を高速に検索する
### 逐次PubMed表現検索 inMeXes (インメクセズ)
生命科学系の文献（PubMedに含まれるタイトルとアブストラクト）に頻出する英語表現を、1文字の入力ごとに高速に再検索します。検索結果から用例や関連情報を容易に取得することができます。
(https://docman.dbcls.jp/im/)

![fig5](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_05.png)

![fig6](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_06.png)

#### inMeXesの特徴
##### 綴りに自信がなくても目的の英語表現を容易に検索

* 4文字以上の入力で、生命科学系の文献で実際に用いられている表現をPubMed/MEDLINEデータベースにおける頻度順に表示します。1文字の入力 を追加するごとに逐次的に文字列にマッチする表現を検索し直すので、目的とする表現をみつけやすくなっています。

##### 一度のクリックでマッチした表現の用例が閲覧可能

* 用例は、「ライフサイエンス辞書プロジェクト（京都大学）」が提供している共起表現リストや、「生命科学DB横断検索（開発：ライフサイエンス統合データ ベースセンター、サービス提供：バイオサイエンスデータベースセンター）」の文献・データベースリストなどで確認できます。

##### 検索結果をブックマークしてほかの利用者と共有できる

* 一度検索した表現の用例は、結果を再現しやすくするためにURL（Permalink）を動的に生成することができます。検索結果のブックマークや共有に便利です。

#### 利用例

* 英語で論文や記事を書く際に、よく使われる表現を確認する。
* 興味のある遺伝子や蛋白質に関する記述としてよく使われる表現を検索する。

#### 今後の開発予定

利用者のフィードバックなどを参考にしながら機能拡張、新規機能の追加を検討します。

#### 参考文献

統合TV「[inMeXesを使って文献に頻出する英語表現や関連語を高速に検索する 2018](https://togotv.dbcls.jp/20180126.html)」DOI: 10.7875/togotv.2018.026

---

## 生命科学分野の略語・展開形を検索する
### Allie (アリー): A Search Service for Abbreviation / Long Form
PubMed（米国立医学図書館が開発・維持している生物医学文献書誌情報データベース）を利用して、文献中に登場する略語とその正式名称の組およびその付随情報を検索します。
(https://allie.dbcls.jp/)

![fig7](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_07.png)
![fig8](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_08.png)
#### Allieの特徴

* PubMed収録文献のタイトルとアブストラクトに出現する略語とその正式名称の組について、略語と正式名称のいずれか一方、あるいは、正式名称の一部をクエリとする検索ができます。
* 日本語の対訳がある正式名称については、あわせて表示します。
* 検索結果の略語もしくは正式名称について、それらが出現する文献情報も取得できます。
* タイトルあるいはアブストラクト中に共起するほかの略語も検索結果から閲覧できます。
* 各種WebAPI(REST/SOAP/SPARQL)を備えているので、自分で作成したプログラムでAllieを呼び出すことができます。
* 略語と正式名称の組、および、その出現PubMed IDを収めたデータベースを、タブ区切りとResource Description Framework (RDF)の双方の形式で自由にダウンロードできます。

#### 利用例

* ある略語について、その正式名称を知る。
* ある略語が最初に文献に登場した時期を知る。
* 新たな略語をつくろうとしたとき、その略語がすでに存在しているかどうかを調べる。

#### 今後の開発予定

引き続き日本語訳の充実および月一度の定期更新を行います。

#### 参考文献

* Yamamoto, Y., Yamaguchi, A., Bono, H., Takagi T. (2011). Allie: a database and a search service of abbreviations and long forms. Database, 2011:bar03.
* 統合TV「[Allieを使って略語の正式名称を検索する 2017](https://togotv.dbcls.jp/20171025.html)」DOI: 10.7875/togotv.2017.104

---

## 類似したテキストの差分を検索・表示する
### テキスト比較ツール difff《ﾃﾞｭﾌﾌ》
https://difff.jp/

![fig9](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_09.png)

#### difff(ﾃﾞｭﾌﾌ)の特徴
* diffコマンドを使った比較結果をWeb上に表示するツール
* テキストボックスに比較したい文章をコピペしてボタンを押すだけで2つの文章でどこが変更されたのか差分の確認ができる
* 日本語のテキストも対応
* Word文章はもちろんソースコード、 遺伝子リストなどの比較も可能
* [某問題で活躍](http://www.itmedia.co.jp/news/articles/1403/12/news121.html)

#### 参考文献
* 統合TV「[difff《デュフフ》を使って文章の変更箇所を調べる](https://togotv.dbcls.jp/20130828.html)」DOI: 10.7875/togotv.2013.056

---
## NCBI (National Center for Biotechnology Information)
### [NCBI Databases](https://www.ncbi.nlm.nih.gov/search/?term=)
- 米国 国立生物工学情報センター (National Center for Biotechnology Information: NCBI)
- 文献、遺伝子、遺伝学、タンパク質、ゲノム、化合物といったあらゆるデータベースがあります。
![NCBI top](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_NCBI.png)
- [【NCBI】に関係する統合TV動画](https://togotv.dbcls.jp/tags.html?tag=NCBI)
### NCBIで 遺伝子 を調べる
- <details><summary>そもそも遺伝子(gene)ってなに?　ゲノム(genome)とDNAの違いは?</summary>[遺伝子とゲノム](https://www.ddbj.nig.ac.jp/column/genegenome.html)(国立遺伝学研究所 生命情報・DDBJセンター ウェブサイト)</details>
- ALDH2 について調べる
  - [エタノール(エチルアルコール)](https://pubchem.ncbi.nlm.nih.gov/compound/702) の代謝産物である[アセトアルデヒド](https://pubchem.ncbi.nlm.nih.gov/compound/177)をさらに分解する、アセトアルデヒドデヒドロゲナーゼという酵素をコードしている遺伝子で、ヒトでは12番染色体に存在する


1. NCBI のトップページにALDH2と入れてみる
  - ![NCBI search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_1.png)
1. 遺伝子について調べたいので、[Gene](https://www.ncbi.nlm.nih.gov/gene/) を選びます
1. ALDH2 という名前の付いた遺伝子が様々な生物種込みで検索されます
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_3.png)
1. ヒトのALDH2を調べたいので、ALDH2 homo sapiens　としてみるとどう変わるでしょうか
1. 一番上にでてきた **ALDH2 ID:217** というのがお目当てのもののようなのでクリックします
1. NCBI Gene データベースにおける **ヒトのALHD2 のページ** [https://www.ncbi.nlm.nih.gov/gene/217](https://www.ncbi.nlm.nih.gov/gene/217) が表示されます
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_4.png)
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_5.png)
  - ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_6.png)

#### 遺伝子のID
- Accession Number
- RefSeq ID
- (NCBI) Gene ID
- Gene Symbol(遺伝子名)

##### Accession Number
- GenBank/ENA/DDBJ 国際塩基配列データベースに登録された塩基配列のID
  - 俗にGenBankのAccession番号と呼ばれることもあるが正確ではない。
- **A12345** や **AB123456** のような形をしている
  - アルファベットの割り当てについては、[DDBJのPrefix Letter List](https://www.ddbj.nig.ac.jp/prefix-e.html)に詳細がある
- A12345**.1**のようにバージョンを表示
  - UTRが延長されたりエラーが修正されて、A12345**.2**のようにアップデートされる

##### RefSeq ID
- 国際塩基配列データベースに登録された配列を基に transcriptごと(塩基配列ごと)に1個登録→RefSeqデータベース
  - 遺伝子の百科事典のようなもの
- 選択的スプライシングで生じるvariantには別々のIDが付与されている
- NM_012345.6 の形式をしている
  - 実用上はAccession番号の一種として扱うことができる
- ![Gene search for ALDH2](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_ALDH2_7.png)

##### (NCBI) Gene ID, Gene Symbol
- 遺伝子ごとに付与される番号と遺伝子

|生物種|慣用名(description)|Gene Symbol|Gene ID|
|:--|:--|:--|:--|
|ヒト|aldehyde dehydrogenase 2 family member|ALDH2|217|
|マウス|aldehyde dehydrogenase 2, mitochondrial|Aldh2|11669|
|アフリカツメガエル|aldehyde dehydrogenase 2 family member |aldh2|448267|

- Symbolは慣用名と一致しないこともある
  - 山中因子の一つで有名なOCT4は、[POU5F1](https://www.ncbi.nlm.nih.gov/gene/5460)がGene Symbol
- 別の生物種で同一のSymbolがついていることもある
- Gene ID は、生物種と遺伝子を特定できる

#### 塩基配列から遺伝子を探す
- NCBI BLAST
  - [NCBI BLASTの使い方 〜基本編〜 2017](https://togotv.dbcls.jp/20170321.html)
- UCSC BLAT
  - [高速アラインメントツールBLATをプライマー設計支援ツールとして使う 2017](https://togotv.dbcls.jp/20171001.html)


---

## 遺伝子やゲノム配列を高速に検索する
### 統合遺伝子検索GGRNA
さまざまなキーワードから遺伝子を簡単に検索することのできる遺伝子検索エンジンです。  
塩基配列やアミノ酸配列から高速に遺伝子を検索することもできます。  
GGRNA： https://GGRNA.dbcls.jp/

![Fig-1](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSServices_GGRNA.png)

#### GGRNAの特徴

* NCBI RefSeqに登録された転写産物の情報を高速に全文検索します。遺伝子名や各種のID、タンパク質の機能など、あらゆるキーワードから簡単に遺伝子を検索できます。
* 塩基配列の検索では、N, R, Yなどのあいまいな塩基を含むパターンも検索できます。
* ヒト、マウス、ラット、ニワトリ、ツメガエル、ゼブラフィッシュ、ホヤ、ショウジョウバエ、線虫、イネ、シロイヌナズナ、出芽酵母、分裂酵母を含め、RefSeqに収録されている全ての生物種に対応しています。

#### 利用例

* ある遺伝子について調べたくなったら、まずはGGRNAで検索。
* 論文の図中に登場する塩基配列やアミノ酸配列から即座に遺伝子を検索。たとえばPCRのプライマー、プローブ、siRNAの配列を検索して標的遺伝子および位置をチェック。
* マイクロアレイのプローブIDを塩基配列に変換して遺伝子を検索。
* 短いアミノ酸配列のモチーフを検索。

#### 参考文献

* Naito Y, Bono H. GGRNA: an ultrafast, transcript-oriented search engine for genes and transcripts. Nucleic Acids Res. 40, W592-W596 (2012) DOI: [10.1093/nar/gks448](https://doi.org/10.1093/nar/gks448)
* 内藤雄樹, 坊農秀雅「統合遺伝子検索GGRNA：遺伝子をGoogleのように検索できるウェブサーバ」ライフサイエンス 新着論文レビュー 2012年5月28日 DOI: [10.7875/first.author.2012.163](https://doi.org/10.7875/first.author.2012.163)
* 統合TV「GGRNAで遺伝子をGoogleのように検索する」 DOI: [10.7875/togotv.2012.003](https://doi.org/10.7875/togotv.2012.003)

### 高速塩基配列検索GGGenome
ゲノムや転写産物等の塩基配列を高速に検索するツールです。  
GGGenome： https://GGGenome.dbcls.jp/

![Fig-1](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSServices_GGGenome.png)

#### GGGenomeの特徴

* BLASTやBLATでは検索の難しい20塩基以下の短い配列の検索が得意です。
* ミスマッチやギャップを含む塩基配列もすばやく検索できます。
* ゲノムの検索は、主要なモデル生物を含む350以上の生物種に対応しています。
* 転写産物の検索は、NCBI RefSeqに収録された全生物種のmRNA、ncRNAを検索できます。
* 検索結果をさまざまなフォーマットで取得することができます。

#### REST APIの提供

```
URI: http[s]://GGGenome.dbcls.jp/db/k/strand/sequence[.format][.download]
```

* `db` : 検索対象データベース　例） ヒトゲノム`hg38`, マウスゲノム`mm10`, RefSeq転写産物`refseq` など
* `k` : 許容するミスマッチまたは挿入欠失の数。省略時は0
* `strand` : `+`,`plus` または `-`,`minus` で特定方向のみ検索
* `sequence` : 検索する塩基配列
* `format` : `html`,`txt`,`csv`,`bed`,`gff`,`json` (省略時は`html`)
* `download` : 検索結果をファイルとしてダウンロード (`txt`,`csv`,`bed`,`gff`,`json`のみ)

**例1：** https://GGGenome.dbcls.jp/hg38/1/TTCATTGACAACATT

* ヒトゲノム `hg38` に対して
* `1` 塩基のミスマッチまたは挿入欠失まで許容して
* `TTCATTGACAACATT` を検索し
* `html` (省略時のデフォルト) で結果を返す

**例2：** https://GGGenome.dbcls.jp/refseq/+/TTCATTGACAACATT.txt

* RefSeq complete RNA `refseq` の最新版に対して
* ミスマッチや挿入欠失を許容せず (省略時のデフォルト)
* 検索方向を `+` 方向に限定し
* `TTCATTGACAACATT` を検索し
* タブ区切りテキスト `txt` で結果を返す

##### 応用例
* [GGGenome《ゲゲゲノム》を使って高速塩基配列検索をする 2018](https://togotv.dbcls.jp/20181026.html)
  - Google スプレッドシート(Spreadsheet)の機能を利用し、プライマー配列情報を半自動的かつ効率的に整理する方法(~4:05)

#### 参考文献

* 統合TV「高速配列検索GGGenome《ゲゲゲノム》の使い方」 DOI: [10.7875/togotv.2013.071](https://doi.org/10.7875/togotv.2013.071)
* 統合TV「GGGenome 《ゲゲゲノム》 で転写因子結合サイトを検索してゲノムブラウザに表示する」 DOI: [10.7875/togotv.2015.067](https://doi.org/10.7875/togotv.2015.067)

### CRISPRdirect
入力した塩基配列に対してCRISPR-Cas9システムのガイドRNAを設計することができるツールです。  
CRISPRdirect： https://crispr.dbcls.jp/

![Fig-1](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSServices_CRISPRdirect.png)

#### CRISPRdirectの特徴

* 目的以外の部位で誤ってゲノム編集が起こる「オフターゲット効果」の少ないガイドRNAを効率よく設計できます。
* 主要なモデル生物に加え、ゲノム配列が公表されている350以上の生物種に対応しています。

#### 使い方

* 任意の塩基配列、アクセッション番号、またはゲノムの座標を入力して [design] ボタンをクリック。
* 標的部位の候補が表示されます。緑色にハイライト表示されたものが、特異性の高いガイドRNAを設計できる部位です。
* 表のなかの [detail] をクリックすると、オフターゲット候補部位が表示されます。ガイドRNAとゲノムとのあいだにミスマッチや挿入・欠失がある場合についても表示することが可能です。

#### 今後の開発予定

* データを定期的に更新し、ユーザからのフィードバックに応じて機能を改善していく予定です。

#### 関連プロジェクト
* siDirect (http://siDirect.RNAi.jp/)  
  哺乳類細胞で活性が高く標的遺伝子に特異的なsiRNAの設計ウェブサーバ

#### 参考文献

* Naito Y, Hino K, Bono H, Ui-Tei K. CRISPRdirect: software for designing CRISPR/Cas guide RNA with reduced off-target sites. Bioinformatics 31, 1120-1123 (2015) DOI: [10.1093/bioinformatics/btu743](https://doi.org/10.1093/bioinformatics/btu743)
* 統合TV「CRISPRdirectを使ってCRISPR/Cas法のガイドRNA配列を設計する」 DOI: [10.7875/togotv.2014.025](https://doi.org/10.7875/togotv.2014.025)

---

## 公共データベースから利用可能な遺伝子発現データを解析する
### RefEx
RefEx（Reference Expression dataset）は、遺伝子発現解析の基準となる各遺伝子の遺伝子発現量を簡単に検索、閲覧できるウェブツールです。 (https://refex.dbcls.jp/)  

![Fig-1](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-1_180523.png)  

![Fig-2](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-2_180523.png)

#### RefExの特徴
##### 正常組織・細胞等の遺伝子発現状況が ひと目でわかる
* 複数の遺伝子発現計測手法によって得られた哺乳類の正常組織、細胞等における遺伝子発現データを収集し並列に表現することによって、各組織における遺伝子発現状況を計測手法間の差異とともに直感的に比較できることが特長です。RefExを利用することで、研究者は研究対象とする遺伝子が平常時にどの組織、細胞でどの程度発現しているのかについて、自ら実験をすることなく確認することができます。また、研究者がしばしば遭遇する馴染みのない遺伝子について、一般的には個別の研究論文における実験データや記述などからそれらの生物学的特徴を類推したりしますが、RefExでは実験デザインに左右されない大規模かつ網羅的な測定データから研究者自身の目でそれらを簡単に確認することができます。さらに、研究者の用意した複数の遺伝子IDについて一括で検索できる機能を備えているほか、リスト機能を用いて遺伝子の詳細データを並列に比較することができるため、遺伝子発現解析などで見出された遺伝子群の関係性を知るためのツールとしても有用です。
##### 調べたい遺伝子を より探しやすく よりわかりやすく
* もっとも基本的なキーワード·遺伝子名検索では文字を入力する度に検索語の候補が提示されるので、それらから選択することで容易にキーワード入力を行うことができます。また、「転写因子」や「Gタンパク質共役受容体」、「2番染色体」などのように、ある分類に属する遺伝子群についてまとめて検索·比較できるよう整理されています。さらに、さまざまな実験における比較対照などに用いられる『組織特異的遺伝子』を測定データから独自に算出し、組織ごとに一覧することができます。Advanced searchでは、複雑な検索条件を一度に指定することが可能であり、あらかじめID情報などが手元にある場合には、目的とするデータに簡単に行き着くことができます。
##### 直感的な可視化で 新たな知識発見・仮説構築を
* 検索結果一覧および個別の遺伝子の詳細情報ページでは、組織間の比較と測定手法間（EST、GeneChip、CAGE、RNA-seq）の比較を両立させた相対発現量が棒グラフで示されるとともに人体の3Dモデルである[BodyParts3D/Anatomography](http://lifesciencedb.jp/bp3d/)に発現量を反映させたヒートマップが表示されます。またリスト機能を使えば、検索結果の個別の遺伝子について一時的に保存しておくことができます。リストに追加した遺伝子は、最大でその3つについて、40分類の組織·臓器における発現データを比較しながら、遺伝子に付与された機能に関する注釈情報（Gene Ontology他）を見比べることができます。これらの機能は、新たな知識発見あるいは仮説の構築をサポートします。詳細情報ページに記載された種々のIDには、それぞれRefExの内部リンクやオリジナルのデータベースサイトへの外部リンクが貼られており、同じ分類に属する遺伝子を再検索したり、RefEx自体を遺伝子検索の起点とすることもできます。
##### 再利用可能で有用なパブリックデータの活用例
* RefExが提供するすべてのデータは、クリエイティブ·コモンズライセンスのもとで、オープンデータとして自由にダウンロードおよび再利用することができます。検索結果一覧や詳細情報ページのデータはいずれもダウンロードすることが可能で、研究者自身のデータと参照することも、それらを使った再解析も自由に行うことができます。また、外部の研究データレポジトリ「figshare」にも全てのデータがDOI付きで公開されています [(https://doi.org/10.6084/m9.figshare.c.3812815)](https://doi.org/10.6084/m9.figshare.c.3812815)。 さらに、ソフトウェア開発プロジェクトのための共有ウェブサービス「GitHub」上にも、公開データの再解析に用いたプログラムやドキュメントを整理しており、RefExで提供する再解析データについてある一定の評価品質および再現性を担保しています [(https://github.com/dbcls/RefEx)](https://github.com/dbcls/RefEx)。RefExは生命科学データの共有および再利用の活用例のひとつであり、データ駆動型研究のためのデータセット、ウェブツールとしてだれでも自由に使うことができます。

#### 利用例
* 正常組織や細胞株における遺伝子発現データを調べる｡
* 測定手法による遺伝子発現量の違いを比較する｡
* 組織特異的に発現する遺伝子をワンタッチで検索可能｡
* 遺伝子発現解析などで見出された不詳な遺伝子群の機能および関係性を調べる｡
![fig-3'](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-3_180523.png)

#### 今後の開発予定

* 今後は、世界各地で進められている遺伝子発現に関する大規模研究プロジェクト（FANTOM、GTExなど）を中心に、高精度かつ広範囲な遺伝子発現データを収集し、統合することによって、より有用性の高い参照データを作成する予定です。また、それらの参照データを簡単に検索したり、発現データ同士を詳細に比較したりすることを可能にする直感的なウェブインターフェースの開発を進めています。

#### 参考文献

* Hiromasa Ono, Osamu Ogasawara, Kosaku Okubo, Hidemasa Bono
    **RefEx, a reference gene expression dataset as a web tool for the functional analysis of genes**
    Scientific Data, 4:170105
    [DOI: 10.1038/sdata.2017.105](https://doi.org/10.1038/sdata.2017.105)
* 川路 英哉、粕川 雄也、坊農 秀雅、小野 浩雅 「FANTOM5データを誰でも活用できる形に」 Scientific Data誌著者インタビュー (平成29年8月29日)
    https://www.natureasia.com/ja-jp/scientificdata/papers-from-japan/fantom5
* 小野 浩雅・坊農 秀雅 「遺伝子発現解析の基準となるデータを快適に検索できるウェブツールRefEx」 ライフサイエンス新着論文レビュー (平成29年9月5日)
    [DOI: 10.7875/first.author.2017.093](https://doi.org/10.7875/first.author.2017.093)
* 統合TV 「RefExの使い方」[DOI: 10.7875/togotv.2014.009](https://doi.org/10.7875/togotv.2014.009)


### 【実習1】RefExを使って、組織特異的遺伝子を検索する
- 【復習用】[RefExの使い方](https://doi.org/10.7875/togotv.2014.009)

1. https://refex.dbcls.jp/ を開きます。
2. 画面中央の「組織特異的に発現する遺伝子を見る」の臓器アイコンにカーソルを合わせると、更に詳細な部位のアイコンが出るので、調べたい臓器（例として肝臓）をクリックします。  
  - ![http://gyazo.com/35c8f38340753e8f433cb8c4d8fd812b](http://i.gyazo.com/35c8f38340753e8f433cb8c4d8fd812b.jpg)

3. 検索結果一覧が表示されます。検索結果一覧では、「ソート項目の切り替え」や「絞り込み検索」、「リストへの追加」ができます。(手順11以降で解説します。)
4. 各遺伝子の青字の部分（例 [fibrinogen alpha chain](https://refex.dbcls.jp/gene_info.php?lang=ja&db=human&geneID=2243&refseq=NM_000508&unigene=Hs.351593&probe=205649_s_at))をクリックすると詳細情報を閲覧できます。
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
 - [RefEx用に整理したサンプル情報一覧](https://bit.ly/fantom5cagehuman)も閲覧可能です。
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
 - [肝臓特異的遺伝子の検索結果一覧](https://refex.dbcls.jp/genelist.php?lang=ja&db=human&roku_valid=1&rk[31]=31&order_key=score)に移動して、3つの遺伝子を「リストに追加」してみましょう。
 - 追加した件数は「リストを見る」の横に表示されます。
 - 「リストを見る」をクリックするとリストに移動します。
 - 『並べて表示する』にチェックを入れて、「遺伝子を並べて表示」をクリックします。
 - 遺伝子発現データやGeneOntology情報を並列に比較することで見えてくる「違い」はなんでしょうか。その違いからどういうことが推測できるでしょうか。
 - ![並列比較1](http://i.gyazo.com/ba11e4c7c38a4e78d3a64d7b8b6efee8.jpg)
 - ![並列比較2](http://i.gyazo.com/3f2f9e5cbf135a2c298ae164d6360302.jpg)
14. 自分の研究テーマに関連する、また興味のある遺伝子について検索してみましょう。

----

### ChIP-Atlas
ChIP-Atlasは、論文などで報告された ChIP-seq データを閲覧し、利活用するためのウェブサービスです。データ処理の知識やスキルがない方でも簡単に利用できます。データソースは、公開 NGS データレポジトリ (NCBI, EMBL-EBI, DDBJ) に登録されたほぼ全ての ChIP-seq データです。ChIP-Atlas は、九州大学大学院医学研究院 発生再生学分野 (http://www.dev.med.kyushu-u.ac.jp) と DBCLS が共同で開発しています。  
 (https://chip-atlas.org/)

![fig10](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_10.png)

![fig11](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_11.png)

#### ChIP-Atlasの機能
##### Peak Browser
* 既報の ChIP-seq データをまとめて閲覧し、何がどこに結合しているかが一目でわかります。Integrative Genomics Viewer (IGV) によりスムーズなブラウジングが可能で、興味の遺伝子のシス調節領域を予測したり、それを制御する転写因子の予測ができます。
  * [ChIP\-Atlasを使って既報のChIP\-seqデータをまとめて閲覧する 〜Peak Browserの使い方〜](https://togotv.dbcls.jp/20180123.html)
##### Target Genes
* 興味のある転写因子を選択し、その標的遺伝子候補を検索できます。
  * 統合TV「[ChIP\-Atlasを使って興味のある転写因子を選択しその標的遺伝子候補を検索する 〜Target Genesの使い方〜](https://togotv.dbcls.jp/20180124.html)」
##### Colocalization
* 興味のある転写因子を選択し、それとゲノム上で共局在する転写因子候補を検索できます。
  * 統合TV「[ChIP\-Atlasを使って共局在タンパク質を探す 〜Colocalizationの使い方〜](https://togotv.dbcls.jp/20180128.html)」
##### Enrichment Analysis
* ユーザデータを受け付け、既存データとの比較解析をおこないます。たとえば、興味のある遺伝子リストを submit すると、それらをまとめて制御する転写因子候補が返されます。ほかにも BED 形式のファイルや、シーケンスモチーフを submit すると、それらに enrichment する転写因子群が返されます。


#### 利用例
* 論文として発表された ChIP-Seq データを閲覧したい
* 興味のあるゲノム領域における、転写因子や修飾ヒストンの分布を知りたい
* 興味のある転写因子の下流遺伝子や、複合体形成パートナーを知りたい
自身の研究データと公開 ChIP-seq データを用いて比較解析をおこないたい
#### 参考文献
- Source code and documentation    
  - https://github.com/inutano/chip-atlas
- Preprint
  - Shinya Oki, Tazro Ohta, et al. Integrative analysis of transcription factor occupancy at enhancers and disease risk loci in noncoding genomic regions. bioRxiv 262899; doi: https://doi.org/10.1101/262899
- Database
  - Oki, S; Ohta, T (2015): ChIP-Atlas. http://dx.doi.org/10.18908/lsdba.nbdc01558-000

### 【実習2】ChIP-Atlasのin silico ChIP を使って、興味ある遺伝子リストを制御する可能性の高い転写因子を調べる
* 「発現差のあった遺伝子リスト」を持っている想定で、それらの遺伝子に結合しうる、あるいは上流でそれらの遺伝子の発現を制御する可能性がある転写因子を検索する
* 使用するデータ
  - [List_of_GeneSymbol_txt](https://raw.githubusercontent.com/hiromasaono/training/master/180901_seikawakate/180901_List_of_GeneSymbol.txt)
    - ある「興味ある遺伝子リスト」をGeneSymbolにID変換したデータ。
    - これを使って、もともとどういう遺伝子リストだったかを考察します。
  - ChIP-Atlas では、遺伝子IDとしてGeneSymbolのみを受け付けているので、それ以外のIDで遺伝子リストを持っている場合は、適宜変換が必要。
    - ID変換はいろいろなツールがあるが、今回は[HGNC BioMart](https://biomart.genenames.org/)を利用する。
      - HGNC(The HUGO Gene Nomenclature Committee)はヒトのGeneSymbolを認定・管理している機関。
      - [DAVID(Database for Annotation, Visualization and Integrated Discovery)
   ](https://david.ncifcrf.gov/)のGene ID Conversion Toolも便利。([使い方動画](https://youtu.be/4f1t1ma9IRc?t=4m5s))

1. [ChIP\-Atlas \- Enrichment Analysis](https://chip-atlas.org/enrichment_analysis)にアクセスする
2. 下図のようにオプションを設定する
![fig12](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_12.png)
3. submit すると遺伝研スパコンへクエリが飛ぶ(ので、講義中は見てるだけにしてください)
4. submit したあとの画面
![fig13](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_13.png)
5. 計算が終わるまで待つ
![fig14](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_14.png)
6. 計算が終わると、「Result URL」が有効になる
  - 今回の例では、 http://ddbj.nig.ac.jp/wabi/chipatlas/wabi_chipatlas_2018-0606-1701-36-865-010614?info=result&format=html
7. 結果の解釈をする
  - 今回は、どういう「興味ある遺伝子リスト」をクエリとしたか考察してみましょう。
  - 結果の見方としては、「p-valueが低く、Overlaps/My dataが多く、Fold Enrichmentが高い」転写因子がたくさんヒットしてくると入力した遺伝子群をまとめて制御する、マスター転写因子を抽出できている確度が高い

8. [答え合わせ](https://github.com/hiromasaono/training/blob/master/180901_seikawakate/180901_ChIP-Atlas_answer.md)


## まとめ
- つまみ食い的ではありますが、通り一遍の今日から使える便利な生命科学系公共データベース・ウェブツールを学びました。
- 一生モノのデータベース、ウェブツールの使いこなし術を持ち帰ってください。
- 顕微鏡 や 実験試薬 などと同じ「道具(ツール)」
- 便利な「道具」を知って、その使い方が分かれば、あとは情報分析力と想像力の勝負。
  - 正面からしか見られなかったものが横や後ろやナナメから見ることができて初めて気づくことがあるかもしれません。
- 仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化していきましょう。
- データベースやウェブツールで困ったら、「統合TV」でまず探して・見てみる
- 研究に役立ったら、ぜひ引用・クレジットを!
  - DBCLSの提供するサービス(あるいはそれ以外でも)が、あなたの研究に役立ったら、どんなに些細な事でもぜひ引用(論文、URL等)してください。DBCLSの活動は、提供するサービスがどのくらい活用されたかについて主に引用数などで評価されており、利用者の方の積極的なサポートが必要不可欠です!!
  - [NBDC関連サービスの活用に関する情報提供フォーム](https://form.jst.go.jp/enquetes/nbdcexamples)
