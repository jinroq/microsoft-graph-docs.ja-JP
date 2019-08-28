---
title: ConversationMember の追加
description: チャネルに conversationMember を追加します。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd1f2c6689176422fa35a500224c6f2a5f277851
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634018"
---
# <a name="add-conversationmember"></a>ConversationMember の追加

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](../resources/channel.md)に[conversationMember](../resources/conversationmember.md)を追加します。

> [!NOTE]
>この操作は、チャネルの[メンバーシップ](../resources/enums.md#channelmembershiptype-values)の`private`種類がであるチャネルでのみサポートされています。 その他の[Channelメンバーシップ型](../resources/enums.md#channelmembershiptype-values)を使用して呼び出しを行うと、400不正な要求応答が返されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の小さいものから大きいものへ)|
|---------|-------------|
|委任 (職場または学校のアカウント)|Group.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません|
|アプリケーション|Group.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文

要求の本文には次のプロパティが含まれます。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|roles|string collection|そのユーザーの役割。|
|user|[ユーザー](../resources/user.md)|チャネルに追加するユーザーです。|

## <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[conversationMember](../resources/conversationmember.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "microsoft.graph.aadConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

以下は、応答の例です。

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
