---
title: FeatureRolloutPolicy の更新
description: Featurerolloutpolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdbe19a401f10acead10884f02de5d380465e0a
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062155"
---
# <a name="update-featurerolloutpolicy"></a>Featurerolloutpolicy の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | FeatureRollout |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|String|このポリシーの説明。|
|displayName|String|このポリシーの表示名。|
|isAppliedToOrganization|Boolean|この機能ロールアウトポリシーを組織全体に適用する必要があるかどうかを示します。|
|isEnabled|Boolean|機能ロールアウトが有効になっているかどうかを示します。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a

Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
