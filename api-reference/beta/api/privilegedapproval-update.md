---
title: privilegedapproval の更新
description: privilegedapproval オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: cb108ca35b07138f84a9fd969bfe7c7241e9672e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538678"
---
# <a name="update-privilegedapproval"></a>privilegedapproval の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

privilegedapproval オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess、AzureAD、および directory.accessasuser.all。    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|approvalduration|期間||
|approvalstate|string| 可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。|
|approvalType|String||
|approverreason|String||
|endDateTime|DateTimeOffset||
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset||
|userId|String||

## <a name="response"></a>応答

成功した場合、このメソッド`204 No Content`は応答コードを返します。

テナントが PIM に登録されている必要があることに注意してください。 それ以外の場合、HTTP 403 の禁止状態コードが返されます。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
