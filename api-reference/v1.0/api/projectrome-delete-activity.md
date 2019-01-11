---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
localization_priority: Normal
ms.openlocfilehash: fab008e9a9d031aed12605f14bf447247c0227ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838151"
---
# <a name="delete-an-activity"></a>アクティビティを削除する

アプリの既存のユーザーのアクティビティを削除します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | UserActivity.ReadWrite.CreatedByApp    |
|委任 (個人用 Microsoft アカウント) | UserActivity.ReadWrite.CreatedByApp    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a>要求ヘッダー

|名前 | 種類 | 説明|
|:----|:-----|:-----------|
|Authorization | string | ベアラー {トークン}。必須。|

## <a name="request-body"></a>要求本文

要求の本体がありません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a>応答

以下は、応答の例です。

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
