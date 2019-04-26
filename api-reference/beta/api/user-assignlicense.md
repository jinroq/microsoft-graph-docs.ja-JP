---
title: assignLicense
description: ユーザーのライセンスを追加または削除して、Microsoft クラウド製品の使用を有効または無効にします。 たとえば、組織には100ライセンスを持つ Office 365 Enterprise E3 サブスクリプションがあり、この要求はそれらのライセンスの1つを特定のユーザーに割り当てます。 また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。 サブスクリプションとライセンスの詳細については、Technet の記事を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9946a7ac53a0e0e8b90a31fd4767bcc0549468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547992"
---
# <a name="assignlicense"></a>assignLicense

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのライセンスを追加または削除して、Microsoft クラウド製品の使用を有効または無効にします。 たとえば、組織には100ライセンスを持つ Office 365 Enterprise E3 サブスクリプションがあり、この要求はそれらのライセンスの1つを特定のユーザーに割り当てます。 また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。 サブスクリプションとライセンスの詳細については、 [Technet の記事](https://technet.microsoft.com/en-us/library/mt765146.aspx)を参照してください。

ディレクトリで利用可能なサブスクリプションを取得するには、 [get subscribedSkus 要求](subscribedsku-list.md)を実行します。 

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
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|追加するライセンスを指定する[assignedLicense](../resources/assignedlicense.md)オブジェクトのコレクションです。 [assignedLicense](../resources/assignedlicense.md)オブジェクトの**disabledPlans**プロパティを設定することによって、ライセンスに関連付けられた serviceplans を無効にすることができます。|
|removeLicenses|Guid|削除するライセンスを識別する skuids のコレクション。|

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で更新された[ユーザー](../resources/user.md)オブジェクトを返します。

## <a name="example"></a>例
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

## <a name="example"></a>例
ユーザーからライセンスを削除します。

##### <a name="request"></a>要求
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
どちらの例でも、応答は更新されたユーザーオブジェクトです。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
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
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
