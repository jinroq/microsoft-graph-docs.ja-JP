---
title: PrivilegedRoleAssignmentRequest を作成します。
description: Privilegedroleassignmentrequest オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521069"
---
# <a name="create-privilegedroleassignmentrequest"></a>PrivilegedRoleAssignmentRequest を作成します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。 

| プロパティ     | 型    |  説明|
|:---------------|:--------|:----------|
|roleId|String|ロールの ID です。 必須。|
|type|String|表す、ロールの割り当ての操作の種類です。 値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。 必須です。|
|assignmentState|String|割り当ての状態です。 値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。 可能な値は、``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired` です。 必須です。|
|理由|String|理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。|
|Schedule|[governanceSchedule](../resources/governanceschedule.md)|役割の割り当て要求のスケジュールです。|

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトです。

### <a name="error-codes"></a>エラー コード
この API 規格を取得する HTTP エラー コードです。 さらに、次の表に記載されているエラー コードを返すことです。

|エラー コード     | エラー メッセージ              | 
|:--------------------| :---------------------|
| 400 BadRequest | RoleAssignmentRequest プロパティが NULL をしました |
| 400 BadRequest | RoleAssignmentRequest オブジェクトを逆シリアル化できません。 |
| 400 BadRequest | RoleId は、必要があります。 |
| 400 BadRequest | スケジュールの開始日は指定する必要があり、今よりも大きい必要があります。 |
| 400 BadRequest | このユーザー、ロール、およびスケジュールの種類のスケジュールが既に存在します。 |
| 400 BadRequest | 既に保留中の承認は、このユーザー、ロール、および承認の種類に存在します。 |
| 400 BadRequest | リクエスターの理由はされていません。 |
| 400 BadRequest | リクエスターの理由は、500 文字未満にする必要があります。 |
| 400 BadRequest | 昇格期間は、0.5 の間で、{の設定} からである必要があります。 |
| 400 BadRequest | スケジュールのアクティブ化と要求との間の重複があります。 |
| 400 BadRequest | ロールが既にアクティブになっています。 |
| 400 BadRequest | GenericElevateUserToRoleAssignments: Tickting の情報は必要し、ライセンス認証プロセスで指定されていません。 |
| 400 BadRequest | スケジュールのアクティブ化と要求との間の重複があります。 |
| 403 許可されていません。 | 昇格時に、複数要素の認証が必要です。 |
| 403 許可されていません。 | 昇格のため許可されていません。 |

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a>応答
応答の例を次に示します。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
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
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
