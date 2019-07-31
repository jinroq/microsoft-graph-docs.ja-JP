---
author: JeremyKelley
description: DriveItem のメタデータを、ID またはパスで更新します。
ms.date: 09/10/2017
title: ファイルまたはフォルダーを更新する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0fa3002a81310b025c51a4ff52930d3b9087c155
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956941"
---
# <a name="update-driveitem-properties"></a>DriveItem プロパティを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。

別の親に[アイテムを移動](driveitem-move.md)するために更新を使用することもできます。その場合は、アイテムの **parentReference** プロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前          | 型   | 説明                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。 |

## <a name="request-body"></a>要求本文

要求本文で、更新すべきプロパティの値を指定します。

要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。
最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。

## <a name="example"></a>例

この例では、DriveItem リソースを「new-file-name.docx」という名前に変更します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

成功した場合、このメソッドは応答本文で [driveItem][item-resource] リソースを返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
}
-->
