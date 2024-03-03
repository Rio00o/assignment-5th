# HTTPにまつわる用語

## HTTPとは

「HyperText Transfer Protcol」の略でWebサーバとクライアント(PCやスマホ)のWebブラウザがデータを送受信するためのプロトコル(通信手段)です。
プロトコルがあるから異なるメーカーや機種でも通信が可能。



## URLとは

Uniform Resource Locatorの略語で、Webサイトのページがどこに位置するのかを示す「住所」のようなもの。Internet Explorerなどのブラウザでホームページの上部に表示されており、そのhttpやhttpから始まる半角英数の文字列のこと。

## クエリ文字列とは

クエリ（検索）パラメータ（変数）や、クエストリングとも言う

http://〇〇.jp/?▢＝△

上記URLの、？以降の「?▢=△」がクエリ文字列です。

## パス変数(パラメーター)とは何か

パス変数は、ファイル・システム上のロケーションを指定します。パス変数を使用することによってディレクトリー構造をファイル・システムとまったく同じにすることなく、リンクされたリソースを含むプロジェクトをチーム・メンバーと共有することができます。

## クエリ文字列とパス変数の違いとは

①https://zenn.dev/search

②https://zenn.dev/search?q=Laravel

①と②の違いは「search」の後に「?～」があるかどうか

①のパスパラメータはsearchの部分

②の場合はパスパラメータは①と同じくsearch,クエリパラメータは?q=Laravel

## HTTPメソッドとは何か

### GETメソッド
GETメソッドはデータの参照時に使用します。リクエスト元の手元で見えるようにデータを取得します。

### POSTメソッド
POSTメソッドは動作を伴うデータを送ることができます。
データを新規作成するときも使用します。

### PUTメソッド
PUTメソッドはデータの更新、アップロードをするときに使われます。データが存在しない場合は新規作成します。

### PATCHメソッド
PATCHメソッドはデータの更新時に使われます。


### DELETEメソッド
DELETEメソッドはデータの削除をする際に使用します。

## リクエストヘッダーとは
HTTPリクエストで使用されるHTTPヘッダーであり、メッセージの内容には関連しないもの。
HTTPヘッダーとはHTTPリクエストおよびHTTPレスポンスを構成する要素の一つ。HTTPヘッダーにはクライアントとサーバが通信する際の詳細や説明や制御情報などが格納されている。

## HTTPステータスコードとは
HTTPのレスポンスステータスコードは特定のHTTPリクエストが正常に完了したかどうかを示します。レスポンスは５つのクラスに分類されます。

### ・情報レスポンス(100-199)　
リクエストが処理中であることを表すステータスコード
### ・成功レスポンス(200-299)　
クライアントからのリクエストが正常に受付されたことを示すステータスコード
### ・リダイレクトメッセージ(300-399)　
リダイレクトが発生した際に表示されるステータスコード
### ・クライアントエラーレスポンス　
クライアントエラーが出たときに表示されるステータスコード

### ・200 OK
リクエスト成功
### ・201 Created
新たに作成されたリソースのURLが返される
### ・400 Bad Request
リクエストが不正
### ・404 Not Found 
未検出、ページが見つからなかった
### ・500 Internal Service Error
サーバー内部のエラー

## HTTPレスポンスの構成
HTTPレスポンスは

・ステータス行

・ヘッダーフィールド

・ボディ

の３つの要素で構成される

## レスポンスヘッダーとは
HTTPレスポンスの3つの要素のうちの１つ。レスポンス(返答)に関する情報を持ったヘッダー。

フィールド名:内容

の形式で構成される。

## レスポンスボディとは
HTTPレスポンスの3つの要素のうちの１つ。リクエストに対するサーバー応答内容の本文。Webサーバーへのリクエストに対するレスポンスの場合、HTML形式のテキストデータが記述される。

## JSONとは
JavaScript Object Notationの略で、JavaScriptにおけるオブジェクトの書き方を参考に作られたデータフォーマット(データの記述形式)のこと。幅広い環境で使用できるため、異なる言語、環境の間でデータの受け渡しや共有をするときに役立ちます。

優れている点

・CSVやXMLといったデータフォーマットと比べて読み書きしやすい

・処理が重くなりづらい

注意点

・データ構造の自由度が高い分複雑になりがち

・コメントを記載できない

## JSONを使ったデータ表現
```
[
{
  
  "id": "1", 
  
  "name": "yamada",
  
  "home_town": "Tokyo",
  
  "age": "25"},
  
  {"id": "2", 
  
  "name": "tanaka",
  
  "home_town": "Osaka", 
  
  "age": "22"
  
  }
  
]
```
