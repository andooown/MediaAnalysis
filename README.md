# メディア分析法の実験

## twitter.py
Twitterから特定の単語で検索した結果をCSVファイルに書き出すスクリプトです。
`twitter_config.py`を同じディレクトリに作成し、Twitter APIのアクセスキーを以下のように記載して下さい。

```
CONSUMER_KEY = 'XXX'
CONSUMER_SECRET = 'XXX'
ACCESS_TOKEN = 'XXX'
ACCESS_TOKEN_SECRET = 'XXX'
```


## analysis.py
`twitter.py`で出力したツイートの本文を形態素解析にかけ、単語ごとの出現頻度を計算するスクリプトです。

- IPA辞書で形態素解析を行った`out_ipadic_***.csv`
- Neologism dictionary for MeCabで形態素解析を行った`out_neologd_***.csv`
の2つのファイルが出力されます。