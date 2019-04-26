---
title: 同期スキーマの削除
description: カスタマイズされたスキーマを削除し、スキーマを既定の構成にリセットします。 スキーマがテンプレートのコンテキストで削除されると、そのテンプレートに関連付けられている既定のスキーマにリセット`factoryTag`されます。
localization_priority: Normal
ms.openlocfilehash: 0871de0ba5b48784e47fd5cc8d3ac890ab23748b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330622"
---
# <a name="delete-synchronizationschema"></a>同期スキーマの削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

カスタマイズされたスキーマを削除し、スキーマを既定の構成にリセットします。 スキーマがテンプレートのコンテキストで削除されると、そのテンプレートに関連付けられている既定のスキーマにリセット`factoryTag`されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。|
|アプリケーション                            |サポートされていません。| 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 型    | 説明|
|:---------------|:--------|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 No Content` 応答コードを返します。 応答本文では何も返しません。

## <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
