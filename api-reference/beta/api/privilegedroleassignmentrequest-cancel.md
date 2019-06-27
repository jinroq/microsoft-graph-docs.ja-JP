---
title: PrivilegedRoleAssignmentRequest のキャンセル
description: PrivilegedRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: 99b02ac432eab2e0fe8f2b860b92e03719404b2c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264156"
---
# <a name="cancel-privilegedroleassignmentrequest"></a>PrivilegedRoleAssignmentRequest のキャンセル

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を取り消します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess、AzureAD、および Directory.accessasuser.all。    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |


### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 Ok` 応答コードを返します。 応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を返します。

### <a name="error-codes"></a>エラー コード
この API は、標準の HTTP エラーコードを返します。 さらに、次の表に示すカスタムエラーコードを返します。

|エラー コード     | エラー メッセージ              |
|:--------------------| :---------------------|
| 400 BadRequest | RequestId を Null にすることはできません。 |
| 400 BadRequest | 要求 ID の要求が見つかりません。 |
| 400 BadRequest | 取り消しは、スケジュールされた状態と PendingApproval に対してのみ行うことができます。 |
| 403権限がありません | 要求者が取り消し通話を行うことが許可されていないか、または要求が見つかりません。 |

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
