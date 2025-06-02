![Image](https://github.com/user-attachments/assets/226db50b-e355-4897-b383-5d7520d7e0ff)

# お問合せフォーム付きニュースサイト

**最新の IT 技術ニュースを配信・購読するためのニュースレターアプリケーション**

このプロジェクトでは、架空のテック系ニュースサイトを構築しました。
メールフォームからニュースを購読することができます。また、個人・法人用のお問い合わせフォームも実装しました。

## ✨ 主な機能

以下のフォームへの入力が可能です。

- **ニュースレター購読:** React Hook Form,Conform, Zod で作成したフォーム。
- **お問い合わせ:** React Hook Form,Conform, Zod で作成したフォーム。
- **法人のお客様:** React Hook Form,Conform, Zod で作成したフォーム。

## 🚀 技術スタック

- **フレームワーク:** Next.js (App Router)
- **言語:** TypeScript
- **UI:** React
- **スタイリング:** Tailwind CSS
- **UI コンポーネントライブラリ:** shadcn/ui (内部で lucide-react, class-variance-authority, clsx, tailwind-merge を利用)
- **フォーム管理:** React Hook Form, Conform, Zod

## 🛠️ 開発環境のセットアップ

1.  **リポジトリをクローン:**
    ```bash
    git clone https://github.com/あなたのユーザー名/tech-news-letter.git
    cd tech-news-letter
    ```
2.  **依存パッケージのインストール:**
    ```bash
    npm install
    # または
    # yarn install
    # または
    # pnpm install
    ```
3.  **開発サーバーの起動:**
    ```bash
    npm run dev
    # または
    # yarn dev
    # または
    # pnpm dev
    ```
    ブラウザで `http://localhost:3000` を開きます。

## 📁 プロジェクト構成 (src ディレクトリ)

```
src
├── app/            # Next.js App Routerのルーティングとページコンポーネント
│   ├── (routes)/   # 各ルーティングパスに対応するディレクトリ (例: newsletter/, business/, contact/)
│   │   └── page.tsx  # 各ページのメインコンポーネント
│   ├── api/        # APIルート (バックエンド処理)
│   ├── layout.tsx  # アプリケーション全体の共通レイアウトコンポーネント
│   ├── page.tsx    # ルートページ ("/") のメインコンポーネント
│   └── globals.css # グローバルなCSSスタイルシート
├── actions/        # Server Actions (フォーム処理やデータ変更など)
├── components/     # 再利用可能なUIコンポーネント群
│   └── ui/         # shadcn/ui から導入したベースコンポーネント (例: Button, Card)
├── lib/            # 外部ライブラリの設定やユーティリティ (例: shadcn/ui の utils.ts)
├── schemas/        # Zod スキーマ定義 (バリデーションルールなど)
└── ...             # その他、必要に応じて追加されるディレクトリ (例: hooks, context, types)
```
