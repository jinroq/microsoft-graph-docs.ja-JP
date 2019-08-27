---
title: PrivilegedRoleSettings の更新
description: 指定した役割設定の役割設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 01737dd7ffbb15e3fd96cad6b9c9c3aa55cc981d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633658"
---
# <a name="update-privilegedrolesettings"></a>PrivilegedRoleSettings の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した役割設定の役割設定を更新します。 [PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。
## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** 要求者は、役割の設定を更新するための特権の役割管理者の役割を持っている必要があります。 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess、AzureAD、および Directory.accessasuser.all。    |
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
|id|string|ロール設定の一意の識別子。 読み取り専用です。 必須です。|
|isMfaOnElevationConfigurable|ブール値|**true**の場合は、mfaOnElevation を構成できます。 mfaOnElevation を構成できない場合は**false** 。 必須です。|
|lastGlobalAdmin|Boolean|内部使用のみ。|
|maxElavationDuration|duration|アクティブ化されたロールの最大期間。 必須です。|
|mfaOnElevation|Boolean|役割をアクティブ化するために MFA が必要な場合は**true** 。 役割をアクティブ化するために MFA が必要でない場合は**false** 。 必須です。|
|minElevationDuration|duration|アクティブ化されたロールの最小期間。 必須です。|
|notificationToUserOnElevation|Boolean|**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。 **true**の場合は、役割がアクティブ化されたときに通知を送信しません。 必須です。|
|ticketingInfoOnElevation|Boolean|役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。 必須です。|
|approvalOnElevation|Boolean|ロールをアクティブ化するときに承認が必要な場合は**true** 。 **false**を指定すると、役割をアクティブ化するときに承認が必要ありません。 必須です。|
|承認の検証 Ds|string collection|ライセンス認証に承認が必要な場合は、承認 Id のリスト。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

テナントが PIM に登録されている必要があることに注意してください。 それ以外の場合、HTTP 403 の禁止状態コードが返されます。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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
  ]
}
-->
