# <a name="create-onenote-pages"></a>OneNote ページの作成

**適用対象**: OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック

OneNote ページを作成する場合は、POST 要求を *pages* エンドポイントに送信します。次に例を示します。

`POST ../notes/sections/{id}/pages`

<br/>

ページを定義する HTML をメッセージ本文で送信します。 要求が成功すると、Microsoft Graph は 201 HTTP 状態コードを返します。


> **注:** セクション、セクション グループ、ノートブックを作成するために送信できる POST 要求の詳細については、[対話型 REST リファレンス](http://dev.onenote.com/docs)をご覧ください。


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>要求 URI の構築

POST 要求 URI を構築するには、サービス ルート URL から開始します。

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

次に、*pages* エンドポイントを追加します。

- **任意のセクション (セクション名で指定) にページを作成する**<br/><br/>`.../pages?sectionName=DefaultSection`

- **任意のセクション (ID で指定) にページを作成する**<br/><br/>`.../sections/{section-id}/pages` 

ユーザーの個人用ノートブックにページを作成する場合は、Microsoft Graph が提供する、既定のノートブックにページを作成するためのエンドポイントを使用することもできます。

- **既定のノートブックの既定のセクションにページを作成する**<br/><br/>`../pages` 



完全な要求 URI は、次に示す例のいずれかのようになります。

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先をご覧ください。

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a>*sectionName* URL パラメーターの使用

次に示すルールは、*sectionName* パラメーターを使用して、既定のノートブックの指名したセクションにページを作成するときに適用されます。

- 最上位のセクションのみを参照できます (セクション グループ内のセクションは参照できません)。

- 指定した名前のセクションが既定のノートブックに存在しない場合、そのセクションは API によって作成されます。 セクション名に使用できない文字は、「`? * \ / : < > | & # " % ~`」です。

- セクション名の照合では、大文字と小文字が区別されませんが、セクションが作成されるときには大文字と小文字が維持されます。そのため、"My New Section" はこのとおりに表示されますが、これ以降の POST では "my new section" も一致します。

- セクション名は、URL エンコードされている必要があります。たとえば、スペースは *%20* とエンコードされなければなりません。

- *sectionName* パラメーターは、`../notes/pages` のルートでのみ有効になります (`../notes/sections/{id}/pages` では無効です)。

セクションは存在しない場合に作成されるため、この呼び出しはアプリで作成するすべてのページに使用しても問題ありません。 セクションの名前はユーザーが変更する可能性もありますが、API は指定されたセクション名で新しいセクションを作成します。 

> **注:** API から返された、名前を変更したセクション内のページへのリンクは、引き続き元のページに到達します。 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>メッセージ本文の構築

ページのコンテンツを定義する HTML は、*入力 HTML* と呼ばれます。入力 HTML は、[標準の HTML および CSS のサブセット](#supported-html-and-css-for-onenote-pages)と、追加のカスタム属性をサポートしています。(**data-id** や **data-render-src** のようなカスタム属性は[入力および出力 HTML](onenote_input_output_html.md) で記述されます)。 

入力 HTML は、POST 要求のメッセージ本文で送信します。入力 HTML は、`application/xhtml+xml` または `text/html` コンテンツ タイプを使用して、メッセージ本文に直接含めて送信することも、マルチパート要求の "Presentation" 部分に含めて送信することもできます。 

次に示す例では、入力 HTML をメッセージ本文に直接含めて送信しています。

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="http://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

バイナリ データを送信する場合は、[マルチパート要求](#example-request)を使用する必要があります。 

> **注:** プログラミングを簡単にして、アプリでの一貫性を保つために、すべてのページの作成にマルチパート要求を使用できます。 マルチパート メッセージを作成するライブラリの使用をお勧めします。 これにより、無効な形式のペイロードを作成してしまう危険性が少なくなります。


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a>POST pages 要求の入力 HTML に対する要件と制限事項

入力 HTML を送信するときには、次に示す一般的な要件と制限事項に注意してください。  

- 入力 HTML は、UTF-8 でエンコードされた整形式の XHTML である必要があります。すべてのコンテナーの開始タグは、終了タグと一致する必要があります。すべての属性値は、二重引用符または一重引用符で囲む必要があります。<!--docs say MUST be encoded-->

- JavaScript コード (ファイルを含む) および CSS は削除されます。 

- HTML フォームは全体が削除されます。  

- Microsoft Graph は [HTML 要素のサブセット](#supported-html-and-css-for-onenote-pages)をサポートします。 

- Microsoft Graph は一般的な HTML 属性のサブセットとカスタム属性のセットをサポートします (ページの更新に使用される **data-id** 属性など)。 サポートされる属性については、「[入出力 HTML](onenote_input_output_html.md)」をご覧ください。


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a>OneNote ページでサポートされる HTML と CSS

すべての要素、属性、およびプロパティがサポートされるわけではありません (HTML4、XHTML、CSS、HTML5 などについて)。 Microsoft Graph は、ユーザーの OneNote の使用方法に適した、限定的な HTML のセットを受け入れます。 詳細については、「[ページでサポートされる HTML タグ](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages)」をご覧ください。 この参照先に示されていないタグは、無視されることがあります。

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

次に、Microsoft Graph でサポートされる基本的な要素の種類の一覧を示します。

- `<head>` と `<body>`</p>
- `<title>` と `<meta>` (ページのタイトルと作成日を設定する)</p>
- `<h1>` から `<h6>` (セクションの見出し用)</p>
- `<p>` (段落用)</p>
- `<ul>`、`<ol>`、および `<li>` (リストおよびリスト アイテム用)</p>
- `<table>`、`<tr>`、および `<td>` (入れ子になったテーブルを含む)</p>
- `<pre>` (書式設定済みのテキスト用であり、空白と改行が維持される)</p>
- `<b>` と `<i>` (太字および斜体文字スタイル用)</p>

Microsoft Graph は、ページの作成時に入力 HTML の意味内容と基本的構造を維持しますが、サポートされている HTML および CSS のセットを使用するように入力 HTML を変換します。 OneNote に存在しない機能は変換されないため、ソース HTML では認識されない可能性があります。 


<a name="example"></a>

## <a name="example-request"></a>要求の例

ここに示すマルチパート要求の例では、イメージと埋め込みファイルが含まれたページを作成します。 必須の **Presentation** パーツには、ページを定義する入力 HTML が含まれています。 **imageBlock1** パーツにはバイナリ イメージ データが含まれ、**fileBlock1** にはバイナリ ファイル データが含まれています。 データ パーツには、Microsoft Graph が OneNote ページに[画像として HTML をレンダリングする](onenote_images_files.md#add-an-image-using-binary-data)場合の HTML を含めることもできます。 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

複数イメージやその他のファイルを含むページを作成する方法示す例については、「[画像とファイルを追加する](onenote_images_files.md)」、および[チュートリアル](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-tutorial)と[サンプル](https://github.com/onenotedev)を参照してください。また、[絶対配置要素の作成](onenote-abs-pos.md)方法、[ノート シールの使用](onenote-note-tags.md)方法と、名刺キャプチャ、オンラインのレシピ一覧およびオンラインの製品一覧の[データ抽出](onenote-extract-data.md)方法について調べてください。

Microsoft Graph は、マルチパート メッセージ本文の CRLF 改行など、一部の書式設定については厳密です。 無効な形式のペイロードを作成してしまう危険性を少なくするために、マルチパート メッセージはライブラリを使用して作成してください。 

無効な形式のペイロードに関する 400 状態を受信した場合は、改行と空白の書式を確認し、エンコーディングの問題について調べます。 たとえば、`charset=utf-8` を使用してみてください (例: `Content-Type: text/html; charset=utf-8`)。

[入力 HTML に対する要件と制限事項](#requirements-and-limitations-for-input-html-in-post-pages-requests) および [POST 要求のサイズ制限](onenote_images_files.md#size-limitations-for-post-pages-requests)をご覧ください。


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a>*POST pages* 要求の要求情報と応答情報

| 要求データ | 説明 |  
|------|------|  
| プロトコル | すべての要求は SSL/TLS HTTPS プロトコルを使用します。 |  
| 承認ヘッダー | <p>`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</p><p>これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions_reference.md)」を参照してください。</p> |  
| Content-Type ヘッダー | <p>HTML コンテンツの `text/html` または `application/xhtml+xml`。メッセージ本文またはマルチパート要求の必須の "Presentation" パートで直接送信します。</p><p>マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。`{part-boundary}` は、各データ パートの開始と終了を伝える文字列です。</p> |  
| Accept ヘッダー | `application/json` | 

<br/>

| 応答データ | 説明 |  
|------|------|  
| 成功コード | 201 HTTP ステータス コード。 |  
| 応答本文 | JSON 形式での新しいページの OData 表現。 |  
| エラー | 要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトでエラーを返します。 |  
| Location ヘッダー | 新しいページのリソース URL。 |  
| X-CorrelationId ヘッダー | 要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。 |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Microsoft Graph サービスのルート URL の構築

Microsoft Graph サービスのルート URL は、Microsoft Graph へのすべての呼び出しで次の形式を使用します。

`https://graph.microsoft.com/{version}/me/onenote/`  

URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。 安定した運用コードには `v1.0` を使用します。 開発中の機能を試すには `beta` を使用します。 ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。 

現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。 


<a name="permissions"></a>

## <a name="permissions"></a>アクセス許可

OneNote ページを作成するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。

次から選択します。

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」をご覧ください。




<a name="see-also"></a>

## <a name="see-also"></a>関連項目

- [画像とファイルを追加する](onenote_images_files.md)
- [絶対配置要素を作成する](onenote-abs-pos.md)  
- [データを抽出する](onenote-extract-data.md)
- [ノート シールを使用する](onenote-note-tags.md)
- [OneNote との統合](integrate_with_onenote.md)
- [OneNote の開発者ブログ](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Stack Overflow 掲載の OneNote の開発に関する質問](http://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub のリポジトリ](http://go.microsoft.com/fwlink/?LinkID=390178)  


