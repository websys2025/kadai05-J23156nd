## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
   エンドポイント	https://zipcloud.ibsnet.co.jp/api/search
   機能	郵便番号（例：1000001）を指定すると、該当する都道府県、市区町村、町域を返すAPI
* リクエストとレスポンスのフォーマット
    リクエストGET https://zipcloud.ibsnet.co.jp/api/search?zipcode=1000001
    レスポンスのフォーマット
  {
  "message": null,
  "results": [
    {
      "zipcode": "1000001",
      "prefcode": "13",
      "address1": "東京都",
      "address2": "千代田区",
      "address3": "千代田"
    }
  ],
  "status": 200
}

### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
名称	wttr.in
参照URL	https://wttr.in
* エンドポイントと機能
  エンドポイント	https://wttr.in/{city}?format=3
  機能	指定した都市の現在の天気情報（テキスト）を取得できる。APIキー不要。
* リクエストとレスポンスのフォーマット
   GET https://wttr.in/tokyo?format=3
   Tokyo: 🌦 +20°C
### Q3-3. 感想
* 今回の課題で苦労したこと APIのリクエストURLの書き方やレスポンスの処理方法に苦労しました
* 演習を通して理解できたこと PIのリクエストURLの書き方やレスポンスの処理方法に苦労しました
* Web APIの利便性や課題など
  外部のデータ）をリアルタイムで取得し、活用できるとても便利な仕組みです。また、API仕様やフォーマットを正しく理解しないと動作しない。
