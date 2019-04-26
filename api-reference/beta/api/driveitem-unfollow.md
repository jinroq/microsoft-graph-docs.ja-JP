---
author: chackman
ms.author: chackman
title: フォロー取り消しドライブ項目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1cd3976feb643d8553920df624e30d232c5b5ed4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325371"
---
# <a name="unfollow-drive-item"></a>フォロー取り消しドライブ項目

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ドライブ](../resources/driveitem.md)のフォローを取り消します。

>**注:** アイテムをフォローするには、「[アイテムをフォロー](driveitem-follow.md)する」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a>要求本文

要求の本文は必要ありません。

## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No Content` を返します。 応答本文には何も返されません。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
この例では、で識別さ`{item-id}`れるアイテムのフォローを取り消します。

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a>応答
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": []
}
-->
