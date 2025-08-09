# 💰 MoneyTracker Pro - スマート家計簿アプリ

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

## 🌟 概要

収支管理から予算管理、データ分析まで、お金の流れを完全に可視化するスマート家計簿アプリです。直感的なUIと豊富な分析機能で、賢い家計管理をサポートします。

### ✨ デモ

[🔗 ライブデモはこちら](https://se0831.github.io/expense-tracker-app/)

### 📸 スクリーンショット

<details>
<summary>クリックして表示</summary>

#### ダッシュボード
![Dashboard](https://via.placeholder.com/800x500/10b981/ffffff?text=MoneyTracker+Dashboard)

#### 分析画面
![Analytics](https://via.placeholder.com/800x500/10b981/ffffff?text=Analytics+View)

#### モバイル表示
![Mobile](https://via.placeholder.com/400x800/10b981/ffffff?text=Mobile+View)

</details>

## 🎯 主な機能

### 💵 収支管理
- **クイック入力** - 素早く簡単に収支を記録
- **カテゴリ分類** - 9種類のカテゴリで自動分類
- **取引履歴** - 全ての取引を時系列で表示
- **検索・フィルター** - 特定の取引を素早く検索

### 📊 データ分析
- **カテゴリ別円グラフ** - 支出の内訳を視覚化
- **月次推移グラフ** - 収支の推移を把握
- **前月比較** - 支出の増減を自動計算
- **AIインサイト** - 支出パターンから節約ポイントを提案

### 🎯 予算管理
- **カテゴリ別予算設定** - 項目ごとに予算を設定
- **進捗バー** - リアルタイムで予算消化率を表示
- **警告システム** - 予算超過を色分けで警告
- **貯金目標** - 目標金額と達成率を表示

### 📈 レポート機能
- **期間切り替え** - 月次/年次/全期間で表示
- **CSV出力** - データをエクスポート
- **CSVインポート** - 外部データの取り込み
- **統計サマリー** - 主要指標を一覧表示

## 🛠️ 使用技術

| カテゴリ | 技術 | 用途 |
|---------|------|------|
| **フロントエンド** | HTML5, CSS3, JavaScript | UI構築 |
| **グラフ描画** | Chart.js | データ可視化 |
| **アイコン** | Font Awesome | UIアイコン |
| **データ保存** | LocalStorage | データ永続化 |
| **スタイリング** | CSS Grid, Flexbox | レスポンシブレイアウト |

## 💻 インストール & 使用方法

### オンラインで使用

```
https://se0831.github.io/expense-tracker-app/
```

### ローカルで実行

1. **リポジトリをクローン**
```bash
git clone https://github.com/SE0831/expense-tracker-app.git
cd expense-tracker-app
```

2. **ブラウザで開く**
```bash
# Macの場合
open index.html

# Windowsの場合
start index.html
```

## 📖 使い方ガイド

### 基本的な使い方

1. **収支の記録**
   - クイック入力フォームで金額を入力
   - カテゴリを選択
   - メモを追加（任意）
   - 「記録する」ボタンをクリック

2. **予算の設定**
   - 各カテゴリの予算は自動設定済み
   - コード内で調整可能

3. **データの分析**
   - 期間を切り替えて推移を確認
   - グラフで支出パターンを把握
   - インサイトで改善点を発見

### カテゴリ一覧

#### 支出カテゴリ
- 🍔 **食費** - 食料品、外食
- 🚃 **交通費** - 電車、バス、タクシー
- 🛍️ **買い物** - 衣類、日用品
- 🎮 **娯楽** - 趣味、レジャー
- 📱 **固定費** - 家賃、光熱費、通信費
- 🏥 **医療・健康** - 病院、薬、フィットネス
- 📚 **教育** - 書籍、講座、学費
- 📦 **その他** - 分類外の支出

#### 収入カテゴリ
- 💰 **給与** - 月給、時給
- 🎁 **賞与** - ボーナス、臨時収入
- 📈 **投資収益** - 配当、売却益
- 📦 **その他** - その他の収入

## 🎨 カスタマイズ

### 予算額の変更

```javascript
// コード内の budgets オブジェクトを編集
const budgets = {
    food: 30000,        // 食費
    transport: 10000,   // 交通費
    shopping: 20000,    // 買い物
    // ... 他のカテゴリ
};
```

### カテゴリの追加

```javascript
// categories オブジェクトに新しいカテゴリを追加
expense: {
    newCategory: { 
        name: '新カテゴリ', 
        icon: '🆕', 
        color: '#yourcolor' 
    }
}
```

### 貯金目標の変更

```javascript
// HTML内の貯金目標セクションを編集
<div class="savings-goal-amount">¥100,000</div>
```

## 📊 データ構造

```javascript
// 取引データの構造
{
    id: 1234567890,           // タイムスタンプID
    type: 'expense',          // 'income' or 'expense'
    amount: 1500,             // 金額
    category: 'food',         // カテゴリキー
    note: 'コンビニで昼食',    // メモ
    date: '2024-08-09T...'    // ISO日付
}
```

## 🚀 今後の改善予定

- [ ] 定期収支の自動入力
- [ ] 複数通貨対応
- [ ] レシート画像のOCR読み取り
- [ ] 家族間での共有機能
- [ ] 銀行口座との連携
- [ ] 詳細な分析レポート生成
- [ ] 節約チャレンジ機能
- [ ] PWA対応（オフライン動作）
- [ ] データのクラウド同期
- [ ] 支出予測AI

## 🤝 貢献

プルリクエストは大歓迎です！

1. フォーク
2. フィーチャーブランチ作成 (`git checkout -b feature/AmazingFeature`)
3. コミット (`git commit -m 'Add some AmazingFeature'`)
4. プッシュ (`git push origin feature/AmazingFeature`)
5. プルリクエスト作成

## 📝 ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 👨‍💻 作者

**SE0831**

- GitHub: [@SE0831](https://github.com/SE0831)
- ポートフォリオ: [その他のプロジェクト](https://github.com/SE0831?tab=repositories)

## 🙏 謝辞

- [Chart.js](https://www.chartjs.org/) - データ可視化ライブラリ
- [Font Awesome](https://fontawesome.com/) - アイコンセット
- [Google Fonts](https://fonts.google.com/) - Webフォント

## 💡 関連プロジェクト

他のポートフォリオ作品もご覧ください：

- [📋 タスク管理アプリ](https://github.com/SE0831/task-management-app)
- [📊 売上分析ダッシュボード](https://github.com/SE0831/sales-analytics-dashboard)
- [📩 お問い合わせフォーム自動通知システム](https://github.com/SE0831/google-forms-chatwork-notifier)

## ⭐ サポート

このプロジェクトが役に立ったら、⭐スターをお願いします！

---

*最終更新: 2024年8月*
