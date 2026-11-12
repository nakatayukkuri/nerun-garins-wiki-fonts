# ネルン字・ガリンス文字｜Miraheze Wikiフォント

混裵世界で使用する架空文字 **ネルン刻線文字** と **ガリンス文字** のWebフォント公開リポジトリです。

## 公開フォント

| ファイル | 内容 |
|---|---|
| `nerun-script.woff2` | ネルン文字：16字根＋複合6字、計22字形 |
| `garins-script.woff2` | ガリンス語：手描き84字形に対応 |

**重要：** フォント本体をGitHubへアップロードすると、以下のURLから読み込めるようになります。

- ネルン字：`https://cdn.jsdelivr.net/gh/nakatayukkuri/nerun-garins-wiki-fonts@main/nerun-script.woff2`
- ガリンス語：`https://cdn.jsdelivr.net/gh/nakatayukkuri/nerun-garins-wiki-fonts@main/garins-script.woff2`

## Mirahezeへの導入

1. このリポジトリに上記の **2つの WOFF2 ファイル**をアップロードします。
2. `Miraheze_Common.css` を開き、その内容をWikiの `MediaWiki:Common.css` の末尾へ貼り付けて保存します。
3. `Wiki_表示テスト.wikitext` をWikiのテストページに貼り付けて字形が表示されるか確認します。

Wikiの編集には、通常インターフェース管理者権限が必要です。外部Webフォントの表示はWikiのCSPとCDNのCORSにも依存します。

## 文字の入力

- **ネルン文字：** 専用文字コード（私用領域、PUA）を使用。例：U+E000 = `na`、U+E010 = `na-mo`。文字列 `na` を直接入力しても自動変換されません。
- **ガリンス文字：** この再生成フォントは通常の英字 `a`〜`z`、大文字・アクセント付き文字とPUAを対応づけています。
- 2フォントは私用領域の割当が重なるため、必ず `.nerun-script` と `.garins-script` のCSSクラスで区別してください。

## デザイン・データについて

ネルン字のフォントは元の `NerunScratch-Regular.woff2` を改名。ガリンス文字のフォントは手描き84字データから再生成したものです。いずれも混裵世界の創作用素材であり、本文の設定や正史の採否とは別に取り扱います。

**このリポジトリはフォント公開専用です。**
