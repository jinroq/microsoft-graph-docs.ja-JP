---
title: 'groupLifecyclePolicy: renewGroup'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: d07025b076e78193f1c712d70892bd5a262ea2a2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262735"
---
# <a name="grouplifecyclepolicy-renewgroup"></a>groupLifecyclePolicy: renewGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。

> **注:** V 1.0 で[は、グループリソースを使用して更新要求を行い](/graph/api/group-renew?view=graph-rest-1.0)ます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。
 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All または Directory.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません |
|アプリケーション | Group.ReadWrite.All または Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型 | 説明 |
|:---------------|:--------|:----------|
|groupId|Guid| 更新するグループの id。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
