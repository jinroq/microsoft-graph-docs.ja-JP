---
title: ConversationMember の削除
description: チャネルから conversationMember を削除します。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 739705d2c57210d15813ad8cbed4627afef29d07
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634017"
---
# <a name="delete-conversationmember"></a>ConversationMember の削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](../resources/channel.md)から[conversationMember](../resources/conversationmember.md)を削除します。

> [!NOTE]
> この操作は、チャネルの[メンバーシップ](../resources/enums.md#channelmembershiptype-values)の`private`種類がであるチャネルでのみサポートされています。 その他の[Channelメンバーシップ型](../resources/enums.md#channelmembershiptype-values)を使用して`400 Bad Request`呼び出しを行うと、応答が返されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の小さいものから大きいものへ)|
|---------|-------------|
|委任 (職場または学校のアカウント)|**User**または**chat**リソースの場合:<br/>チャット。読み取り、読み取り/書き込み<br/><br/>**チャネル**リソースの場合:<br/>Group.Read.All、Group.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません|
|アプリケーション| **User**または**chat**リソースの場合:<br/>Chat. All、すべてのチャット。<br/><br/>**チャネル**リソースの場合:<br/>Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

以下は、応答の例です。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
