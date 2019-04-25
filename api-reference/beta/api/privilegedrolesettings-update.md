---
title: privilegedRoleSettings の更新
description: 指定した役割設定の役割設定を更新します。 privilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: 779b0d4cd61672c90c103ebb2545cb75324273fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538663"
---
# <a name="update-privilegedrolesettings"></a>privilegedRoleSettings の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した役割設定の役割設定を更新します。 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。
## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** 要求者は、特権ロール管理者、全体管理者、セキュリティ管理者、またはセキュリティ閲覧者のいずれかの役割を持っている必要があります。 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess、AzureAD、および directory.accessasuser.all。    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表記を指定します。

次の表に、役割の設定を更新するときに指定できるプロパティを示します。

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|elevationDuration|duration|役割がアクティブ化される期間。 必須。|
|id|string|ロール設定の一意の識別子。 読み取り専用。 必須です。|
|isMfaOnElevationConfigurable|ブール値|**true**の場合は、mfaonelevation を構成できます。 mfaonelevation を構成できない場合は**false** 。 必須です。|
|lastglobaladmin|ブール値|内部使用のみ。|
|maxelavationduration|duration|アクティブ化されたロールの最大期間。 必須です。|
|mfaonelevation|ブール値|役割をアクティブ化するために MFA が必要な場合は**true** 。 役割をアクティブ化するために MFA が必要でない場合は**false** 。 必須です。|
|minElevationDuration|duration|アクティブ化されたロールの最小期間。 必須です。|
|notificationToUserOnElevation|ブール値|**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。 **true**の場合は、役割がアクティブ化されたときに通知を送信しません。 必須です。|
|ticketingInfoOnElevation|ブール値|役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。 必須です。|
|approvalonelevation|ブール値|ロールをアクティブ化するときに承認が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに承認が必要ありません。 必須です。|
|承認の検証 ds|String collection|ライセンス認証に承認が必要な場合は、承認 id のリスト。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

テナントが PIM に登録されている必要があることに注意してください。 それ以外の場合、HTTP 403 の禁止状態コードが返されます。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
