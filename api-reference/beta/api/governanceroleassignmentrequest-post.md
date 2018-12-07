---
title: GovernanceRoleAssignmentRequest を作成します。
description: 役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。
ms.openlocfilehash: 775cc8e22e7d273bfe387e5be2cc183d3d919a38
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191173"
---
# <a name="create-governanceroleassignmentrequest"></a>GovernanceRoleAssignmentRequest を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。

| 操作       | Type | 
|:---------------|:----------|
| 役割の割り当てを割り当てる| AdminAdd |
| 対象のロール割り当てを有効化します。| UserAdd | 
| アクティブ化されたロール割り当てを非アクティブ化します。| UserRemove | 
| 役割の割り当てを削除します。| AdminRemove |
| 役割の割り当てを更新します。| AdminUpdate |
| 自分の役割の割り当てを拡張する要求| UserExtend | 
| 役割の割り当てを拡張します。| AdminExtend | 
| [期限切れのロールの割り当てを更新する要求| UserRenew | 
| 期限切れのロール割り当てを更新します。| AdminRenew | 

 
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>要求本文
要求の本文には、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。 

| プロパティ     | 種類    |必須|  説明|
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|リソースの ID。|
|roleDefinitionId|String|はい|役割の定義の ID です。|
|subjectId|String|はい|サブジェクトの ID です。|
|assignmentState|String|はい|割り当ての状態です。 値は、``Eligible``と``Active``。|
|type|String|はい|要求の種類。 値は、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、`AdminRenew`と`AdminExtend`。|
|理由|String| |理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。|
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)| | 役割の割り当て要求のスケジュールです。 要求の種類の`UserAdd`、 `AdminAdd`、`AdminUpdate`と`AdminExtend`、これは必須です。|

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。

### <a name="error-codes"></a>エラー コード
この API では、標準の HTTP エラー コードを返します。 さらに、また次の表に記載されているエラー コードを返します。

|エラー コード     | エラー メッセージ              | 詳細 |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleNotFound    | `roleDefinitionId` 、要求の本文が見つかりません指定します。
| 400 BadRequest | ResourceIsLocked    | 状態の要求の本文に記載されているリソースは、`Locked`と、役割の割り当て要求を作成することはできません。
| 400 BadRequest | SubjectNotFound    | `subjectId` 、要求の本文が見つかりません指定します。
| 400 BadRequest | PendingRoleAssignmentRequest    | あるシステムで保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を既に存在します。
| 400 BadRequest | RoleAssignmentExists    | 既に要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在します。
| 400 BadRequest | RoleAssignmentDoesNotExist    | 更新または拡張するように要求した[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。
| 400 BadRequest | RoleAssignmentRequestPolicyValidationFailed | [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は、社内ポリシーを満たしていないと、作成することはできません。

## <a name="examples"></a>例
次の例では、この API を使用する方法を示しています。

### <a name="example-1"></a>例 1
この例では、管理者は、課金情報の閲覧者の役割にユーザーの nawu@fimdev.net を割り当てます。

 >**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。 

| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| 対象となる/アクティブ|
|type|String|はい| AdminAdd|
|理由|String| ロールの設定によって異なります||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|はい|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

### <a name="example-2"></a>例 2
この例では、ユーザー nawu@fimdev.net は、対象となる請求のリーダーの役割をアクティブにします。

| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| アクティブ|
|type|String|はい| UserAdd|
|理由|String| ロールの設定によって異なります||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|はい|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

### <a name="example-3"></a>例 3
この例では、ユーザー nawu@fimdev.net には、作業中の課金情報の閲覧者の役割が無効になります。

| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| アクティブ|
|type|String|はい| UserRemove|
|理由|String| いいえ||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|いいえ|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a>例 4
この例では、管理者は、課金情報の閲覧者の役割からユーザー nawu@fimdev.net を削除します。

 >**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。
 
| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| 対象となる/アクティブ|
|type|String|はい| AdminRemove|
|理由|String| いいえ||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|いいえ|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a>例 5
この例では、管理者は、所有者をユーザー nawu@fimdev.net の役割の割り当てを更新します。

 >**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。 

| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| 対象となる/アクティブ|
|type|String|はい| AdminUpdate|
|理由|String| roleSettings によって異なります||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|はい|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a>例 6
次の使用例は、API の管理サービスの共同作成者に ANUJCUSER のユーザーの有効期限切れのロールの割り当てを拡張します。

 >**注:** Additon アクセス許可を次の使用例が必要です、依頼者が少なくとも 1 つであること`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。
 
| プロパティ     | 種類    |必須|  値 |
|:---------------|:--------|:----------|:----------|
|resourceId|String|はい|\<とります\>|
|roleDefinitionId|String|はい|\<roleDefinitionId\>|
|subjectId|String|はい|\<subjectId\>|
|assignmentState|String|はい| 対象となる/アクティブ |
|type|String|はい| AdminExtend|
|理由|String| roleSettings によって異なります||
|スケジュール|[governanceSchedule](../resources/governanceschedule.md)|はい|        |
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
