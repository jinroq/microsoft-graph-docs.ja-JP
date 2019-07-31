---
author: JeremyKelley
description: DriveItem のプライマリ ストリーム (ファイル) のコンテンツをダウンロードします。 file プロパティを持つ driveItem のみがダウンロード可能です。
ms.date: 09/10/2017
title: ファイルをダウンロードする
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6f5d836b5c5dbd382cbf11cf94fc0273515d4806
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957109"
---
# <a name="download-the-contents-of-a-driveitem"></a>DriveItem のコンテンツをダウンロードする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

DriveItem のプライマリ ストリーム (ファイル) のコンテンツをダウンロードします。 **file** プロパティを持つ driveItem のみがダウンロード可能です。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前          | 値  | 説明                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="example"></a>例

完全なファイルをダウンロードする例を示します。



# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

ファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。これは、DriveItem の `@microsoft.graph.downloadUrl` プロパティを通じて使用可能な URL と同じものです。

ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。

事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a>部分的な範囲のダウンロード

ファイルから部分的なバイトの範囲をダウンロードするには、[RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) で規定されているように、アプリで `Range` ヘッダーを使用します。`Range` ヘッダーは実際の `@microsoft.graph.downloadUrl` URL に追加する必要があり、`/content` の要求には追加しない点に注意してください。

<!-- { "blockType": "request", "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

これにより、ファイルからのバイトの要求範囲を含む `HTTP 206 Partial Content` 応答が返されます。範囲が生成できない場合、Range ヘッダーは無視され、ファイルの完全なコンテンツを含む `HTTP 200` 応答が返されます。

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

### <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
}
-->
