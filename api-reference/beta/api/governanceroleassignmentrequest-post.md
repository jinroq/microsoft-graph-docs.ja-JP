---
title: GovernanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
ms.openlocfilehash: 674a69f5697f5abf6e654ea71419bdfdfd660343
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859113"
---
# <a name="create-governanceroleassignmentrequest"></a>GovernanceRoleAssignmentRequest を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。

| Operation                                   | 型        |
|:--------------------------------------------|:------------|
| 役割の割り当てを割り当てる                    | AdminAdd    |
| 適格な役割の割り当てをアクティブ化する        | UserAdd     |
| アクティブ化された役割の割り当てを無効にする     | UserRemove  |
| 役割の割り当てを削除する                    | AdminRemove |
| 役割の割り当てを更新する                    | AdminUpdate |
| 自分の役割の割り当てを拡張するための要求        | UserExtend  |
| 役割の割り当てを拡張する                    | AdminExtend |
| 期限切れの役割の割り当てを更新する要求 | UserRenew   |
| 期限切れの役割の割り当てを更新する            | AdminRenew  |

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可                               |
|:---------------------------------------|:------------------------------------------|
| 委任 (職場または学校のアカウント)     | PrivilegedAccess AzureResources |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                            |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明      |
|:--------------|:-----------------|
| Authorization | Bearer {code}    |
| Content-type  | application/json |

## <a name="request-body"></a>要求本文

要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。

| プロパティ         | 型                                                     | 説明 |
|:-----------------|:---------------------------------------------------------|:--|
| resourceId       | String                                                   | リソースの ID。 必須です。 |
| roleDefinitionId | String                                                   | ロール定義の ID。 必須です。 |
| subjectId        | String                                                   | 件名の ID。 必須です。 |
| 割り当ての状態  | String                                                   | 割り当ての状態を指定します。 値には、 `Eligible`および`Active`を指定できます。 必須。 |
| type             | String                                                   | 要求の種類。 値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。 必須です。 |
| したがっ           | String                                                   | 監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。 |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | 役割の割り当て要求のスケジュール。 、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate` |

## <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。

### <a name="error-codes"></a>エラー コード

この API は、標準の HTTP エラーコードを返します。 また、次の表に示されているエラーコードも返します。

| エラー コード     | エラー メッセージ                               | 詳細       |
|:---------------|:--------------------------------------------|:--------------|
| 400 BadRequest | RoleNotFound                                | 要求`roleDefinitionId`本文で指定されたが見つかりません。 |
| 400 BadRequest | ResourceIsLocked                            | 要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。 |
| 400 BadRequest | SubjectNotFound                             | 要求`subjectId`本文で指定されたが見つかりません。 |
| 400 BadRequest | Pendingrole割り当て要求                | 保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。 |
| 400 BadRequest | Role割り当てが存在する                        | 作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。 |
| 400 BadRequest | RoleAssignmentDoesNotExist                  | 更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。 |
| 400 BadRequest | Role割り当て要求 Policyvalidationfailed | [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。 |

## <a name="examples"></a>例

次の例は、この API の使用方法を示しています。

### <a name="example-1-administrator-assigns-user-to-a-role"></a>例 1: 管理者がユーザーを役割に割り当てる

この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。

 >**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。

| プロパティ         | 型                                                     | 必須                 | 値 |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | はい                      | \<resourceId\> |
| roleDefinitionId | String                                                   | はい                      | \<roleDefinitionId\> |
| subjectId        | String                                                   | はい                      | \<subjectId\> |
| 割り当ての状態  | String                                                   | はい                      | 対象/アクティブ |
| type             | String                                                   | はい                      | AdminAdd |
| したがっ           | String                                                   | 役割の設定によって異なる |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | はい                      |   |

#### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a>例 2: ユーザーが対象となる役割をアクティブにする

この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。

| プロパティ         | 型                                                     | 必須                 | 値 |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | はい                      | \<resourceId\> |
| roleDefinitionId | String                                                   | はい                      | \<roleDefinitionId\> |
| subjectId        | String                                                   | はい                      | \<subjectId\> |
| 割り当ての状態  | String                                                   | はい                      | Active |
| type             | String                                                   | はい                      | UserAdd |
| したがっ           | String                                                   | 役割の設定によって異なる |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | はい                      |   |

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a>例 3: ユーザーが割り当てられた役割を非アクティブにする

この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。

| プロパティ         | 型                                                     | 必須 | 値 |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | はい      | \<resourceId\> |
| roleDefinitionId | String                                                   | はい      | \<roleDefinitionId\> |
| subjectId        | String                                                   | はい      | \<subjectId\> |
| 割り当ての状態  | 文字列                                                   | はい      | Active |
| type             | 文字列                                                   | はい      | UserRemove |
| したがっ           | String                                                   | いいえ       |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | いいえ       |   |

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-4-administrator-removes-user-from-a-role"></a>例 4: 管理者が役割からユーザーを削除する

この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。

 >**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。

| プロパティ         | 型                                                     | 必須 | 値 |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | はい      | \<resourceId\> |
| roleDefinitionId | 文字列                                                   | はい      | \<roleDefinitionId\> |
| subjectId        | 文字列                                                   | はい      | \<subjectId\> |
| 割り当ての状態  | 文字列                                                   | はい      | 対象/アクティブ |
| type             | 文字列                                                   | はい      | AdminRemove |
| したがっ           | String                                                   | いいえ       |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | いいえ       |   |

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a>例 5: 管理者の更新の役割の割り当て

この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。

 >**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。

| プロパティ         | 型                                                     | 必須                | 値 |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | はい                     | \<resourceId\> |
| roleDefinitionId | 文字列                                                   | はい                     | \<roleDefinitionId\> |
| subjectId        | 文字列                                                   | はい                     | \<subjectId\> |
| 割り当ての状態  | 文字列                                                   | はい                     | 対象/アクティブ |
| type             | 文字列                                                   | はい                     | AdminUpdate |
| したがっ           | String                                                   | roleSettings に依存 |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | はい                     |   |

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a>例 6: 管理者が期限切れの役割の割り当てを拡張する

この例では、user ANUCUSER の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。

 >**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。

| プロパティ         | 型                                                     | 必須                | 値 |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | はい                     | \<resourceId\> |
| roleDefinitionId | 文字列                                                   | はい                     | \<roleDefinitionId\> |
| subjectId        | String                                                   | はい                     | \<subjectId\> |
| 割り当ての状態  | String                                                   | はい                     | 対象/アクティブ |
| type             | String                                                   | はい                     | AdminExtend |
| したがっ           | String                                                   | roleSettings に依存 |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | はい                     |   |

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
