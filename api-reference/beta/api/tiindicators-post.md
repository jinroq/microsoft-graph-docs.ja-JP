---
title: 脅威インテリジェンス指標の作成
description: 新しい tiIndicator を作成します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 990084b4e928527bbd43ee631489bc165d7f36f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868110"
---
# <a name="create-threat-intelligence-indicator"></a>脅威インテリジェンス指標の作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい[Tiindicator](../resources/tiindicator.md)オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | ThreatIndicators.ReadWrite.OwnedBy  |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

要求本文で、少なくとも1つの[メール](../resources/tiindicator.md#indicator-observables---email)、[ファイル](../resources/tiindicator.md#indicator-observables---file)、または観測可能な[ネットワーク](../resources/tiindicator.md#indicator-observables---network)を含む[tiindicator](../resources/tiindicator.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

> [!NOTE]
> ここに示す response オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
