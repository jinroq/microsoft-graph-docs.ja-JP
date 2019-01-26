---
title: PrivilegedRoleSettings を更新します。
description: 役割の設定を特定の役割の設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: 7b49d228372e2fa122f9461706f782c60cfea379
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577271"
---
# <a name="update-privilegedrolesettings"></a>PrivilegedRoleSettings を更新します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

役割の設定を特定の役割の設定を更新します。 [PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。
## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** 依頼者は、次のロールのいずれかの必要があります: ロールの権限を持つ管理者、グローバル管理者、セキュリティ管理者、またはセキュリティのリーダーです。 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All    |
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
要求の本文には、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表現を指定します。

役割の設定を更新するときは指定するプロパティを次の表に一覧します。

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|elevationDuration |文字列 (タイムスタンプ) |ロールが有効な場合の期間です。 必須です。|
|id| 文字列 (識別子) |ロールの設定の一意の識別子です。 読み取り専用です。 必須です。|
|isMfaOnElevationConfigurable|boolean|**真**mfaOnElevation は、構成可能な場合です。 場合は**false を指定**mfaOnElevation は構成できません。 必須です。|
|lastGlobalAdmin| Boolean |内部使用のみ。|
|maxElavationDuration| 文字列 (タイムスタンプ)|アクティブ化されたロールの最大の期間です。 必須です。|
|mfaOnElevation| Boolean |**true** MFA は、ロールをアクティブにするために必要な場合です。 **false**場合は、MFA は、ロールをアクティブにする必要はありません。 必須です。|
|minElevationDuration| 文字列 (タイムスタンプ) |アクティブ化されたロールの最小の期間です。 必須です。|
|notificationToUserOnElevation|Boolean|**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。 **false**場合は、ロールがアクティブになったときに通知を送信できません。 必須です。|
|ticketingInfoOnElevation|Boolean|**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。 **false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。 必須です。|
|approvalOnElevation|Boolean|**true の**場合は、承認が必要な場合は、ロールをアクティブにします。 **false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。 必須です。|
|approverIds| 文字列 (識別子) のコレクション|承認 Id、ライセンス認証の必要な場合は承認の一覧です。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

テナントの PIM を登録する必要があることに注意してください。 それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。
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
