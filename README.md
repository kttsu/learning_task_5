## URLは、ウェブ上のリソースの場所を指し示すための統一された形式のアドレスです。
一般的に、プロトコル（http、httpsなど）、ホスト名、オプションでポート番号、パス、そしてクエリ文字列で構成されます。    

## クエリ文字列
クエリ文字列は、URLの末尾に続く、リソースに関する追加のデータやパラメータを含む文字列です。  
URLの末尾に **?** で始まり、キーと値のペアで構成されます。各ペアは **&** で区切られます。  
 - クエリ文字列の例:[Git hubをGoogl検索](https://www.google.com/search?q=github)  
  このURLの例では、Googleの検索エンジンを使用しています。**search** はリソースを表し、**q** が検索クエリを表し、 **github** が検索語を表すクエリパラメータです。

## パス変数（パスパラメーター）
URLのパス内に直接値を埋め込む方法です。  
通常はコロン **:** で始まります。これにより、変数部分に異なる値が入ります。
 - パス変数の例: [Git hubをユーザー検索](https://github.com/kttsu)  
   このURLの例では、GitHubのユーザー「kttsu」のページが表示しています。kttsuが特定のユーザーを識別するためのパス変数です。  
   つまり、ユーザーIDを変更することで、異なるユーザーのページにアクセスできます。

## クエリ文字列とパス変数の違い
クエリ文字列は **?** 以降の部分で、キーと値のペアで情報を渡し、リソースのフィルタリングやページネーションなどの検索条件を伝えるために使用されます。　　

一方、パス変数はパス内に値を埋め込む手段です。URL自体がリソースの一意の識別子を表す場合に使用され、リソースの取得や特定の操作に関連する情報を含みます。  

要するに、パス変数はリソースの一部であり、クエリ文字列はリソースに対する操作や検索条件を伝えるために使用されます。


## HTTPメソッド
HTTPメソッドは、HTTPリクエストの目的を示すための動詞です。主要なものにはGET、POST、PUT、PATCH、DELETEなどがあります。  
 - HTTPメソッドの意味:
  - GET: リソースの取得
  - POST: データの送信や新しいリソースの作成
  - PUT: リソースの作成または更新（全体を置き換え）
  - PATCH: リソースの部分的な更新
  - DELETE: リソースの削除
    
リクエストヘッダー:

定義: HTTPリクエストにおけるメタデータを含むヘッダー。クライアントがサーバーに対してさまざまな情報を送信するために使用されます。

HTTPステータスコード:

HTTPステータスコードは、ウェブサーバーからのHTTPリクエストに対するレスポンスの成否や種類を示す3桁の数字です。それぞれのステータスコードには特定の意味があり、クライアントや開発者に対してリクエストが成功したか、エラーが発生したか、あるいはリダイレクトが行われたかなどを伝えます。

一部の主要なHTTPステータスコード:

200 OK:

リクエストが成功したことを示します。これは通常、GETリクエストに対する正常な応答を表します。
201 Created:

リクエストが成功し、新しいリソースが作成されたことを示します。通常、POSTリクエストに使用されます。
400 Bad Request:

サーバーがリクエストを理解できない場合や、不正なリクエストが送信された場合に返されます。
404 Not Found:

要求されたリソースがサーバー上に見つからなかった場合に返されます。
500 Internal Server Error:

サーバーがリクエストを処理中にエラーが発生した場合に返されます。これは一般的にサーバー側の問題を示します。
レスポンスヘッダー:

レスポンスヘッダーは、HTTPレスポンスに関連するメタデータを含む部分です。これには、クッキー、コンテンツタイプ、サーバータイプなどが含まれます。ヘッダーは、レスポンスの情報や動作をクライアントに伝えるのに使用されます。

レスポンスボディ:

レスポンスボディは、HTTPレスポンスの実際のデータ部分です。これには、HTML、JSON、画像など、クライアントに返されるコンテンツが含まれます。成功したリクエストの場合、レスポンスボディには要求されたデータが含まれることがあります。エラーの場合は、エラーメッセージなどがレスポンスボディに含まれます。


JSON（JavaScript Object Notation）は、データの軽量なデータ交換フォーマットであり、人間が読み書きしやすく、機械がパースおよび生成しやすい特徴があります。JSONはプログラミング言語に依存せず、テキスト形式でデータを表現します。
