---
title: PublishedResource を onPremisesAgentGroup に割り当てます。
description: '**Publishedresource**オブジェクトを**onPremisesAgentGroup**オブジェクトに割り当てます。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ec20b1208906129e5559307fc347e9d39c6dd7e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840969"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a>PublishedResource を onPremisesAgentGroup に割り当てます。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Publishedresource](../resources/publishedresource.md)オブジェクトを[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトに割り当てます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:--------------------------------------|:---------------------------------------------------------|
| 委任 (職場または学校のアカウント)     | OnPremisesPublishingProfiles |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | ベアラー {トークン} |

## <a name="request-body"></a>要求本文

要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[publishedresource](../resources/publishedresource.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
Content-type: application/json

```http
{
 "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2B032383-897C-42BA-917E-700B6890BDC3/"
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
HTTP/1.1 204
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
