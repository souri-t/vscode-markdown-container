---
marp: true
theme: default
paginate: true
header: "Marpスライドサンプル"
footer: "© 2024 Your Name"
style: |
  section {
    font-size: 1.5em;
  }
  h1 {
    color: #1a73e8;
  }
---

# Marpスライドサンプル
## プレゼンテーション作成の基本

---

# スライドの構成要素

- 見出し
- リスト
- コード
- 画像
- 表

---

# コードの表示

```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)
```

---

# 画像の表示

![bg left:40% 80%](https://via.placeholder.com/400x300)

## 画像とテキストのレイアウト

- 左側に画像を配置
- 右側にテキストを配置
- 背景画像としても使用可能

---

# 表の表示

| 機能 | 説明 | 使用例 |
|------|------|--------|
| テーマ | スライドのデザイン | `theme: default` |
| ページ番号 | スライド番号の表示 | `paginate: true` |
| ヘッダー | 上部に表示するテキスト | `header: "タイトル"` |

---

# カスタムスタイル

<style scoped>
section {
  background: linear-gradient(to right, #1a73e8, #34a853);
  color: white;
}
</style>

## スライドごとにスタイルを変更

- 背景色のグラデーション
- テキストの色
- フォントサイズ
- その他のCSSプロパティ

---

# 終わりに

## ご清聴ありがとうございました

- 質問はありますか？
- フィードバックをお待ちしています
- 連絡先: example@example.com 