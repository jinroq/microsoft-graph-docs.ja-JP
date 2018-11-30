---
title: GovernanceRoleAssignmentRequest をキャンセルします。
description: GovernanceRoleAssignmentRequest をキャンセルします。
ms.openlocfilehash: 3e83d47b94f69b124b841f99490a012f2e39a42c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069232"
---
# <a name="cancel-governanceroleassignmentrequest"></a>GovernanceRoleAssignmentRequest をキャンセルします。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)をキャンセルします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは [OData クエリ パラメーター](/graph/query-parameters)をサポートして**いません**。

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
この API は、HTTP のコードの標準に準拠します。 ほかに、カスタムのエラー コードを以下に示します。
|エラー コード     | エラー メッセージ              | 詳細 |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleAssignmentRequestNotFound | GovernanceRoleAssignmentRequest は、システムに存在しません。
| 400 BadRequest | RequestCannotBeCancelled    | 状態でのみ要求`Granted`、 `PendingApproval`、`PendingApprovalProvisioning`と`PendingAdminDecision`キャンセルすることができます。

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
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->