---
title: チャネルでの chatMessage reply の作成
description: 既存の chatMessage オブジェクトへの返信に新しい chatMessage オブジェクトを作成します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6b09efa8b0d35b2377b9980c456b794954445a3e
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720935"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="801fe-103">チャネルでの chatMessage reply の作成</span><span class="sxs-lookup"><span data-stu-id="801fe-103">Create chatMessage reply in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="801fe-104">既存の[chatmessage](../resources/chatmessage.md)オブジェクトへの返信に新しい[chatmessage](../resources/chatmessage.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="801fe-104">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="801fe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="801fe-105">Permissions</span></span>

<span data-ttu-id="801fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="801fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="801fe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="801fe-108">Permission type</span></span>                        | <span data-ttu-id="801fe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="801fe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="801fe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="801fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="801fe-111">チャットの読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="801fe-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="801fe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="801fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="801fe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801fe-113">Not supported.</span></span> |
| <span data-ttu-id="801fe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="801fe-114">Application</span></span>                            | <span data-ttu-id="801fe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="801fe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="801fe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
POST /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="801fe-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="801fe-117">Request headers</span></span>

| <span data-ttu-id="801fe-118">名前</span><span class="sxs-lookup"><span data-stu-id="801fe-118">Name</span></span>          | <span data-ttu-id="801fe-119">説明</span><span class="sxs-lookup"><span data-stu-id="801fe-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="801fe-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="801fe-120">Authorization</span></span> | <span data-ttu-id="801fe-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="801fe-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="801fe-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="801fe-122">Request body</span></span>

<span data-ttu-id="801fe-123">要求本文で、 [Chatmessage](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="801fe-123">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="801fe-124">応答</span><span class="sxs-lookup"><span data-stu-id="801fe-124">Response</span></span>

<span data-ttu-id="801fe-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[chatmessage](../resources/chatmessage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="801fe-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="801fe-126">例</span><span class="sxs-lookup"><span data-stu-id="801fe-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="801fe-127">要求</span><span class="sxs-lookup"><span data-stu-id="801fe-127">Request</span></span>

<span data-ttu-id="801fe-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="801fe-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chatmessage"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```

### <a name="response"></a><span data-ttu-id="801fe-129">応答</span><span class="sxs-lookup"><span data-stu-id="801fe-129">Response</span></span>

<span data-ttu-id="801fe-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="801fe-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="801fe-131">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="801fe-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="801fe-132">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="801fe-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->