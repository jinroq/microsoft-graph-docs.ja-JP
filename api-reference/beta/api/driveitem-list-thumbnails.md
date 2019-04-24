---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーのサムネイルを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 68c1adf275a6a8720aab4df638f69c7162e301a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454378"
---
# <a name="list-thumbnails-for-a-driveitem"></a>DriveItem のサムネイルを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。

DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。

OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。

* アイテムの利用可能なサムネイルを列挙する
* アイテムの 1 つのサムネイルを取得する
* サムネイルのコンテンツを取得する
* 1 つの要求で複数のアイテムのサムネイルを取得する
* カスタムのサムネイル サイズを取得する
* アイテムのカスタム サムネイルをアップロードする
* カスタムのアップロード済みサムネイルが存在するかどうかを確認する


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
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例

次は、現在のユーザーの OneDrive 内のアイテムで使用可能なサムネイルを取得する要求の例です。

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

このアイテムの使用可能な **thumbnailSets** の配列が返されます。 ドライブにあるすべてのアイテムは、0 個以上のサムネイルを保持できます。

**注:**_select_ クエリ文字列パラメーターを使用すると、**ThumbnailSet** で返されるサムネイルのサイズを制御できます。 たとえば、`/thumbnails?select=medium` では、中サイズのサムネイルのみを取得します。


### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="get-a-single-thumbnail"></a>1 つのサムネイルを取得する

1 つのサムネイルとサイズのメタデータを、要求で直接アドレス指定して取得します。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a>パス パラメーター

| 名前         | 型   | 説明                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| **item-id**  | string | 参照されるアイテムの一意識別子。                                           |
| **thumb-id** | number | サムネイルのインデックス (通常 0-4)。 カスタム サムネイルがある場合は、そのインデックスは 0 になります。 |
| **size**     | string | 要求されたサムネイルのサイズ。 これは、後述する標準サイズか、カスタム サイズのいずれかになります。 |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a>サムネイルのバイナリ コンテンツを取得する

サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接取得できます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a>応答

サービスは、サムネイルの URL へのリダイレクトで応答します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

サムネイル URL はキャッシュ対応です。 この URL は、新しいサムネイルの生成を必要とする方法でアイテムを変更する場合に変更されます。


## <a name="getting-thumbnails-while-listing-driveitems"></a>DriveItems を一覧表示する際にサムネイルを取得する

表示する DriveItem リソースのリストを取得する場合、_$expand_ クエリ文字列パラメーターを使用して、それらのリソースのサムネイルも含めることができます。
これによりアプリは、複数の要求を実行することなく、サムネイルとアイテムを 1 つの要求で取得することができます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a>応答

サービスは、DriveItems とそのサムネイルのリストで応答します。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-values"></a>サイズの値

次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。

| 名前           | 解決方法  | 縦横比 | 説明                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 longest  | Original     | 圧縮率の高い小さなサムネイルは、正方形にトリミングされます。 |
| `medium`       | 176 longest | Original     | OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。         |
| `large`        | 800 longest | 元の比率     | サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。               |
| `smallSquare`  | 96x96       | 正方形にトリミング  | 小さな正方形のサムネイル                                               |
| `mediumSquare` | 176x176     | 正方形にトリミング  | 小さな正方形のサムネイル                                               |
| `largeSquare`  | 800x800     | 正方形にトリミング  | 大きな正方形のサムネイル                                               |

## <a name="requesting-custom-thumbnail-sizes"></a>カスタムのサムネイル サイズを要求する

定義済みのサイズに加えて、アプリでは、先頭に `c` を付けたサムネイルのディメンションを指定することで、カスタムのサムネイル サイズを要求できます。
たとえば、アプリで 300x400 のサムネイルが必要な場合は、そのサイズを次に示すように要求できます。

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

これにより、選択したカスタムのサムネイル サイズのみの応答が返されます。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

要求するサムネイルのサイズの後ろに、次に示すオプションを指定できます。

### <a name="examples-of-custom-identifiers"></a>カスタム識別子の例

| サムネイル識別子 | 解像度             | 縦横比 | 説明                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| c300x400             | 300x400 のボックスに制限されます | Original     | 300x400 ピクセルのボックスに収まるサムネイルを生成します。縦横比は維持されます。                                                                 |
| c300x400_Crop        | 300x400                | トリミング      | 300x400 ピクセルのサムネイルを生成します。 これは、300x400 のボックスに収まるように画像のサイズを変更し、このボックスに収まらない部分をトリミングするように動作します。 |

**注:** 返されるサムネイルのピクセル ディメンションは要求されたものと正確に一致しないことがありますが、縦横比は一致します。
サムネイルがすでに存在しており、要求された解像度に簡単に拡大縮小できる場合、要求されたものよりも大きいサムネイルが返されることがあります。

## <a name="remarks"></a>備考

**注:** OneDrive for Business および SharePoint の場合:

次の呼び出しを使用したサムネイル コレクションの展開は機能しません: 

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

サムネイルは、SharePoint Server 2016 ではサポートされていません。

### <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
