# sed

> スクリプトによるテキスト編集。
> もっと詳しく: <https://manned.org/sed.1posix>。

- ファイルの各行で正規表現の最初の出現箇所を置換し、その結果を表示する:

`sed 's/{{正規表現}}/{{置き換え後}}/' {{ファイル名}}`

- ファイル内の拡張正規表現のすべての出現箇所を置換し、その結果を表示する:

`sed -r 's/{{正規表現}}/{{置き換え後}}/g' {{ファイル名}}`

- ファイル内のすべての文字列を置き換え、ファイルを上書きする(すなわち インプレイス):

`sed -i 's/{{置き換え前}}/{{置き換え後}}/g' {{ファイル名}}}`

- ラインパターンに一致する行のみを置換:

`sed '/{{ラインパターン}}/s/{{置き換え前}}/{{置き換え後}}/' {{ファイル名}}`

- ラインパターンに一致する行を削除する:

`sed '/{{ラインパターン}}/d' {{ファイル名}}}`

- ファイルの最初の 11 行を表示する:

`sed 11q {{ファイル名}}`

- 複数の検索・置換式をファイルに適用:

`sed -e 's/{{置き換え名}}/{{置き換え後}}/' -e 's/{{置き換え前}}/{{置き換え後}}/' {{ファイル名}}`

- 区切り文字 `/` を、検索や置換のパターンで使われていない他の文字（例：`#`）で置き換える:

`sed 's#{{置き換え前}}#{{置き換え後}}#' {{ファイル名}}`
