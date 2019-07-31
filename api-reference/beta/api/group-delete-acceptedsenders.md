---
title: AcceptedSender の削除
description: '承認済み送信者リストからユーザーまたはグループを削除します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 341f887de0252dd6ae1ebc9f899263c67716658f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954031"
---
# <a name="remove-acceptedsender"></a>AcceptedSender の削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したグループの承認済み送信者リストからユーザーまたはグループを削除します。 

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)  |
|:---------------------------------------|:-------------------------------------------- |
| 委任 (職場または学校のアカウント)     | Group.ReadWrite.All    |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。|
| アプリケーション                            | サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー         | 値                      |
|:---------------|:---------------------------|
| Authorization  | ベアラー {トークン}。必須。  

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="examples"></a>例
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a>例 1: グループの承認済み送信者リストからユーザーを削除します。
#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a>応答
応答の例を次に示します。 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a>例 2: グループの承認済み送信者リストからグループを削除します。
#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a>応答
応答の例を次に示します。 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
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
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
