# これから研究室に入る初学者のための便利な生命科学系公共データベースとバイオインフォマティクスツールの使いこなし演習
## [http://bit.ly/202206_NUBS](https://bit.ly/202206_NUBS)

大学共同利用機関法人 情報・システム研究機構  
データサイエンス共同利用基盤施設  
[ライフサイエンス統合データベースセンター (DBCLS)](https://dbcls.rois.ac.jp/)   
小野 浩雅 ([Twitter@h_ono](https://twitter.com/h_ono), [個人サイト](https://sites.google.com/dbcls.rois.ac.jp/hono/))  
hono@dbcls.rois.ac.jp  

2022年6月7日-7月5日(全5回・毎週火曜日4限（14:40-16:10))  
日本大学 生物資源学部 応用生物科学科 3年次開講科目「生命情報科学（必修）」

----

これは、2022年度 日本大学 生物資源学部 応用生物科学科 3年次開講科目「生命情報科学（必修）」の小野担当回の講習資料です。 
© 2022 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

----

## 概要

ヒトゲノム計画が完了してから15年(実は、つい最近まで完全には解読されていなかった - [ヒトゲノム計画とヒトゲノム完全解読](https://www.jstage.jst.go.jp/article/jsbibr/3/1/3_jsbibr.2022.primer2/_html/-char/ja))がたち、今や技術革新により日々膨大なデータが産み出され、それらは様々なデータベースに登録され、その多くは公開される時代となっています。そして、生命科学研究を効率よく進めるためには、これらのデータをいかに有効活用するかが鍵になっています。  
そこで、全5回の講義では、これから研究室に所属して研究を始める皆さんを対象に、誰でも自由に使える便利な生命科学系のデータベースやバイオインフォマティクスツールをご自分のコンピュータを使ったハンズオン形式で紹介します。
生命科学系公共データベースとバイオインフォマティクスツールは、仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化するための便利な「道具」です。ぜひご自身の手で「使い倒し」てみてください。これから始まる研究生活の中で役に立つこと請け合いです。

----
## 自己紹介
- 小野 浩雅(おの ひろまさ)([reseachmap](https://researchmap.jp/hiromasaono/))  
  - [TogoTV](https://togotv.dbcls.jp/)の運営・編集者
  - [RefEx](https://refex.dbcls.jp/)の開発者
    - 遺伝子発現解析の基準となる各遺伝子の遺伝子発現量を簡単に検索、閲覧できるウェブツール
  - [TogoID](https://togoid.dbcls.jp/)
    - 生命科学系データベース間のつながりを探索的に確認しながらID変換を行うことができるウェブツール   
  - [Twitter@h_ono](https://twitter.com/h_ono)

----

## 講義の流れ
今回の講義(全5回)では、お手元のコンピュータを使って以下の内容について説明します。

- [【第8回】研究現場で頻繁に使われるデータベースやツールを知る](#第8回研究現場で頻繁に使われるデータベースやツールを知る)
  - 統合TV
- [【第9回】学術論文を効率的に検索したり、論文執筆を支援するデータベースやツール](#第9回学術論文を効率的に検索したり論文執筆を支援するデータベースやツール)
    - PubMed
  - 生命科学系の文献に頻出する英語表現を高速に検索する
    - inMeXes
  - 生命科学分野の略語・展開形を検索する
    - Allie
  - 類似したテキストの差分を検索・表示する
    - difff(ﾃﾞｭﾌﾌ)
- 【第10回】生命科学分野の様々なデータベース
    - NCBI
  - 遺伝子やゲノム配列を高速に検索する
    - GGRNA
    - GGGenome
    - CRISPRdirect
- 【第11回】ゲノムブラウザ
  - Ensembl Genome Browser
  - UCSC Genome browser   
- 【第12回】公共データベースから利用可能な遺伝子発現データを解析する
    - RefEx
      - 【実習】RefExを使って、組織特異的遺伝子を検索する
    - DAVID
      - 【実習】DAVIDを用いて、遺伝子発現データの結果を生物学的に解釈する

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
# 【第8回】研究現場で頻繁に使われるデータベースやツールを知る
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
- 1,950本を超える動画が公開されており、2,300,000回以上 再生(2022年2月末現在)
- コロナ禍の自粛時に過去最高の視聴数
- YouTubeのチャンネル登録をすると新規公開の通知が来て便利です

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220323_02.jpg)

---
# 個別動画ページ
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_01.png)
- 見どころダイジェスト
  - YouTubeの埋め込みプレーヤなので、おなじみの操作感
  - 動画の概要を示す「見出し」から視聴箇所に移動可能
  - 動画ファイルはダウンロード可能
- 各動画には、[DOI](https://ja.wikipedia.org/wiki/デジタルオブジェクト識別子) (Digital Object Identifier) が付与
  - 恒久的な URL として利用可能
  - e-learning教材として日本初

---
# [スキル別コース](https://togotv.dbcls.jp/courses.html)
- ある目的に対して、「この順で動画をみていくと、こういうスキルを獲得できる」というような体系的な動画リスト集
![bg right:50% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_02.png)
---

# ラボの新人がまずマスターしたいデータベース・ウェブツール(2020年4月)
- 研究室に入ってきた新人が必ず知っておくべき「論文の効率的な検索方法」、「研究発表資料の作成に必要なパワーポイントの図形描画機能」、「Google各種サービスを使って研究生活を効率化する」という3つのテーマに関する10本の動画を紹介しています
- https://biosciencedbc.jp/blog/20200511-01.html
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_03.png)

---
# 現在のラインナップ例 (今後さらに充実させていきます)
- [文献の検索や管理、情報収集に役立つツール](https://togotv.dbcls.jp/course.html?id=PL5409971734873D19)
- [ゲノムブラウザを使ってゲノム配列に関連する情報を検索・取得・可視化する](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00bs1Yno9jCCLqVntyzVPqGT)
- [公共の遺伝子発現データの検索や解析を行う](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00YDVET14wC0-GhpI5l3y8T-)
- [疾患に関連する変異や遺伝子発現の情報を調べる](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00a1DeTTRteZSWzmpDTEImAK)
- [図表を作成する](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00aFMd_yWI0xuzROpPWi7nSb)
- [文章の執筆に役立つツール](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00Y4Nuo6g08Ql3CsCefTvB9H)


---
# 講演・講習会
- キーワードから、「講演」や「講習会」を簡単に検索可能
- 受講生の復習のみならず、初学者の学習教材として活用できます

![bg right:50% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_04.png)

---
# 塩基配列解析に関わる基礎知識(遺伝子IDとそのデータベース)とゲノム編集について
  - [塩基配列解析のためのデータベース・ウェブツール @ AJACSオンライン2](https://togotv.dbcls.jp/20201125.html)
     - [CRISPRdirect](https://crispr.dbcls.jp/)の開発者が自ら解説
       - 入力した塩基配列に対してCRISPR-Cas9システムのガイドRNAを設計することができるツール
  - [ウェブツールを使ってゲノム編集の標的サイトを検索する @ AJACSオンライン8](https://togotv.dbcls.jp/20210831.html)
    - 適切なゲノム編集を行うための標的検索とその考え方について学びます。また、さまざまな目的に特化した標的選定やゲノム編集後の解析に活用できるツールについても紹介
---
# 次世代シーケンス(NGS)データ解析に必要な基礎知識とリテラシーを学ぶ
  - [NGSデータから新たな知識を導出するためのデータ解析リテラシー @ AJACS浜松](https://togotv.dbcls.jp/20180120.html)
    - NGSデータを解析するための基礎的な考え方・知識と、データ解析プロセスをどう設計・実践していくかの技術を学びます。ソフトウェアの使い方の詳細な解説よりも、実験系研究者が独学していくために必要なことに焦点を絞っています。
    - 講義資料: [NGSデータから新たな知識を導出するためのデータ解析リテラシー](https://github.com/AJACS-training/AJACS68/blob/master/05_ozaki/README.md)

---
# NGS解析について、さらにもっと基礎から応用までを深く学びたい方向け (それぞれ約10-50時間程度)
  - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース(2014年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
  - [「バイオインフォマティクス人材育成カリキュラム 次世代シークエンサ(NGS)ハンズオン講習会(2015年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00Yo0Cn0rcF23xof5hqCzGQb)
  - [NGSハンズオン講習会2016](https://www.youtube.com/watch?v=TSa1yPy_sdM&list=PL0uaKHgcG00ZNpICun17CEAFpV_5Q6GCA)
  - [NGSハンズオン講習会2017](https://www.youtube.com/watch?v=6Fzvl_I48tM&list=PL0uaKHgcG00YDmBXYWOgkmfeURjc8BZkk)
  - [先進ゲノム支援\(PAGS\)、DDBJ、DBCLS合同情報解析講習会\(2019\)](https://www.youtube.com/watch?v=VjZIQuWXPu8&list=PL0uaKHgcG00afJqVErwNQariGDKArJtB8)

---
# 画像を探す (Togo picture gallery)
- [「画像を探す」](https://togotv.dbcls.jp/pics.html)
- 生命科学分野のイラスト(約1,000本)が、誰でも自由に利用可能 (CC-BY-4.0)
- 研究発表のスライド・ポスター作成、資料作成等に､ぜひご活用ください
- [TogoTVのコンテンツを再利用したいのですが、著作権の扱いはどうなっていますか?](https://togotv.dbcls.jp/faq.html)
- 2022年2月末で55件の[引用論文](https://dbcls.rois.ac.jp/references.html#TogoTV)

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_05.png)

---
# リクエスト募集中
- お探しの動画マニュアルや画像が見つからない場合は、[統合TV番組リクエストフォーム](https://togotv.dbcls.jp/contact.html)でお気軽にリクエストしてください。
- すべて目を通しています
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_06.png)

---
# TogoTVコンテンツを作ってみたい方も募集中
- 動画や画像(イラスト)を制作してくれる方を随時募集中です
- オンラインで完結する作成環境を整備しており、遠隔地でもOKです。
- DB・ウェブツールについて詳しくなくても、勉強しながらでOK。
- 「本業優先」がポリシーです。
- 謝金あります。
- 動画制作の実際: [「画面録画/編集ソフトウェア Camtasia 2019 を使って統合TVの動画を作成する」](https://togotv.dbcls.jp/20200129.html)
- 静止画制作の実際: [「ライフサイエンス分野のイラスト集を作る仕事@AJACS本郷8」](https://togotv.dbcls.jp/20110322.html)


----
# 【第9回】学術論文を効率的に検索したり、論文執筆を支援するデータベースやツール
---
###  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/)
#### 泣く子も黙る文献・論文検索の総本山
 -  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) (パブメド) は、米国立医学図書館(National Library of Medicine: NLM)が運営している文献情報データベースです。
    - 1997年6月のサービス開始以来、2019年4月時点で5200件を超える学術誌を対象に、およそ 2,900万件超の文献情報を提供しています。
    - 2015年の一年だけで110万件超 (約3,000件/1日)の論文が追加され、その数はさらに増加しています。
    - 一日あたりの検索がおよそ250万件、160万人の利用者、830万件の書誌情報閲覧回数と、生命科学分野で最も利用されているウェブサービスの一つです。
    
- ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_01.png)

- [PubMed Central (PMC)](https://www.ncbi.nlm.nih.gov/pmc/)は、書誌情報、アブストラクトに加えて全文が無料（オープンアクセス）で公開されている論文を収録・提供しています。
    - PMCの件数でおよそ 540 万件、論文誌のウェブサイトで全文が提供されているものも含めると600万件以上の論文で全文を読むことができます。
    - 最近では、研究予算配分機関の指定で、成果をオープンアクセス誌で公表することを義務付けていることもあるので、閲覧できる論文が増えてきています。
- ![PMC](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_02.png)

##### 論文を検索する

 1. Google検索で「PubMed」と検索します。
    1. トップに出てくる「Home - PubMed - NCBI」[https://www.ncbi.nlm.nih.gov/pubmed/](https://www.ncbi.nlm.nih.gov/pubmed/) をクリックします。あるいは、ウェブブラウザのアドレスバーに直接「pubmed.gov」と入力しても自動でリダイレクトされます。
 1. 検索窓にキーワードを入力し始めると、関連語がサジェストされます。
    1. [Hiromasa Ono](https://www.ncbi.nlm.nih.gov/pubmed/?term=Hiromasa+Ono) で検索してみます。
    - ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_04.png)
    - 個別の論文には固有のIDであるPMID(PubMed ID)がついています。
        - URLの末尾に直接入力するとダイレクトにその論文へたどり着けます。 [https://www.ncbi.nlm.nih.gov/pubmed/28850115](https://www.ncbi.nlm.nih.gov/pubmed/28850115)
    1. ちなみに、検索窓に「All[filter]」と入力し検索すると、検索時点におけるPubMedに収載されている全論文数を調べることができます。
    - ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_03.png)
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
- ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_05.png)
- ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/190604_PubMed_06.png)
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
# 【第10回】生命科学分野の様々なデータベース
---
## NCBI (National Center for Biotechnology Information)
### [NCBI Databases](https://www.ncbi.nlm.nih.gov/search/?term=)
- 米国 国立生物工学情報センター (National Center for Biotechnology Information: NCBI)
- 文献、遺伝子、遺伝学、タンパク質、ゲノム、化合物といったあらゆるデータベースがあります。
![NCBI top](https://raw.githubusercontent.com/hiromasaono/training/master/images/190530_NCBI.png)
- [【NCBI】に関係する統合TV動画](https://togotv.dbcls.jp/result.html?type=manual&page=1&query=NCBI)
### NCBIで 遺伝子 を調べる
- <details><summary>そもそも遺伝子(gene)ってなに?　ゲノム(genome)とDNAの違いは?</summary>
    [遺伝子とゲノム](https://www.ddbj.nig.ac.jp/column/genegenome.html) (国立遺伝学研究所 生命情報・DDBJセンター ウェブサイト)</details>
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


### RefExを使って、組織特異的遺伝子を検索する
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
- サンプルデータとして、[NCBI GEO](http://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います。このデータは、 **ある実験の前後の2群間で有意に発現減少した遺伝子群** のリストです。  

     → [マル秘遺伝子リスト](https://raw.githubusercontent.com/AJACS-training/AJACS59/master/hono/secret_list.txt)  （右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）

- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！  【課題レポートの内容】

### DAVIDを用いて、遺伝子発現データの結果を生物学的に解釈する
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

12. DAVIDを使って皆さんが得た結果を解析・考察してみましょう。
 - わかっていること
    - マル秘遺伝子リストは「ある実験の前後の2群間で有意に発現減少した遺伝子群のリスト」  
    - 生物種はArabidopsis thaliana (シロイヌナズナ)  
 - 課題
    1. DAVIDを使って得たGeneOntologyのエンリッチメント解析データのうち、あなたはどの部分に着目したか(複数可)についてその理由とともに説明してください。
    1. i.の説明した実験データの解釈から、「マル秘遺伝子リスト」は、 どのような実験をした結果得られたデータだと推測できるのか、あなたの考えを書いてください。
---


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
