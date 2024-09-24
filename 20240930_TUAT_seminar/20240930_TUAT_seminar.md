---
marp: true
theme:
header: "2024/09/30 東京農工大学動物生化学研究室セミナー『データ(ベース)駆動型生命科学研究への招待: 統合データベースの活用事例とバイオインフォマティクスツールの使いこなし術』"
footer: 2024 ONO Hiromasa, CC-BY-4.0
paginate: true

---
# データ(ベース)駆動型生命科学研究への招待: 統合データベースの活用事例とバイオインフォマティクスツールの使いこなし術

---
[プラチナバイオ株式会社](https://www.pt-bio.com/) 事業推進部 ディレクター / 広島大学ゲノム編集イノベーションセンター バイオDX産学共創拠点 プロジェクトマネージャー 
[小野 浩雅](https://researchmap.jp/hiromasaono)  
ono@pt-bio.com / onohrms@hiroshima-u.ac.jp
2024年9月30日
東京農工大学動物生化学研究室セミナー

----

これは、東京農工大学動物生化学研究室セミナー『データ(ベース)駆動型生命科学研究への招待: 統合データベースの活用事例とバイオインフォマティクスツールの使いこなし術』の講演資料です。   
- PDF のダウンロード　
  - [https://bit.ly/20240930_hono](https://bit.ly/20240930_hono)
  - ![bg right:40% 80%](https://raw.githubusercontent.com/hiromasaono/training/master/images/bit.ly_20240930_hono.png)

© 2024 ONO Hiromasa, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)　(出典明記でご自由にお使いください)

----
## 自己紹介
- [小野 浩雅](https://researchmap.jp/hiromasaono) 
  - [統合TV](https://togotv.dbcls.jp/)の運営・編集
  - [RefEx](https://refex.dbcls.jp/)の開発
    - 遺伝子発現解析の基準となる各遺伝子の遺伝子発現量を簡単に検索、閲覧できるウェブツール

  - 2024年4月から
    - [プラチナバイオ株式会社](https://www.pt-bio.com/) 事業推進部 ディレクター / 広島大学ゲノム編集イノベーションセンター バイオDX産学共創拠点 プロジェクトマネージャー
      - 産業有用生物のゲノム情報の取得・目的機能に関わる遺伝子の特定からゲノム編集による機能向上まで一貫して実現できるプラットフォームをつくる
---
# 統合TV(TogoTV)
## 課題
  - 生命科学分野では、DBやバイオインフォマティクスツールの種類や対象が日々増加している
    - 初学者にとっては、何を選ぶべきか、どう使えるのか、組み合わせて使うことができるのかが分からないため利用を躊躇してしまう
    - DBやウェブツールを利活用するためのまとまった教材がほとんどない
---
# 統合TV(TogoTV)
- https://togotv.dbcls.jp/ 📺
  - [DBCLS](https://dbcls.rois.ac.jp/index.html)が運営する、生命科学分野における有用な **データベースやツールの動画マニュアル、講演や講習会動画、資料、イラスト** を独自に制作し、紹介するウェブサイト
    - 実験系研究者の初学者が主要な想定利用者
    - 技術習得の障壁を下げるため、自主学習、新人･後輩指導、講義・勉強会の教材として誰でも自由に使える
  - 2007年8月スタート(2024年で17年目!)
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20221221_01.jpg)

---
# TogoTV@YouTube
- 各動画は[YouTubeで公開](http://www.youtube.com/user/togotv/)されており、環境に応じた解像度、倍速表示等で快適に閲覧可能
- 2,100本を超える動画が公開されており、のべ300万回 (月間3万回以上) 再生
(2023年12月末現在)

![bg right:58% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20231231_TogoTVYouTube_stats_Ja.png)


---
# 統計情報 (2023年12月)
![bg right:58% 90%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20231231_togotv_stats.png)

---
# 個別動画ページ
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20221221_08.jpg)
- ウェブサイトへのアクセスの仕方から結果の解釈まで、操作の一挙手一投足がわかる
- 見どころダイジェスト
  - YouTubeの埋め込みプレーヤなので、おなじみの操作感
  - 動画の概要を示す「見出し」から視聴箇所に移動可能
  - 動画ファイルはダウンロード可能
- ｢再生リストに保存｣する機能
  - Googleアカウントでログインする
  - 利用者オリジナルの動画再生リストを作成、共有、公開することができる

---
# [スキル別コース](https://togotv.dbcls.jp/courses.html)
- ある目的に対して、「この順で動画をみていくと、こういうスキルを獲得できる」というような体系的な動画リスト集
![bg right:50% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20221221_03.jpg)
---

# ラボの新人がまずマスターしたいデータベース・ウェブツール(2020年4月)
- 研究室に入ってきた新人が必ず知っておくべき「論文の効率的な検索方法」、「研究発表資料の作成に必要なパワーポイントの図形描画機能」、「Google各種サービスを使って研究生活を効率化する」という3つのテーマに関する10本の動画を紹介しています
- [解説ブログもあります](https://biosciencedbc.jp/blog/20200511-01.html)
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_03.png)

---

# 文献の検索や管理、情報収集に役立つツール
- 泣く子も黙るPubMedはもちろん、ZoteroやPaperpileなどの文献情報の管理・引用文献リスト作成支援ツールの動画が人気

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20240114_01.jpg)

---
# ウェブブラウザ上でRNA\-seqデータ解析をする
- コマンド操作に苦手意識がある方でもRNA-seqデータ解析ができる時代
- さまざまなツールがあるので、自身の研究テーマに合った解析方法や図を作成するため、また操作感などが合うかなど、複数試してみるのが吉

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20240114_02.jpg)

---

# 現在のラインナップ例 (今後充実させていきます)
- [ラボの新人がまずマスターしたいデータベース・ウェブツール \(2020年4月\)](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00Z89qgyoEbSof6VSGVxpplc)
- [文献の検索や管理、情報収集に役立つツール](https://togotv.dbcls.jp/course.html?id=PL5409971734873D19)
- [文章の執筆に役立つツール](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00Y4Nuo6g08Ql3CsCefTvB9H)
- [塩基配列の検索、取得、比較を行う](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00YVdf_SS5kpKH9uqrYQLqn7)- [ゲノムブラウザを使ってゲノム配列に関連する情報を検索・取得・可視化する](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00bs1Yno9jCCLqVntyzVPqGT)
- [公共の遺伝子発現データの検索や解析を行う](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00YDVET14wC0-GhpI5l3y8T-)
- [ウェブブラウザ上でRNA\-seqデータ解析をする](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00ZUuDj3jxC8lYshLxxjqi-P)
- [図表を作成する](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00aFMd_yWI0xuzROpPWi7nSb)
- [疾患に関連するバリアントや遺伝子発現の情報を調べる](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00a1DeTTRteZSWzmpDTEImAK)
- [バイオインフォマティクスツール･パッケージを自作する](https://togotv.dbcls.jp/course.html?id=PL0uaKHgcG00aJSa233gkhBA2HHe0-Ha-B)



---
# 講演・講習会
- キーワードから、「講演」や「講習会」を簡単に検索可能
- サービスの開発者･研究者が、背景や周辺の基礎知識を紹介するとともにDBやウェブツールの基本的な使いこなし術や高度な組み合わせ方法などを紹介
- 講習会の復習や、他分野の研究内容を (何度でも繰り返し)学習することができます。
![bg right:50% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20221221_05.jpg)

---
# PubMed検索のプロによる文献検索のイロハを学ぶ
  - [最新の文献検索方法を知る @ AJACSオンライン16](https://togotv.dbcls.jp/20230815.html)
    - PubMedの使い方が身につき、自身に必要な文献を効率よく見つけられることを目的として、2020年にリニューアルされたPubMed (パブメド)の基本的な使い方から検索の仕組み、自分の欲しい論文を効率的に検索するにはどうすればよいかなど、PubMedを余すところなく使いこなす方法を紹介
    - PubMed以外にもある便利なサービスを一通り把握し、自身の目的に応じて使えるようにする

---
# 次世代シーケンス(NGS)データ解析に必要な基礎知識とリテラシーを学ぶ
  - [NGSデータから新たな知識を導出するためのデータ解析リテラシー @ AJACS浜松](https://togotv.dbcls.jp/20180120.html)
    - NGSデータを解析するための基礎的な考え方・知識と、データ解析プロセスをどう設計・実践していくかの技術を学びます。ソフトウェアの使い方の詳細な解説よりも、実験系研究者が独学していくために必要なことに焦点を絞っています。
    - 講義資料: [NGSデータから新たな知識を導出するためのデータ解析リテラシー](https://github.com/AJACS-training/AJACS68/blob/master/05_ozaki/README.md)

---

# ウェブブラウザでできるRNA-seqデータ解析を実例を交えて学ぶ
  - [ブラウザ上でRNA-seqデータを解析する @ AJACSオンライン14]()
      - https://togotv.dbcls.jp/20230113.html
      - バルクRNA-seq下流解析ができるようになることを目的として、ウェブブラウザを用いたバルクRNA-seq解析ツールであるiDEPの使い方をハンズオン形式で講習するとともに、類似ツールであるBioJupiesやRaNA-seqについても紹介
      - 胸腺腫合併重症筋無力症の実データを用いた解析実例も紹介



---
# NGS解析について、さらにもっと基礎から応用までを深く学びたい方向け (それぞれ約10-50時間程度)
  - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース(2014年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
  - [「バイオインフォマティクス人材育成カリキュラム 次世代シークエンサ(NGS)ハンズオン講習会(2015年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00Yo0Cn0rcF23xof5hqCzGQb)
  - [NGSハンズオン講習会2016](https://www.youtube.com/watch?v=TSa1yPy_sdM&list=PL0uaKHgcG00ZNpICun17CEAFpV_5Q6GCA)
  - [NGSハンズオン講習会2017](https://www.youtube.com/watch?v=6Fzvl_I48tM&list=PL0uaKHgcG00YDmBXYWOgkmfeURjc8BZkk)
  - [先進ゲノム支援\(PAGS\)、DDBJ、DBCLS合同情報解析講習会\(2019\)](https://www.youtube.com/watch?v=VjZIQuWXPu8&list=PL0uaKHgcG00afJqVErwNQariGDKArJtB8)

---
# 日本人類遺伝学会との連携
  - 日本人類遺伝学会の教育コンテンツ配信システム[JSHG-WebCast(JWC)](https://jshg.jp/webcast/webtools/) 
  - 統合TVと学会との連携は初めての試み
    - 統合TVで作成する動画について学会の推薦を受けた専門家のレビューを受けられる
    - 分野の専門家自身の講義・講習をコンテンツ化できる 
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20221221_06.jpg)

---
# AJACSオンライン９「疾患に関する多型データを解析する｣
- 日本人類遺伝学会との連携によって、講義内容と講師を選定
  - [表現型と遺伝子型のデータを共有および比較する @ AJACSオンライン9](https://togotv.dbcls.jp/20220106.html)
    - 関心対象の表現型が解析によって明らかになった遺伝子型を説明できるか、を検証できるようになる @ 山本 俊至 先生
  - [バリアントの機能を推定する @ AJACSオンライン9](https://togotv.dbcls.jp/20220107.html)
    - バリアントがタンパク質の機能およびスプライシングに与える影響について in silico解析を行うプログラムについて、その使い方と解析結果について理解する @  才津 浩智 先生

---
# イラストを探す (Togo picture gallery)
- [「イラストを探す」](https://togotv.dbcls.jp/pics.html)
- 生命科学分野のイラストが、出典明記だけで、誰でも自由に利用可能 (CC-BY-4.0)
- 研究発表のスライド・ポスター作成、資料作成等に､ぜひご活用ください
- [日本人類遺伝学会との連携はイラストでも](https://jshg.jp/webcast/educations/)
- [統合TVのコンテンツを利用したいのですが、著作権の扱いはどうなっていますか?](https://togotv.dbcls.jp/faq.html)
- 2023年12月末で98件の[引用論文](https://dbcls.rois.ac.jp/references.html#TogoTV)

![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20230523_05.png)

---
# 日本分子生物学会との連携
- 2023年の第46回日本分子生物学会年会(参加者8000人以上)の参加章シール企画に公式採用!
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20231231_MBSJ_togopic.png)

---

# リクエスト募集中
- お探しの動画マニュアルや画像が見つからない場合は、[統合TV番組リクエストフォーム](https://togotv.dbcls.jp/contact.html)でお気軽にリクエストしてください。
- すべて目を通しています
![bg right:40% 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20201223_06.png)
- 動画やイラストの寄託も大歓迎です。

---
# 統合TVコンテンツを作ってみたい方も募集中
- 動画やイラストを制作してくれる方を随時募集中です!
- オンラインで完結する作成環境を整備しており、遠隔地でもOKです。
- 「本業優先」がポリシーで、謝金あります。
- 動画制作の実際: [「画面録画/編集ソフトウェア Camtasia 2019 を使って統合TVの動画を作成する」](https://togotv.dbcls.jp/20200129.html)
- 静止画制作の実際: [「ライフサイエンス分野のイラスト集を作る仕事@AJACS本郷8」](https://togotv.dbcls.jp/20110322.html)
![bg right:40% 85%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20240114_03.jpg)

---
# 参考・関連書籍
- [実験医学増刊 Vol\.40 No\.17 バイオDBとウェブツール　ラボで使える最新70選 知る・学ぶ・使う、バイオDX時代の羅針盤](https://www.yodosha.co.jp/yodobook/book/9784758104067/)
![bg right:40% 70%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20230816_BioDB_Webtool.jpg)

----
## 　内容
- 生命科学分野におけるデータ(ベース)の統合と、データ駆動型研究を行うためのリソース開発
  - **TogoID** を使って生命科学系データベース間のつながりを探索的に確認しながらID変換を行う
  - **TogoDX/human** を使って統合されたデータを探索･俯瞰･抽出する

---
# 生命科学研究はデータベース作り
- さまざまな実験で得られたデータは、論文投稿時などに公共データベース上に登録し、その後誰でも参照可能になるようにすることが義務付けられていることが多い
- 公共データベースには多種多様なデータが日々大量に登録、蓄積され続けている
- データをうまく活用すれば、多くのメリット(がありそうなことは皆感じている)
  - 予備実験をせずに済む
  - 自分の実験結果を支持する知見が得られる
  - 多角的な視点からの新たな仮説生成
- 似たようなものがいくつもありどれを使ってよいかわからない😰
  - 使えそうなものが見つかっても、実際に使うのは大変/使えない場合も多い

---
# データ(ベース)を統合的に組み合わせて、データ駆動型研究を行う
- 生命科学の目的は様々な要素が相互作用している複雑なシステムの理解
  - 多種多様なデータの｢統合｣( ≒ 相互運用性) が必須   
- 課題
  - データベースごとに異なるインターフェース
  - データベース間を繋ぐリンク情報の欠如
  - データベースごとに異なる出力形式
- 横断的にDBを使うには手間がかかりすぎる
  - 個別にデータベースを解析して組み合わせるための｢前処理｣が作業の8割

---
# 課題を解決するための取り組み
- BioHackathon
  - 生命科学分野のデータベース統合の技術基盤の確立を目的として、
  年1回日本各地で開催している国際開発者会議
  - BioHackathon 2015@長崎 にてFAIR原則の内容に関する議論が行われた
    - Wilkinson MD et. al.: The FAIR Guiding Principles for scientific data management and stewardship. Sci Data., [doi:10.1038/sdata.2016.18](http://dx.doi.org/10.1038/sdata.2016.18) (2016)
  - ![w:600](https://raw.githubusercontent.com/hiromasaono/training/master/images/BH2015_groupphoto.png)

---
# FAIR原則 と 知識グラフ
  - Findable、Accessible、**Interoperable**、Reusable
  - それぞれのデータが使いやすくなった（ちょっとずつなってる）
    - 幅広いデータが統合できる時代になった
- 知識グラフによる生命科学分野のデータベース統合
  - 複数のデータセットが共通のURIで連結される
  - 各データとそのつながりの意味が表現できる、すなわち、知識が表現できる
---
# **TogoID** を使って生命科学系データベース間のつながりを探索的に確認しながらID変換を行う
---
# 生命科学分野におけるID変換の必要性 
- 様々なデータべース (DB) を活用するには異なる ID 間のリンクが重要
  - 使いたい解析ツールが手元にある ID では使えない
  - 等価なものに対する ID 間で変換したい
    - 例: NCBI Gene ID ↔ Ensembl Gene ID
  - 関連する情報を取得したい 
    - 遺伝子が関与する疾患、化合物が関与するパスウェイ etc.
-  既存の ID 変換サービスの問題点
   - 対象としている DB の範囲が限られる
   - 大元の DB の更新に追従していない 
   - プログラムから利用できるAPI が提供されていない
---
# TogoID https://togoid/dbcls.jp/
- 生命科学系データベース間のつながりを探索的に確認しながらID変換を行うウェブアプリケーション
- Shuya Ikeda, Hiromasa Ono et. al.: TogoID: an exploratory ID converter to bridge biological datasets, Bioinformatics, [doi:10.1093/bioinformatics/btac491](https://doi.org/10.1093/bioinformatics/btac491) (2022)

  ![bg right 85%](https://raw.githubusercontent.com/hiromasaono/training/master/images/20230614_togoid_top.png)

---
  - **64のデータベースに由来する 89 のデータセットのペア**を収載
    - 遺伝子から化合物、疾患等までを網羅
    - 毎週の定期更新
  - 生物学的意味を持つID間の対応関係を独自の[オントロジー](https://togoid.dbcls.jp/ontology)として整備
  - [GitHubレポジトリ](https://github.com/togoid)は公開
    - 誰でも自由に参照したり新規データセットペアを提案できる
  ![bg right 100%](https://raw.githubusercontent.com/hiromasaono/training/master/images/TogoID_Original_Fig2B.jpg)
   
---
# TogoDX/human を使って統合されたデータを探索･俯瞰･抽出する
---
# データを統合してTogoDXというアプリケーションを作った
- データは統合できるが、それをどう理解・探索・解析するか？
- 統合されたデータに適したインターフェースが必要
  - ヒトデータはデータ量も膨大で多岐にわたっている
  - 誰も本当に統合・俯瞰したことはないんじゃないか
    - それができる TogoDX/human を作った
    - データを入れ替えれば、マウスや〇〇など他のテーマでも流用できる
---
# TogoDX/human https://togodx.dbcls.jp/human/
- 国内外のデータベースから収集・統合した、ヒトに関する遺伝子、タンパク質、化合物、疾患などの情報をワンストップで探索することができるサービス

- TogoDX(Data eXplorer) は、生命科学分野における様々なデータベースを統合的に探索し、俯瞰するためのフレームワーク
  - 膨大な情報を多様な属性 (attribute) によって柔軟に絞り込み、必要な情報を抽出できる新しい仕組み
- TogoDX/humanでは、21個のデータベースに由来する64個の attribute が利用可能

---
# TogoDX で統合されたデータを俯瞰する
![](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220606_1.jpg)

---
# 検索例
- 肺でタンパク質として発現が確認され、
- 細胞膜表面に局在し、
- タンパク質立体構造が明らかになっており、
- 対応する医薬品が開発されている

ヒトのタンパク質の一覧を取得する
![bg right fit](https://raw.githubusercontent.com/hiromasaono/training/master/images/2022-06-03_01.jpg)

---
# 選択した条件を全て満たすIDのリストを抽出できる
![](https://github.com/togodx/togodx-config-human/raw/develop/docs/img/20211001_togodx_example1_01.png)

---
# 抽出したリストにおける他の属性の分布を調べる

![](https://github.com/togodx/togodx-config-human/raw/develop/docs/img/20211001_togodx_example1_02.png)

---
# 自分の持つIDリストの偏りをTogoDX/humanのデータにマッピングして調べる
![](https://raw.githubusercontent.com/hiromasaono/training/master/images/20220606_2.jpg)

---
# まとめ
  - TogoID を使って生命科学系データベース間のつながりを探索的に確認しながらID変換を行う
    - **多種多様なIDを統一的に利用できるよう整備する**ことで、生命科学データの「相互運用性」を高めるよう取り組んでいる
  
  - TogoDX/human を使って統合されたデータを探索･俯瞰･抽出する
    - 「相互運用性」を高めることによって**高度に統合されたデータベースを探索･俯瞰することで新たな知識を抽出できる(データ駆動型生命科学研究の)仕組み**ができあがりつつある


