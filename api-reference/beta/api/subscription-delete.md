---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509463"
---
# <a name="delete-subscription"></a>サブスクリプションを削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サブスクリプションを削除します。

## <a name="permissions"></a>アクセス許可

次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| リソースの種類/項目        | アクセス許可          |
|-----------------------------|---------------------|
| 連絡先                    | Contacts.Read       |
| スレッド               | Group.Read.All      |
| イベント                      | Calendars.Read      |
| メッセージ                    | Mail.Read           |
| グループ                      | Group.Read.All      |
| ユーザー                       | User.Read.All       |
| ドライブ (ユーザーの OneDrive)    | Files.ReadWrite     |
| ドライブ (共有、SharePoint コンテンツおよびドライブ) | Files.ReadWrite.All |
| セキュリティの警告              | SecurityEvents.ReadWrite.All |

***注:***/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。 ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
