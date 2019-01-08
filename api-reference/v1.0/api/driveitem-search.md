---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルを検索する
ms.openlocfilehash: 591aa271a9e5a1d9ae69af2e5d8f6ea9ba7fe74b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748221"
---
# <a name="search-for-a-driveitems-within-a-drive"></a>ドライブ内の DriveItems を検索する

クエリと一致するアイテムを対象にアイテムの階層を検索します。
フォルダー階層内、ドライブ全体、または現在のユーザーと共有されるファイル内で検索できます。

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
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="function-parameters"></a>関数パラメーター

| Parameter | 種類  | 説明                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| q  | string | アイテムの検索に使用するクエリ テキスト。値は、ファイル名、メタデータ、およびファイルのコンテンツを含む複数のフィールドに渡って照合できます。 |

## <a name="example"></a>例

### <a name="request"></a>要求

ここでは、現在のユーザーの OneDrive を検索する要求の例を示します。

<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a>応答

このメソッドは、検索条件に一致する [DriveItems](../resources/driveitem.md) のコレクション含んでいるオブジェクトを返します。アイテムが見つからない場合は、空のコレクションが返されます。

一致が多すぎる場合は、応答はページ化され、**@odata.nextLink** プロパティには、後続の結果ページへの URL が含まれます。`$top` クエリ パラメーターを使用すると、ページ内のアイテム数を指定できます。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a>ユーザーがアクセスできるアイテムの検索

ドライブ内のアイテムの検索に加えて、アプリでは現在のユーザーと共有されるアイテムを含めるように、検索範囲を広げることができます。検索範囲を広げるには、[Drive](../resources/drive.md) リソースの **search** メソッドを使用します。

### <a name="example"></a>例

<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a>応答

**ドライブ** リソースからの検索時の応答には、ドライブの外部のアイテム (現在のユーザーと共有されているアイテム) が含まれていることがあります。こうしたアイテムには、それらが対象のドライブの外部に保存されていることを示す、[**remoteItem**](../resources/remoteitem.md) ファセットが含まれます。 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "parentReference": { "driveId": "s!1020101jlkjl12lx" } }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search"
} -->
