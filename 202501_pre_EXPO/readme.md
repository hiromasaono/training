# 鳥類のオボムコイドを比較しよう！
## 〜なぜ鳥の卵によってアレルギー反応が違うの？〜

### 🔍 概要
**所要時間**: 15分  
**対象**: 中学生・高校生  
**テーマ**: 卵アレルギーの原因タンパク質の比較解析

### 🛠️ 準備するもの
- インターネットに接続されたPC/タブレット
- このワークシート
- メモ用紙・筆記用具

### 📚 学習目標
1. タンパク質のアミノ酸配列データベースの使い方を学ぶ
2. 配列アラインメントの基本を理解する
3. 生物種間での配列の違いを観察する

---

### 🔰 Step 1: オボムコイドの配列を取得しよう！

#### 1-1. UniProtにアクセス
- ブラウザで https://www.uniprot.org/ を開く
- 右上の検索ボックスを使用

#### 1-2. 以下の配列を検索
| 生物種 | UniProt ID | 和名 |
|--------|------------|------|
| Gallus gallus | P01005[P01005](https://www.uniprot.org/uniprotkb/P01005/entry) | ニワトリ |
| Coturnix japonica | P01003[P01003](https://www.uniprot.org/uniprotkb/P01003/entry) | ウズラ |
| Anas platyrhynchos | P68150[P68150](https://www.uniprot.org/uniprotkb/P68150/entry) | アヒル |
| Struthio camelus | P05557[P05557](https://www.uniprot.org/uniprotkb/P05557/entry) | ダチョウ |

#### 1-3. 配列の取得手順
1. 各ページの"Sequences"セクションに移動
2. "Download" をクリックして、FASTAフォーマットの配列を表示・コピー
3. メモ帳などに一時保存

> **Point!**
> - UniProt IDを使うと正確に検索できます
> - FASTAフォーマットは「>」で始まる配列データです

---

### 🔄 Step 2: 配列をアラインメントしよう！

#### 2-1. Clustal Omegaにアクセス
- https://www.ebi.ac.uk/Tools/msa/clustalo/ を開く

#### 2-2. 配列の入力方法
1. Step 1でコピーした配列を入力欄に貼り付け
2. パラメータはデフォルトのまま
3. "Submit"ボタンをクリック

#### 2-3. 結果の見方
アラインメント結果の表示記号：
- `*` : 完全に保存された残基
- `:` : 性質が類似したアミノ酸への置換
- `.` : やや性質が異なるアミノ酸への置換

> **Point!**
> - 結果が表示されるまで少し時間がかかります
> - 色分けされた表示で見やすくなっています

---

### 👀 Step 3: 結果を観察しよう！

#### 3-1. 観察ポイント
- システイン残基（C）の位置
- 完全に保存された領域（*マーク）
- 種間で異なるアミノ酸配列の領域

#### 3-2. 結果記入シート
```
【保存された領域のメモ】

システイン残基の位置：

その他の保存された領域：

【違いが見られた領域のメモ】

主な違いが見られた位置：

特徴的な変化：

```

#### 3-3. 考察ポイント
- [ ] システイン残基は保存されているか
- [ ] どの領域に違いが集中しているか
- [ ] アレルギー反応の違いとの関連は？

---

### ❓ トラブルシューティング

#### よくある問題と解決方法

**1. 配列が見つからない場合**
- UniProt IDを再確認
- 検索ボックスに直接IDをコピー＆ペースト

**2. アラインメントがうまくいかない場合**
- FASTAフォーマットを確認
- 余分な空白や記号を削除
- 配列を再コピー

**3. 結果の見方がわからない場合**
- カラー表示を参考に
- スタッフに質問

---

### 📝 まとめシート

```
【本日の発見】

1. 最も保存されていた領域：


2. 種間で異なる領域：


3. アレルギーとの関係で気づいたこと：


【感想・質問】

```

---

### 📚 発展学習のために

#### 参考文献
1. タンパク質構造データベース (PDB)
2. アレルギー情報データベース
3. 統合データベース

#### 関連キーワード
- タンパク質立体構造
- アミノ酸配列保存性
- アレルギーエピトープ
- 分子進化

---

### 🏁 おわりに
お疲れさまでした！
このワークショップで学んだスキルは、他のタンパク質の研究にも応用できます。
さらに詳しく知りたい方は、スタッフまでご質問ください。