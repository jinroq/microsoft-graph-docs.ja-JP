---
title: Certificateベース Authconfiguration の作成
description: この API を使用して、新しい Certificateベース Authconfiguration を作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc78cd5a2de6a8ce1b44dd346c6c19ad8741736f
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667655"
---
# <a name="create-certificatebasedauthconfiguration"></a>Certificateベース Authconfiguration の作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい[Certificateベース Authconfiguration](../resources/certificateBasedAuthConfiguration.md)オブジェクトを作成します。

> [!NOTE]
> **Certificateベース Authconfiguration**のインスタンスは1つしか作成できません (コレクションには1つのメンバーしか指定できません)。 常に、値が ' 29728ade-6ae4-4ee9-9103-412912537da5 ' の固定 ID を持っています。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | 組織の ReadWrite |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション    | 組織の ReadWrite |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | ベアラー {トークン} |
| Content-Type | application/json |

## <a name="request-body"></a>要求本文

[Certificateベース Authconfiguration](../resources/certificatebasedauthconfiguration.md)オブジェクトを作成するには、次のプロパティが必要です。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|certificateAuthorities| [Certificateauthority](../resources/certificateauthority.md)コレクション |信頼された証明書チェーンを作成する証明機関のコレクション。  コレクションの各メンバーには、**証明書**と**isrootauthority**のプロパティが含まれている必要があります。 |

## <a name="response"></a>応答

成功した場合、この`201 Created`メソッドは応答コードと、応答本文で新しい[Certificateベース authconfiguration](../resources/certificatebasedauthconfiguration.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
