---
title: HistoryItem を削除します。
description: 既存のユーザー アクティビティの既存の履歴項目を削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 30e7ee53e6546d6c70e3d576e0e2eb57965cf46f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979860"
---
# <a name="delete-a-historyitem"></a>HistoryItem を削除します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

既存のユーザー アクティビティの既存の履歴項目を削除します。

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
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a>要求ヘッダー

|名前 | 種類 | 説明|
|:----|:-----|:-----------|
|Authorization | string | ベアラー {トークン}。必須。|

## <a name="request-body"></a>要求本文

要求の本体がありません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、 `204 No Content` 、履歴項目が削除された場合の応答コード。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
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
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
