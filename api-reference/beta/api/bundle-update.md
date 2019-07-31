---
author: JeremyKelley
ms.author: jeremyke
title: バンドルを更新する
description: ドライブ項目のバンドルを更新する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e3d7e684b9987aa5bcd4c601654956c84b6f7904
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944816"
---
# <a name="update-bundle"></a>バンドルの更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ID を使用して、[ドライブ項目]の[ドライブ項目]の[バンドル][]のメタデータを更新します。
次のメタデータのみを更新できます。

* バンドル名
* アルバム`coverImageItemId` (該当する場合)

その他の変更要求は無視されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。                             |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All   |
|アプリケーション          | サポートされていません。                                           |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明  |
|:------------- |:------------ |
| Authorization | ベアラー \{トークン\}。 必須。 |
| if-match      | eTag. 省略可能。 この要求ヘッダーが含まれており、指定された eTag が buncle の現在の eTag と`412 Precondition Failed`一致しない場合は、応答が返されます。

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

## <a name="response"></a>応答

成功した場合、このメソッドは、応答本文で更新されたバンドルを表す、[ドライブ項目][]リソースを返します。

エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。

## <a name="example"></a>例

この例では、バンドルの名前を変更します。

### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

ここに示す response オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。


[バンドル]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath": "Bundles/Update"
} -->
