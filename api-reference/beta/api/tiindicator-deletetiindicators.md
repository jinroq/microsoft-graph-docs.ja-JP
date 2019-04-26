---
title: 'tiindicator: deletetiindicators'
description: 複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d5ceaa7e7c0402719b8ee202053da54ad235cc28
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335307"
---
# <a name="tiindicator-deletetiindicators"></a>tiindicator: deletetiindicators

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | ThreatIndicators.ReadWrite.OwnedBy |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型        | 説明 |
|:-------------|:------------|:------------|
|value|String collection| 削除する tiindicator `id`s のコレクションです。 |

## <a name="response"></a>応答

成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[resultinfo](../resources/resultinfo.md)コレクションオブジェクトを返します。

## <a name="examples"></a>例

次の例は、この API を呼び出す方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> [!NOTE]
> ここに示す response オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
