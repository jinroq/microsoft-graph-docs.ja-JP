# <a name="create-page"></a>page を作成する

既定のノートブックの既定のセクションで OneNote の新しいページを作成します。

既定のノートブックの別のセクションにページを作成する場合は、`sectionName` クエリ パラメーターを使用できます。例: `../onenote/pages?sectionName=My%20section`

`POST /onenote/pages` の操作は、現在のユーザーの既定のノートブックでページを作成する場合のみに使用します。他のノートブックを対象とする場合は、[指定されたセクションでページを作成](../api/section_post_pages.md)できます。           
## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。  

Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a>要求ヘッダー  
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | string | HTML コンテンツを表す `text/html` または `application/xhtml+xml` (マルチパート要求の必須の "Presentation" パートを含む)。マルチパート要求では `multipart/form-data; boundary=your-boundary` コンテンツ タイプを使用します。 |

## <a name="request-body"></a>要求本文
要求本文には、ページの HTML コンテンツを指定します。

本文には、要求本文に直接入力した HTML を含めることができます。または、例に示すようにマルチパート メッセージ形式を含めることもできます。バイナリ データを送信する場合は、マルチパート要求を送信する必要があります。

## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新規 [page](../resources/page.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

`../onenote/pages` のパスで、`sectionName` クエリ パラメーターを使用して、特定のノートブックの指定したセクションにページを作成できます。例: `../onenote/pages?sectionName=My%20section`。セクションが存在しない (または名前が変更された) 場合、API は新しいセクションを作成します。

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
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
##### <a name="response"></a>応答
以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->