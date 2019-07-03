---
title: 'securityAction: cancelSecurityAction'
description: セキュリティ操作をキャンセルします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3a4c71441b4d1af381057ea14fdce1a27512d69a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457353"
---
# <a name="securityaction-cancelsecurityaction"></a>securityAction: cancelSecurityAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

セキュリティ操作をキャンセルします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | サポートされていません。 |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | SecurityActions.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="examples"></a>例

次の例は、この API を呼び出す方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
