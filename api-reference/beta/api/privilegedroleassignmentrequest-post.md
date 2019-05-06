---
title: PrivilegedRoleAssignmentRequest を作成する
description: Privilegedroleassignmentrequest オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: d963bd1cc103928675890aa7ddeccd5fd27594c0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593766"
---
# <a name="create-privilegedroleassignmentrequest"></a>PrivilegedRoleAssignmentRequest を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess、AzureAD、および Directory.accessasuser.all。    |
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
要求本文で、 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。 

| プロパティ     | 型    |  説明|
|:---------------|:--------|:----------|
|roleId|String|ロールの ID。 必須。|
|type|String|役割の割り当てに対する操作の種類を表します。 値は次の`AdminAdd`ようになります。「ユーザーを役割に追加する」。`UserAdd`: ユーザーが役割の割り当てを追加します。 必須です。|
|割り当ての状態|String|割り当ての状態を指定します。 この値は、 `Eligible`管理者に`Active`よって直接割り当てら`Active`れている場合、またはユーザーによる資格のある割り当てに対してアクティブ化されている場合に、対象となる割り当てに使用できます。 使用可能な値は、``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired` です。 必須です。|
|したがっ|String|監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|役割の割り当て要求のスケジュール。|

## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを返します。

### <a name="error-codes"></a>エラー コード
この API は、その標準の HTTP エラーコードを返します。 また、次の表に示されているエラーコードを返すこともできます。

|エラー コード     | エラー メッセージ              | 
|:--------------------| :---------------------|
| 400 BadRequest | Role割り当て要求プロパティが NULL でした |
| 400 BadRequest | Role割り当て要求オブジェクトをシリアル化解除できません。 |
| 400 BadRequest | RoleId が必要です。 |
| 400 BadRequest | スケジュールの開始日を指定する必要があります。これより大きい値を指定する必要があります。 |
| 400 BadRequest | このユーザー、役割、およびスケジュールの種類に対するスケジュールが既に存在します。 |
| 400 BadRequest | このユーザー、ロール、承認の種類に対して、保留中の承認が既に存在します。 |
| 400 BadRequest | 要求者の理由がありません。 |
| 400 BadRequest | 要求者の理由は、500文字未満である必要があります。 |
| 400 BadRequest | 昇格期間は0.5 と {from 設定} の間である必要があります。 |
| 400 BadRequest | スケジュールされたライセンス認証と要求の間に重複があります。 |
| 400 BadRequest | このロールは、あらかじめアクティブ化されています。 |
| 400 BadRequest | GenericElevateUserToRoleAssignments: Tickting 情報は必須であり、アクティブ化プロセスでは提供されていません。 |
| 400 BadRequest | スケジュールされたライセンス認証と要求の間に重複があります。 |
| 403権限がありません | 昇格には多要素認証が必要です。 |
| 403権限がありません | 昇格の代理人は許可されていません。 |

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
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/post_privilegedroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_privilegedroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
