---
title: inferenceClassificationOverride の更新
description: '指定どおり**** に優先受信トレイの設定の [分類] フィールドを変更します。 '
localization_priority: Normal
ms.openlocfilehash: 0cb3eab7f8a4efece8099ca8f65577d8a06b18d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500847"
---
# <a name="update-inferenceclassificationoverride"></a>inferenceClassificationOverride の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定どおり**** に優先[受信トレイ](../resources/manage-focused-inbox.md)の設定の [分類] フィールドを変更します。 

[InferenceClassicationOverride](../resources/inferenceclassificationoverride.md) インスタンスのその他のフィールドの変更には、PATCH を使用できません。 

送信者にオーバーライドがあり、その送信者が表示名を変更すると、既存のオーバーライドで [POST](inferenceclassification-post-overrides.md) を使用して [名前] フィールドの更新を実施できます。

送信者にオーバーライドがあり、その送信者が SMTP アドレスを変更すると、既存のオーバーライドを[削除](inferenceclassificationoverride-delete.md)して、新しい SMTP アドレスで新しくオーバーライドを[作成](inferenceclassification-post-overrides.md)することが、この送信者のオーバーライドを「更新」する唯一の方法になります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.ReadWrite    |
|アプリケーション | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求の本文内に、**classifyAs** の新しい値を指定します。最適なパフォーマンスを得るためには、変更されない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|classifyAs|string| 特定の差出人からの着信メッセージを常時分類する方法を指定します。可能な値は、`focused`、`other` です。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下の例は、SMTP アドレス randiw@adatum.onmicrosoft.com のオーバーライドのものであり、`other` から `focused` に変更します。

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassificationoverride-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
