# これから研究室に入る初学者のための便利な生命科学系公共データベースとバイオインフォマティクスツールの使いこなし演習
## [https://x.gd/qM5x6](https://x.gd/qM5x6)

広島大学ゲノム編集イノベーションセンター / プラチナバイオ株式会社  
小野 浩雅 ([X@h_ono](https://twitter.com/h_ono), [researchmap](https://researchmap.jp/hiromasaono))  
onohrms@hiroshima-u.ac.jp

2025年7月2日-30日(全5回・毎週水曜日2限（10:40-12:10))  
日本大学 生物資源学部 動物学科　令和7年度　前期　水曜日2時限

----

これは、2025年度 日本大学 生物資源学部 動物学科　令和7年度　前期　「生物情報学」の小野担当回の講習資料です。 
© 2025 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

----

## 概要

ヒトゲノム計画が完了してから17年(実は、つい最近まで完全には解読されていなかった - [ヒトゲノム計画とヒトゲノム完全解読](https://www.jstage.jst.go.jp/article/jsbibr/3/1/3_jsbibr.2022.primer2/_html/-char/ja))がたち、今や技術革新により日々膨大なデータが産み出され、それらは様々なデータベースに登録され、その多くは公開される時代となっています。そして、生命科学研究を効率よく進めるためには、これらのデータをいかに有効活用するかが鍵になっています。  
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
- 2024年4月から
  - 広島大学ゲノム編集イノベーションセンター 研究員 / [プラチナバイオ株式会社](https://www.pt-bio.com/) 事業推進部 ディレクター
    - さまざまな産業有用生物のゲノム情報の取得や目的機能に関わる遺伝子の特定、ゲノム編集による機能向上までを一貫して実現できるプラットフォームをつくる
      - [Egg for All プロジェクト：世界初のアレルギー対応卵で食の壁を打ち破る](https://www.pt-bio.com/project/egg-for-all)


----

## 講義の流れ(予定)
今回の講義(全5回)では、お手元のコンピュータを使って以下の内容について説明します。

- [【第11回】研究現場で頻繁に使われるデータベースやツールを知る](#第6回研究現場で頻繁に使われるデータベースやツールを知る)
  - 統合TV
- [【第12回】学術論文を効率的に検索したり、論文執筆を支援するデータベースやツール](#第7回学術論文を効率的に検索したり論文執筆を支援するデータベースやツール)
    - PubMed
  - 生命科学系の文献に頻出する英語表現を高速に検索する
    - inMeXes
  - 生命科学分野の略語・展開形を検索する
    - Allie
  - 類似したテキストの差分を検索・表示する
    - difff(ﾃﾞｭﾌﾌ)
- [【第13回】生命科学分野の王道データベースNCBIを使って遺伝子について調べる](#第8回生命科学分野の王道データベースncbiを使って遺伝子について調べる)
    - NCBI
  - 遺伝子やゲノム配列を高速に検索する
    - GGRNA
    - GGGenome
    - CRISPRdirect
- [【第14回】ゲノムデータベースとゲノムブラウザ](#第9回ゲノムデータベースとゲノムブラウザ)
  - Ensembl Genome Browser
  - UCSC Genome browser   
- [【第15回】公共データベースから利用可能な遺伝子発現データを解析する](#第15回公共データベースから利用可能な遺伝子発現データを解析する)
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
# 【第11回】研究現場で頻繁に使われるデータベースやツールを知る
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
- コロナ禍の自粛時に過去最高の視聴数
- YouTubeのチャンネル登録をすると新規公開の通知が来て便利です…!
  -　チャンネル登録者数10,700人突破！

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20250626_01.jpg)

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
       - 入力した塩基配列に対してゲノム編集実験に用いるCRISPR-Cas9システムのガイドRNAを設計することができるツール
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
# イラストを探す (Togo picture gallery)
- [「イラストを探す」](https://togotv.dbcls.jp/pics.html)
- 生命科学分野のイラスト(約2,200本)が、誰でも自由に利用可能 (CC-BY-4.0)
- 研究発表のスライド・ポスター作成、資料作成等に､ぜひご活用ください
- [TogoTVのコンテンツを再利用したいのですが、著作権の扱いはどうなっていますか?](https://togotv.dbcls.jp/faq.html)
- 2024年4月末で120件の[引用論文](https://dbcls.rois.ac.jp/references.html#TogoTV)

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20230523_05.png)

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
# 【第12回】学術論文を効率的に検索したり、論文執筆を支援するデータベースやツール
---
## 現代の生命科学の研究の流れ
  - 対象とする生体試料を準備し、それを測定し、計算機で解析し、成果をまとめて論文にする
  - 学術誌、論文誌に投稿する
    - 編集者が内容をチェック
    - 大きな問題なければ、同じ研究分野の研究者に記載内容のチェックを依頼する(査読･レビュー)
      - 掲載受理(accept)
      - 修正するべき小さな問題がある(minor revision)
      - 修正するべき大きな問題がある(major revision)
      - 掲載するのに適切ではない(reject)
    - 論文誌に掲載
  - 関連分野の論文を読んだり、新たな仮説や追加のデータを得るなどして、新たな論文を書く
  - 以下ループ

--- 
###  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/)
#### 泣く子も黙る文献・論文検索の総本山
 -  [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) (パブメド) は、米国立医学図書館(National Library of Medicine: NLM)が運営している文献情報データベースです。
    - 1997年6月のサービス開始以来、2022年6月時点で5200件を超える学術誌を対象に、およそ 3,400万件超の文献情報を提供しています。
    - 2015年の一年だけで110万件超 (約3,000件/1日)の論文が追加され、その数はさらに増加しています。
    - 一日あたりの検索がおよそ250万件、160万人の利用者、1,000万件以上の書誌情報閲覧回数と、生命科学分野で最も利用されているウェブサービスの一つです。
    - [MEDLINE PubMed Production Statistics](https://www.nlm.nih.gov/bsd/medline_pubmed_production_stats.html)
    
- ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/220613_01.jpg)

- [PubMed Central (PMC)](https://www.ncbi.nlm.nih.gov/pmc/)は、書誌情報、アブストラクトに加えて全文が無料（オープンアクセス）で公開されている論文を収録・提供しています。
    - PMCの件数と論文誌のウェブサイトで全文が提供されているものも含めると800万件以上の論文で全文を読むことができます。
    - 最近では、研究予算配分機関の指定で、成果をオープンアクセス誌で公表することを義務付けていることもあるので、閲覧できる論文が増えてきています。
- ![PMC](https://raw.githubusercontent.com/hiromasaono/training/master/images/220613_02.jpg)

#### 論文を検索する

 1. Google検索で「PubMed」と検索します。
    1. トップに出てくる「Home - PubMed - NCBI」[https://www.ncbi.nlm.nih.gov/pubmed/](https://www.ncbi.nlm.nih.gov/pubmed/) をクリックします。あるいは、ウェブブラウザのアドレスバーに直接「pubmed.gov」と入力しても自動でリダイレクトされます。
 1. 検索窓にキーワードを入力し始めると、関連語がサジェストされます。
    1. [Hiromasa Ono](https://www.ncbi.nlm.nih.gov/pubmed/?term=Hiromasa+Ono) で検索してみます。
    - ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/230530_03.png)
    - 個別の論文には固有のIDであるPMID(PubMed ID)がついています。
        - URLの末尾に直接入力するとダイレクトにその論文へたどり着けます。 [https://www.ncbi.nlm.nih.gov/pubmed/28850115](https://www.ncbi.nlm.nih.gov/pubmed/28850115)
    1. ちなみに、検索窓に「All[filter]」と入力し検索すると、検索時点におけるPubMedに収載されている全論文数を調べることができます。
    - ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/220613_04.jpg)
 1. 初期設定では、検索結果は、検索語との｢Best match｣順に表示されます。
    1. ｢Display option｣で表示する順番や表示形式を変更することができます。
    1. 画面左側には検索用のフィルタが用意されており、論文の種類や全文を購読できるか否か、出版日の指定、論文の種類などで絞り込むことができます。
 1. 検索結果一覧に「Free PMC article」や「Free Article」の表示がある場合は、全文を読むことができるオープンアクセスの論文であることを示しています。
    1. 前者はPMCのウェブサイトで全文閲覧ができ、後者は論文誌のウェブサイトで全文閲覧ができます。
    1. PMCへのリンクをクリックすると、PMCが提供する様々な形式で全文を読むことができます。
        1. 論文PDFのダウンロードはもちろん可能です。
        1. 引用文献へのリンクが動的に表示されるなどウェブサイトでの表示に適したスタイルのほか、近年利用が増えているタブレット端末での表示に最適化された「PubReader」の機能が提供されています。
 1. 個別の論文の右側には、｢page navigation｣がついており、クリックすると該当箇所に飛べます。
      1. **Similar articles** で関連する論文を検索
      1. **Cited by** でその論文を引用した論文を検索
      1. MeSH Termsでその論文のキーワードを知る(後述)

#### 自分の探している論文が見つからないときはMeSH Terms を使ってみる

 1. 検索結果が思ったように得られない、あるいは、数が多すぎて絞りきれない場合は、MeSH Termsを有効活用してみましょう。
    1. PubMedでは各論文にMeSH Termsが検索用の「#ハッシュタグ」のように付与されています。
            1. MeSH Terms とは、
                1. MeSHは、Medical Subject Headings の略で、階層構造を持つ統制された概念・語彙集として主に医学関係の用語を整理したものです。語彙数は約3万弱ほどあり、毎年更新されています。PubMedに収録された全論文に対して専門のスタッフがMeSHタームを用いて注釈付けを行っています。
    - [https://pubmed.ncbi.nlm.nih.gov/21419102/](https://pubmed.ncbi.nlm.nih.gov/21419102/) のMeSH Termsの例
      - ![PubMed](https://raw.githubusercontent.com/hiromasaono/training/master/images/220613_05.jpg)
- [Google Scholar](https://scholar.google.com/) を使うのも手
  - Google Scholarでは、その文献が引用された数を元に検索結果を表示するため、引用先の論文を非常に探しやすい
  - 統合TV: [研究者のためのGoogle活用術 〜Google Scholarを中心に〜 2017](https://togotv.dbcls.jp/20170605.html)

#### PubMedの検索結果を定点観測する

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

#### 統合TVでPubMedの使いかたを学ぶ
 - PubMedで論文を検索する [https://doi.org/10.7875/togotv.2020.053](https://doi.org/10.7875/togotv.2020.053)
 - PMC (PubMedCentral) の使い方 2017　 [https://doi.org/10.7875/togotv.2017.122](https://doi.org/10.7875/togotv.2017.122)  
 - 最新の文献検索方法を知る @ AJACSオンライン16 [https://doi.org/10.7875/togotv.2023.054](https://doi.org/10.7875/togotv.2023.054)
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

#### 統合TVで使いかたを学ぶ

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

#### 統合TVで使いかたを学ぶ

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

#### 統合TVで使いかたを学ぶ
* 統合TV「[difff《デュフフ》を使って文章の変更箇所を調べる](https://togotv.dbcls.jp/20130828.html)」DOI: 10.7875/togotv.2013.056


## 英語の文章を翻訳する
### DeepL
- [DeepL](https://www.deepl.com/ja/blog)は、ドイツのDeepL社が開発した基本利用は無料の機械翻訳サービス
- コピペするだけで精度の高い翻訳文を得ることができる
- ときどき、判断が難しい文章をスルーすることがある点は注意

## 英語の文章を校正する
### Grammarly
- [Grammarly](https://www.grammarly.com/)は、英文法および英単語スペルのチェックを行うことができるウェブツール。
- Grammarlyのウェブサイト上にタイプ(あるいはコピー・アンド・ペースト)した文章は自動的に校正され、修正候補が表示される。
- Chromeのアドオンも提供(Grammarly for Chrome)されており、これを導入すると、他のウェブサービスで入力中の文章も自動的に校正することができる
	- Grammarly を使って英文校正をする [https://togotv.dbcls.jp/20181213.html](https://togotv.dbcls.jp/20181213.html)

### 生成AI
- [ChatGPT](https://chat.openai.com)は、OpenAI社が開発した人工知能チャットボットで、大規模なデータセットから学習して自然な対話を生成する、生成AIの一種。
- 高度な自然言語処理技術を使用し、質疑応答や文章生成に優れた性能を発揮する。
- 正しく使うことができれば、Web検索よりも迅速で効果的な情報収集が可能になったり、また幅広い作業タスクに対応することができる。
- 期待した出力を得るためには、「プロンプト」の作成方法を工夫する必要がある
	- [科学研究のためのChatGPTの使い方\(基本編\)](https://togotv.dbcls.jp/20231228.html)
- 活用の心構え
  - **知らないことは命令できない**
  - **優秀かつ業界未経験の新人だと思って接する**    
    - [生成AIの可能性と課題 ～賢く使いこなすために～](https://togotv.dbcls.jp/20240805.html)
    - [研究効率化の鍵は生成AI ～文献調査・資料作成を加速するサービス～](https://togotv.dbcls.jp/20240806.html)

---


# 【第13回】生命科学分野の王道データベースNCBIを使って遺伝子について調べる
---
## NCBI (National Center for Biotechnology Information)
### [NCBI Databases](https://www.ncbi.nlm.nih.gov/search/?term=)
- 米国 国立生物工学情報センター (National Center for Biotechnology Information: NCBI)
- 文献、遺伝子、遺伝学、タンパク質、ゲノム、化合物といったあらゆるデータベースがあります。
![NCBI top](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220621_1.jpg)
  - ここでも **all[filter]** を使って全件数を調べられます。
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
1. NCBI Gene データベースにおける **ヒトのALHD2 のページ** [https://www.ncbi.nlm.nih.gov/gene/217](https://www.ncbi.nlm.nih.gov/gene/217) が表示されます
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
# 【第14回】ゲノムデータベースとゲノムブラウザ
## ゲノムデータベース・ゲノムブラウザ
### ゲノムデータベースとは？
- ゲノム配列をはじめとした（遺伝）情報を生物種ごとにまとめたデータベース
- 狭義にはゲノム配列のデータベースを指す
### リファレンス(参照)ゲノム配列
- ヒトやその他の生物のゲノム配列は個体ごとに異なる
- 基準となるゲノム配列がなければその｢違い｣を定量的に評価することができない
- 様々なゲノム配列をもとにしてその最大公約数的なゲノム配列を基準ゲノム配列として決めている
	- リファレンス配列と個々の生物のゲノム配列を比較する
	- シーケンシングされたリード配列をリファレンス配列にマッピングすることで発現量を定量する
- 各ゲノムのいわゆる「バージョン」は、アセンブリやビルドと呼ばれる
	- 最新のヒトゲノムは、GRCh38 (for Genome Research Consortium human build 38)
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
  - 生命科学分野の[Google map](https://www.google.co.jp/maps/place/%E6%97%A5%E6%9C%AC%E5%A4%A7%E5%AD%A6%E7%94%9F%E7%89%A9%E8%B3%87%E6%BA%90%E7%A7%91%E5%AD%A6%E9%83%A8/@35.3806744,139.4674663,17z/data=!3m1!4b1!4m5!3m4!1s0x601851a101ca6eaf:0x3c594193604e3516!8m2!3d35.38067!4d139.469655?hl=ja)のようなイメージ
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

### 【実習2】 Ensembl Genome Browser

- [Ensembl Genome Browser](http://asia.ensembl.org/index.html)
   - European Bioinformatics Institute (EMBL-EBI)(欧州バイオインフォマティクス研究所) で開発、維持されているゲノムブラウザ、ゲノムアノテーション閲覧システム
   - あんさんぶる、と読みます。
   - 脊椎動物のゲノムを対象としたゲノムブラウザ
   - 比較ゲノム、進化、配列変異、転写制御などの研究をサポート
   - Ensembl Genome Browser でも上記のALDH2を検索してみましょう。
- EnsemblGenomes [`https://ensemblgenomes.org/`](https://ensemblgenomes.org//)
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
- 過去のバージョンのゲノムアノテーションを調べる [`http://doi.org/10.7875/togotv.2017.088`](http://doi.org/10.7875/togotv.2017.088)
- 遺伝子の場所や周辺情報を調べる [`http://doi.org/10.7875/togotv.2017.082`](http://doi.org/10.7875/togotv.2017.082)

### ID変換ツール
  - [TogoID](https://togoid.dbcls.jp/)
    - 直感的なインターフェースにより生命科学系データベース(DB)間のつながりを探索的に確認しながらID変換を行うことができるウェブアプリケーションです。
    - 遺伝子、タンパク質、化合物、疾患、遺伝子バリアントといった幅広いカテゴリーに渡る65種(2022年5月時点)のIDを対象としています。
    - 変換されたIDをすぐに他のサービスで利用できるようクリップボードにコピーする機能があるほか、変換されたIDリスト、IDに対応するURL、そして変換経路のすべてのIDを含むデータをCSV形式でダウンロードすることができます。
    - 統合TV: [TogoIDを使って生命科学分野のデータベースのID間の対応関係を検索し変換する](https://togotv.dbcls.jp/20210910.html)
---


# 【第15回】公共データベースから利用可能な遺伝子発現データを解析する
## 遺伝子発現データの機能解析とは
- 実験条件によって得られる遺伝子の発現量を測定する
  - 実験区と対照区
    - がんの肝臓(実験区)と健康な肝臓(対照区)
    - 薬剤投与したマウス(実験区)と生理食塩水を投与したマウス(対照区)
  - 発展編として時系列データ
- 大規模に遺伝子発現量を調べる方法
  - マイクロアレイ
  - NGS(Next Generation Sequencer:次世代シーケンサー)
- 発現変動遺伝子(Differentially Expressed Genes: DEGs)
  - 発現量を比較して差があった遺伝子(群)
    - ｢差があった｣の定義もいろいろある
      - n倍変化した、統計的有意に変化した、その両方、など
    - 発現量が顕著に異なる遺伝子=その実験条件に影響を受けた遺伝子
- 遺伝子発現･機能解析
  - 実験条件によって得られた数十～数千のDEGsが生物学的にどういう意味を持つかを考えることが第一歩
  - ![Gyazo](http://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)
- [Gene Ontology(GO)](http://geneontology.org/)
  - 遺伝子の属性を記述する語彙を統一化(GO term)し、種を越えた遺伝子関連情報を記述し構造化することを目的とした国際プロジェクトであり、その成果のこと
  - すべてのGO termは、**biological process（生物学的プロセス）**、**cellular component（細胞の構成要素）**、**molecular function（分子機能）** の3カテゴリーのいずれかに属し、GO term同士の上下関係が一義に決まっている(のでコンピュータで処理しやすい)
  - molecular function＞binding＞protein binding＞receptor binding＞以下、より具体的になる
  - Go term には、[Evidence code](http://geneontology.org/docs/guide-go-evidence-codes/) が付いている

  - [ALDH2の場合の例](https://www.ncbi.nlm.nih.gov/gene/217#gene-ontology)
  - ![ALDH2 GO](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220704_1.jpg)
- GO term のエンリッチメント(Enrichment:濃縮)解析
  - 数十〜数千個のDEGsにそれぞれ付与されたGO termに、どのような偏り(=特徴)があるのかを解析することで、その実験条件のもたらす影響を生物学的に解釈をすることができる
  	- 転写因子活性に関する遺伝子が多いのか、細胞周期に関する遺伝子が多いのか､ 受容体に関する遺伝子が多いのか、など

 

## [DAVID: The Database for Annotation, Visualization and Integrated Discovery](https://davidbioinformatics.nih.gov)
- アメリカ国立アレルギー・感染症研究所が開発･運用
- 2021年に大幅アップデート
- 最新の原著論文 [PMID: 35325185](http://www.ncbi.nlm.nih.gov/pubmed/35325185)
- DEGsのような遺伝子リストをコピペするだけで簡単にエンリッチメント解析 ( GO､KEGG など )することができる
- 対応生物種･遺伝子ID が 豊富｡ ID変換ツールもある
- IDリストしか投げられない (発現量込みやタイムコースデータは不可)


#### マイクロアレイデータの準備
- サンプルデータとして、[NCBI GEO](http://www.ncbi.nlm.nih.gov/geo/)から取得した公共の遺伝子発現データを用います。
- このデータは、 **ある実験の前後の2群間で有意に発現減少した遺伝子群** のリストです。  

     → [マル秘遺伝子リスト](https://raw.githubusercontent.com/hiromasaono/training/master/2022_NUBS/secret_list.txt)  （右クリックして「新しいタブで開く」もしくは「名前を付けてリンク先を保存」してください。）

- このデータは、どのような実験から得られたデータなのか、どのように解釈できるのかをDAVIDを使って考察してみましょう！  【本日の課題】

### DAVIDを用いて、遺伝子発現データの結果を生物学的に解釈する
- 【復習用】[DAVIDを使ってマイクロアレイデータを解析する 2012](http://doi.org/10.7875/togotv.2012.079)
- 【復習用】[DAVIDの使い方 実践編](http://doi.org/10.7875/togotv.2013.033)  

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
  - Benajamini = P-value の多重検定補正された値
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
  <details>
  
  <summary> 「マル秘遺伝子リスト」は、 どのような実験をした結果得られたデータだと推測できるのか、考えてみましょう。</summary>

### 答え　
  - マル秘遺伝子リストは、以下の比較実験をして得たマイクロアレイデータの発現減少遺伝子群でした。
  - 植物細胞と細胞壁分解酵素を用いて取り除いた植物細胞（プロトプラスト)との比較（＝植物細胞のカルス作成前・後）
  - オリジナルデータ取得元 [GSE15515](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE15515)

### 生物学的解釈の一例
  - ｢分化した植物細胞は、G0期という特別な細胞周期にはいり、細胞分裂を行わずに休止している。しかし、このように分化した後でも、植物細胞は分化全能性を保持している。そのため、いったん未分化の状態に戻せば（脱分化）、周囲の環境の調節しだいであらゆる方向へ再分化させることができる。この脱分化された植物細胞こそがカルスである。｣という記載が[カルスのWikipedia](https://ja.wikipedia.org/wiki/%E3%82%AB%E3%83%AB%E3%82%B9_(%E6%A4%8D%E7%89%A9))にあります。カルス=植物の脱分化であり、脱分化が分化した機能の消失を招くならば、植物細胞が機能をしている≒光合成をする、と考えると、今回のGOエンリッチメント解析で｢光合成｣や｢クロロプラスト｣といったGOtermが極めて低いP-valueを示し上位に並んだこと、すなわち、その機能に関与する遺伝子数が偏って多く減少したことと一致すると言えます。
    - このあたりは、植物や細胞生物学の背景知識が必要なところなので皆さんは正解できなくても落ち込む必要はありません。
    - しかし、研究は答えのない問いの｢答え｣を自分で作り他人に納得してもらうような作業でもあるので、その練習をしてもらいました(かなり難しかったとおもいますが、プロの研究者でもそう感じる内容ですのでご安心ください。)
    - 今回は(いちおうの)正解がわかったとおもうので、その上でもう一度講義資料を見返してみるとまた新たな見方ができる良い練習になるかもしれません。</details>
---


## まとめ
- つまみ食い的ではありましたが、全5回の演習で、今日から使える便利な生命科学系公共データベース・バイオインフォマティクスツールについて学びました。
- これらの｢バイオインフォマティクス｣も顕微鏡 や 実験試薬 などと同じ「道具(ツール)」です。
- 便利な「道具」を知って、その使い方が分かれば、あとはみなさん自身の情報分析力と想像力の勝負。
  - 正面からしか見られなかったものが横や後ろやナナメから見ることができて初めて気づくことがあるかもしれません。
- 仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化していきましょう。
- データベースやウェブツールで困ったら、「統合TV」でまず探して・見てみる
- 研究に役立ったら、ぜひ引用・クレジットを!
  - DBCLSの提供するサービス(あるいはそれ以外でも)が、あなたの研究に役立ったら、どんなに些細な事でもぜひ引用(論文、URL等)してください。DBCLSの活動は、提供するサービスがどのくらい活用されたかについて主に引用数などで評価されており、利用者の方の積極的なサポートが必要不可欠です!!
  - [NBDC関連サービスの活用に関する情報提供フォーム](https://form.jst.go.jp/enquetes/nbdcexamples)
