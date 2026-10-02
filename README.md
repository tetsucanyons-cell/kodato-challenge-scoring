# 古田土会計チャレンジプログラム 得点集計・プロジェクター投影システム

古田土会計チャレンジプログラムの得点集計、リアルタイム順位表示、プロジェクター投影、A4用紙印刷（原本デザイン再現）に対応したWebアプリケーションです。

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Ftetsucanyons-cell%2Fkodato-challenge-scoring)

## 🌐 オンラインURL
- **GitHub Pages 公開URL**: [https://tetsucanyons-cell.github.io/kodato-challenge-scoring/](https://tetsucanyons-cell.github.io/kodato-challenge-scoring/)
- **GitHub リポジトリ**: [https://github.com/tetsucanyons-cell/kodato-challenge-scoring](https://github.com/tetsucanyons-cell/kodato-challenge-scoring)
- **Vercel ワンクリックデプロイ**: 上記の「Deploy with Vercel」ボタンをクリックすると、お使いのVercelアカウントに数秒でデプロイされます。

---

## 🌟 主な機能と特徴

### 1. 得点入力・管理 (Score Input)
- **チーム数**: 基本9チーム（設定画面より増減・名称変更が自由に行えます）
- **チャレンジ種目（No.1〜8、各最大30点）**:
  - **水色グループ**:
    - No.1 じゃんけんチャレンジ（連勝数×3点 または直接入力）
    - No.2 割り箸切りチャレンジ（成功本数×3点 または直接入力）
    - No.3 ピクチャーコミュニケーション（計20問、直接入力）
  - **黄色グループ**:
    - No.4 ヘリウムリング（チャレンジ10点 / 惜しい20点 / 達成30点 ワンタップ選択）
    - No.5 トラフィックジャム（チャレンジ10点 / 惜しい20点 / 達成30点 ワンタップ選択）
    - No.6 Aフレーム（チャレンジ10点 / 惜しい20点 / 達成30点 ワンタップ選択）
  - **赤色グループ**:
    - No.7 スーパー神経衰弱（全26ペア完成30点ボーナス込み / 20ペア / 取消 ボタン付き）
    - No.8 パイプライン（成功数×3点 または直接入力）
- **カラー達成チェック**:
  - ルール「*それぞれ色のチャレンジ種目を必ず１つ以上チャレンジしてください*」に基づき、水色・黄色・赤色それぞれの実施状況を自動判定。
  - 未達色の警告アラート、全色達成時のスターバッジを表示。
- **最終チャレンジ（14時45分開始予定）**:
  - 配点マスタ: 1位60点、2位50点、3位45点、4位40点、5位35点、6位30点、7位25点、8位20点、9位15点
  - チームごとに着順（1〜9位）を選択すると配点が自動加算。
  - 順位重複の警告アラート機能＆「順位一括割り当て」モーダル搭載。

### 2. リアルタイム順位表 (Leaderboard)
- 全チームの総合得点、種目別小計、最終チャレンジ得点、各色の達成状況を一覧表示。
- 同点時の順位処理（同位表示）に対応。

### 3. プロジェクター投影モード (Presentation)
- 会場の大型スクリーン・プロジェクター投影用の大画面レイアウト。
- 暗所で見やすいスタイリッシュなダークテーマ。
- 1位〜3位のゴールド・シルバー・ブロンズ装飾。
- **結果発表セレモニー演出**:
  - 9位から1位へカウントダウン発表。
  - Web Audio APIによるドラムロール効果音＆ファンファーレ（外部音声ファイル不要・完全自律動作）。
  - 紙吹雪（Confetti）アニメーション。

### 4. A4印刷対応 (Print Friendly)
- ブラウザの印刷（`Ctrl + P`）でそのままA4出力可能。
- **チーム別得点表**: 元画像の得点表シートデザインを忠実に再現。手書き用白紙シートとしても印刷可能。
- **総合結果発表一覧**: 結果報告・掲示用のレポート。

### 5. データ保護 & オフライン対応
- ブラウザの `localStorage` に自動保存（リロードやブラウザ終了時もデータ保持）。
- JSONバックアップの保存（エクスポート）および復元（インポート）。
- テスト用の「サンプルデータ自動投入」機能。

---

## 💻 使い方

### ローカルでの利用
1. `index.html` をお好みのブラウザ（Google Chrome, Microsoft Edge等）でダブルクリックして開きます。
2. インターネット接続がないオフライン環境でも動作します。

### Vercel での公開
1. 上部の [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Ftetsucanyons-cell%2Fkodato-challenge-scoring) をクリックします。
2. Vercelの画面で「Create」を押すと、わずか数秒で独自の公開URLが発行されます。
