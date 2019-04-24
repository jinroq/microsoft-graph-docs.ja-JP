---
title: governanceRoleAssignmentRequest のキャンセル
description: governanceRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: 0437051a3d2550da8a8fe3e9984214ff7c885e3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467328"
---
# <a name="cancel-governanceroleassignmentrequest"></a>governanceRoleAssignmentRequest のキャンセル

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取り消します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess AzureResources |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、 [OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。

### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。 

## <a name="error-codes"></a>エラー コード
この API は、HTTP コードの標準に従います。 それに加えて、カスタムエラーコードは以下のとおりです。
|エラー コード     | エラー メッセージ              | 詳細 |
|:--------------------| :---------------------|:--------------------|
| 400 badrequest | RoleAssignmentRequestNotFound | governanceRoleAssignmentRequest は、システムに存在しません。
| 400 badrequest | RequestCannotBeCancelled    | 、 `Granted` `PendingApproval`、、の状態の要求のみ`PendingAdminDecision`を取り消すことができます。 `PendingApprovalProvisioning`

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
