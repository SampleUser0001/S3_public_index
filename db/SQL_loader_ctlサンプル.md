# SQL*loader ctlサンプル

# ctlファイル

```
options(skip = 1)
load data
infile '<csvパス>'
<登録方法>
preserve blanks
into table <テーブル名>
fields terminated by ','
optionally enclosed by '"'
trailing nullcols(
  <カラム名>, <カラム名> ...
)
```

# 実行
```
sqlldr <接続情報> <ctlファイルパス>
```

※接続情報はsql*plusと同じ。

## 備考

登録方法はとりあえずTRUNCATEでいいと思う。

# Origin

https://www.dropbox.com/scl/fi/5ov376n99yugpxpvad3j8/SQLloader-ctl.paper?dl=0&rlkey=oh1waijovlswoqbdgj0vjlpbz

# 参考

[SQL*Loader](https://www.ne.jp/asahi/hishidama/home/tech/oracle/sqlldr.html)
