# SQL*loader ctlサンプル

# ctlファイル
    options(skip = 1)
    load data
    infile '<csvパス>'
    append
    info table <テーブル名>
    field terminateed by ','
    optionally enclosed by '"'
    trailing nullcols(
      <カラム名>, <カラム名> ...
    )


# 実行
    sqlldr <接続情報> <ctlファイルパス>

※接続情報はsql*plusと同じ。

