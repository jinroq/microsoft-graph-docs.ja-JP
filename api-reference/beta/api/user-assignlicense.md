---
title: assignLicense
description: 追加またはユーザーを有効にするか、マイクロソフトのクラウド サービスの使用を無効にするためのライセンスを削除します。 たとえば、組織は、100 のライセンスを持つ、Office 365 エンタープライズ E3 サブスクリプションを持つことができ、この要求がこれらのライセンスのいずれかを特定のユーザーに割り当てます。 有効にし、サブスクリプションに関連付けられている特定のプランを無効にできます。 サブスクリプションとライセンスに関する詳細については、この Technet の記事を参照してください。
ms.openlocfilehash: ecfe1f97e2e951998e0a62eea68412279eae524f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074515"
---
# <a name="assignlicense"></a>assignLicense

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

追加またはユーザーを有効にするか、マイクロソフトのクラウド サービスの使用を無効にするためのライセンスを削除します。 たとえば、組織は、100 のライセンスを持つ、Office 365 エンタープライズ E3 サブスクリプションを持つことができ、この要求がこれらのライセンスのいずれかを特定のユーザーに割り当てます。 有効にし、サブスクリプションに関連付けられている特定のプランを無効にできます。 サブスクリプションとライセンスに関する詳細については、この[Technet の記事](https://technet.microsoft.com/en-us/library/mt765146.aspx)を参照してください。

ディレクトリで利用可能なサブスクリプションを取得するには、 [subscribedSkus 要求の取得](subscribedsku-list.md)を実行します。 

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.ReadWrite.All、Directory.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|追加するのにはライセンスを指定する[assignedLicense](../resources/assignedlicense.md)オブジェクトのコレクションです。 [AssignedLicense](../resources/assignedlicense.md)オブジェクトの**disabledPlans**プロパティを設定することにより、ライセンスに関連する servicePlans を無効にすることができます。|
|removeLicenses|Guid|削除するライセンスを識別する skuIds のコレクションです。|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本体の更新された[ユーザー](../resources/user.md)オブジェクトです。

## <a name="example"></a>使用例
ユーザーにライセンスを追加します。
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a>使用例
ユーザーからライセンスを削除します。

#####<a name="request"></a>要求
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a>応答
どちらの例では、応答は、更新されたユーザー オブジェクトです。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
