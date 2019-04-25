---
title: 'privilegedRole: selfactivate'
description: 要求者に割り当てられている役割をアクティブ化します。
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546592"
---
# <a name="privilegedrole-selfactivate"></a>privilegedRole: selfactivate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

要求者に割り当てられている役割をアクティブ化します。

>**注:** 2018年12月有効になると、この API はサポートされなくなり、使用されなくなります。 代わりに、 [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md)を使用します。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

リクエスターは、自分に```selfActivate```割り当てられている役割に対してのみ呼び出すことができます。
 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

これは``<id>`` 、ターゲットの役割 ID であることに注意してください。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|したがっ|string|省略可能。 この役割のライセンス認証の理由についての説明。|
|duration|string|省略可能。 有効な値は```min``` 、(最小ライセンス認証の```default```期間)、(ロールの既定のライセンス認証の期間)、または倍精度の値を使用してライセンス認証の時間数を指定します。 指定した期間は、役割の設定から、役割のアクティブ化の期間より長くすることはできません。 |
|ticketNumber|string|省略可能。 この役割のライセンス認証の追跡に使用されるチケット番号。|
|ticketSystem|string|省略可能。 チケットシステム。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。

テナントが PIM に登録されている必要があることに注意してください。 それ以外の場合、HTTP 403 の禁止状態コードが返されます。
## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
