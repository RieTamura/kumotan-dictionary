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

```text
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

特に以下のサービスの文章の無断転載・複製は禁止されています：

- 英辞郎 on the WEB（eow.alc.co.jp）
- Cambridge Dictionary（dictionary.cambridge.org）
- その他、利用規約で転載・複製を禁止している辞書サービス全般

**英辞郎特有の記法（`〔〕`・`◆`・`《》`）がそのまま含まれている場合、コピーと判断されます。**

### やってよいこと

- 意味・概念を**自分の言葉で言い換えて**記載する（意味・概念自体は著作権で保護されません）
- オープンライセンスの辞書の内容を**参照し、自分の言葉で書き直す**こと

### 参考にしてよいオープンライセンス辞書

以下の辞書は、各ライセンスの範囲内で内容を参考にできます。
基本的には「意味や用例を確認して、自分の文章として書き直す」ようにしてください。
文章を引用・転載する場合は、**各辞書のライセンス条件（例：出典表記・ライセンス表記・ShareAlike 等）に必ず従ってください**。

| 辞書 | ライセンス | URL |
|------|-----------|-----|
| Wiktionary | CC BY-SA 4.0 | https://ja.wiktionary.org/ |
| JMdict/EDICT | CC BY-SA 4.0 | https://www.edrdg.org/jmdict/j_jmdict.html |
| WordNet | WordNet License (Princeton University) | https://wordnet.princeton.edu/license-and-commercial-use |

#### 各ライセンスの主な条件

**CC BY-SA 4.0**（Wiktionary・JMdict/EDICT に適用）

| 条件 | 内容 |
|------|------|
| 表示（Attribution） | 著作者名・ライセンス名・ライセンスへのリンクを明記すること |
| 継承（ShareAlike） | 改変・二次利用する場合は、同一ライセンス（CC BY-SA 4.0）で公開すること |
| 商用利用 | 条件を満たせば可能 |

> 例：Wiktionary の内容を転載する場合は「出典：Wiktionary（CC BY-SA 4.0）」と表記し、成果物も CC BY-SA 4.0 で公開する必要があります。

**WordNet License**（WordNet に適用）

| 条件 | 内容 |
|------|------|
| 帰属表示 | すべてのコピー・改変物に著作権表示を含めること（"Copyright 2006 Princeton University"） |
| 引用・クレジット | 利用時は Princeton WordNet を適切に引用・クレジットすること |
| 商用利用 | 可能（無料） |
| 保証 | なし（"AS IS" 提供） |

> 例：WordNet を参照した場合は「WordNet 3.0, Copyright 2006 by Princeton University. All rights reserved.」と表記します。

### 確認用に使ってよい辞書（コピーは不可）

意味を**確認するためだけ**に使用し、文章はそのままコピーしないでください：

- ことばの窓（https://kotobanomado.jp/）
- Cambridge Dictionary（https://dictionary.cambridge.org/ja/）

---

## チャンク提案の書き方

チャンク（熟語・イディオム）を提案する場合は、以下の形式でIssueを作成してください：

```markdown
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
