# コントリビューションガイド

くもたん辞書リポジトリへの貢献方法について説明します。

---

## 貢献の種類

| 種類 | 説明 | Issueラベル |
|------|------|------------|
| 検索不具合の報告 | 単語の意味・品詞が間違っている | `word_search` |
| チャンク提案 | 熟語・イディオムの追加提案 | `chunk` |
| 検索ロジック改善 | 検索アルゴリズムの改善提案 | `search-improvement` |

---

## Issueの流れ

```
フィードバック投稿 (Bluesky等)
        ↓
  Issue 自動作成
        ↓
  レビュー・確認
        ↓
 「approved」ラベル付与
        ↓
 辞書データへ自動反映
 (overrides.json / chunks.json)
```

`approved` ラベルを付与するのはメンテナーのみです。

---

## 意味の記載について（著作権に関する重要事項）

### やってはいけないこと

他の辞書サービスから文章をそのままコピーすることは**著作権侵害になるおそれ**があります。

特に以下のサービスの文章の無断転載は禁止されています：

- 英辞郎 on the WEB（eow.alc.co.jp）
- Cambridge Dictionary（dictionary.cambridge.org）
- その他、利用規約で転載・複製を禁止している辞書サービス全般

**英辞郎特有の記法（`〔〕`・`◆`・`《》`）がそのまま含まれている場合、コピーと判断されます。**

### やってよいこと

- 意味・概念を**自分の言葉で言い換えて**記載する（意味・概念自体は著作権で保護されません）
- オープンライセンスの辞書の内容を参考にする

### 参考にしてよいオープンライセンス辞書

以下の辞書はライセンスの範囲内で内容を参考にできます：

| 辞書 | ライセンス | URL |
|------|-----------|-----|
| Wiktionary | CC BY-SA 4.0 | https://ja.wiktionary.org/ |
| JMdict/EDICT | CC BY-SA 3.0 | https://www.edrdg.org/jmdict/j_jmdict.html |
| WordNet | MIT相当 | https://wordnet.princeton.edu/ |

### 確認用に使ってよい辞書（コピーは不可）

意味を**確認するためだけ**に使用し、文章はそのままコピーしないでください：

- ことばの窓（https://kotobanomado.jp/）
- Cambridge Dictionary（https://dictionary.cambridge.org/ja/）

---

## チャンク提案の書き方

チャンク（熟語・イディオム）を提案する場合は、以下の形式でIssueを作成してください：

```
### チャンク提案 (chunk)
- **フレーズ**: by the way
- **日本語の意味**: ところで
- **例文**: By the way, did you see the news?
```

---

## ライセンス

このリポジトリの辞書データは [JMdict/EDICT](https://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project) を使用しています。

JMdict is licensed under **CC BY-SA 4.0**.

コントリビューションを行う場合、提供する内容がこのライセンスに適合していることを確認してください。
