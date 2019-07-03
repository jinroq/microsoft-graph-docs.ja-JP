---
title: Create groupLifecyclePolicy
description: 新しい groupLifecyclePolicy を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f022be2e393f10805e9d62c49a6dbfd8333d93e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442609"
---
# <a name="create-grouplifecyclepolicy"></a>Create groupLifecyclePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません |
|アプリケーション |  Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
