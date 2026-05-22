# IME用将棋用語辞書

将棋用語をすばやく快適に入力するための、かな漢字変換システム向け変換辞書です。語の意味を説明する辞書ではなく、MS-IME、ATOK、ことえりなどに登録して将棋用語の入力を楽にするための辞書データです。

詰将棋用語を含む幅広い語彙を収録し、将棋界の変化に合わせて継続的に保守しています。語の追加要望や誤りの指摘は、Issue または Pull Request でお寄せください。

なお、この辞書を登録したことによって日常の入力で誤変換などが発生しても責任は取れませんので、注意してお使いください。

## ダウンロード

最新版は [GitHub Releases](https://github.com/knu/imedic-shogi/releases/latest) からダウンロードできます。

- [ATOK形式](https://github.com/knu/imedic-shogi/releases/latest/download/shogi.atok.txt)
- [MS-IME形式](https://github.com/knu/imedic-shogi/releases/latest/download/shogi.msime.txt)
- [ことえり形式](https://github.com/knu/imedic-shogi/releases/latest/download/shogi.kotoeri.txt)

MS-IME形式は BOM 付き UTF-16LE / CRLF です。

開発版の元データは [shogi.txt](./shogi.txt) です。

## 使い方

お使いの環境に合った形式の辞書テキストをダウンロードして、各 IME の辞書登録機能で取り込んでください。ブラウザ内で辞書ファイルが開いた場合は、ファイルとして保存してから登録してください。

### Windows

Windows 標準の Microsoft IME では、MS-IME形式を使います。

IME の設定画面から辞書ツールを開き、「テキストファイルからの登録」でダウンロードした `shogi.msime.txt` を指定してください。

ATOK では、辞書ユーティリティの一括処理で単語ファイルとして `shogi.atok.txt` を指定して登録します。

Google 日本語入力では、辞書ツールからフォーマット「Microsoft IME」で `shogi.msime.txt` をインポートしてください。

### macOS

標準の日本語入力では、ことえり形式を使います。日本語入力ソースに切り替え、メニューバーの入力メニューから「“日本語 - ……入力”設定を開く」を選択してください。サイドバーで対象の入力ソースを選び、「入力ソース」設定ダイアログ下部の「追加辞書」ボックスに `shogi.kotoeri.txt` をドラッグして登録します。

ATOK ではATOK形式を使います。辞書ユーティリティの一括処理で `shogi.atok.txt` を指定して登録してください。

Google 日本語入力ではATOK形式またはMS-IME形式が使えます。辞書ツールから `shogi.atok.txt` をインポートしてください。

### その他

利用している IME が上記の形式に対応している場合は、対応する形式のファイルをインポートしてください。未対応の環境では、[shogi.txt](./shogi.txt) を元に適宜変換して利用してください。

## ライセンス

この変換辞書データは、クリエイティブ・コモンズ「表示-継承 2.1 日本」ライセンスの下で利用できます。

- [Creative Commons Attribution-Share Alike 2.1 Japan License](http://creativecommons.org/licenses/by-sa/2.1/jp/)

なお、この辞書の編集著作権は、これを利用して入力した文章には及びません。文章の著作権は、その著作者に属します。

Copyright (c) 2001-2026 Akinori MUSHA
