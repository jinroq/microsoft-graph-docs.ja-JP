---
title: 所有者を作成する
description: この API を使用して、新しい所有者を作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3a0270d18856b32b6298ab66740ec754123dbbd8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439589"
---
# <a name="create-owner"></a>所有者を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この API を使用して、新しい所有者を作成します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Application.readwrite.ownedby とディレクトリ。すべての、およびすべてのディレクトリを取得します。すべてのアプリケーション |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
