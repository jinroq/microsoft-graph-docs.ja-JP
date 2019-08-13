---
title: OnPremisesAgent を onPremisesAgentGroup に割り当てる
description: OnPremisesAgent を onPremisesAgentGroup に割り当てます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 000385e1b2faad98bee217d2709f5516ea40b6b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342643"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a>OnPremisesAgent を onPremisesAgentGroup に割り当てる

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトに[onPremisesAgent](../resources/onpremisesagent.md)を割り当てます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | OnPremisesPublishingProfiles |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | ベアラー {トークン} |

## <a name="request-body"></a>要求本文

要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトへの OData 参照の JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトへの OData 参照の JSON 表記を指定します。

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
