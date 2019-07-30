---
author: JeremyKelley
ms.author: jeremyke
title: バンドルにアイテムを追加する
description: ドライブ項目のバンドルにアイテムを追加する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e6706fecd425162345e718fd43f6dc44e7c6b9db
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932850"
---
# <a name="add-item-to-a-bundle"></a>バンドルにアイテムを追加する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ドライブから[バンドル][]に、追加のドライブ[項目][]を追加します。

[バンドル]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。                             |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All   |
|アプリケーション          | サポートされていません。                                           |

## <a name="http-request"></a>HTTP 要求

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明  |
|:------------- |:------------ |
| Authorization | ベアラー \{トークン\}。 必須です。 |

## <a name="request-body"></a>要求本文

要求本文には、バンドルの子コレクションに追加する必要があるアイテムの識別子が含まれています。

## <a name="response"></a>応答

成功した場合、応答`204 No Content`はになります。

エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。

## <a name="example"></a>例

### <a name="request"></a>要求

この要求は、指定したバンドルに既存のアイテムを追加します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->
