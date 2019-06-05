---
title: ChatMessage の取得
description: ChatMessage オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ef40a53be083744f99cac01cf2e72466e616b20
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720941"
---
# <a name="get-chatmessage"></a><span data-ttu-id="afd87-103">ChatMessage の取得</span><span class="sxs-lookup"><span data-stu-id="afd87-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afd87-104">[Chatmessage](../resources/chatmessage.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="afd87-104">Retrieve the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd87-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afd87-105">Permissions</span></span>

<span data-ttu-id="afd87-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afd87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afd87-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afd87-108">Permission type</span></span>                        | <span data-ttu-id="afd87-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="afd87-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afd87-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afd87-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="afd87-111">チャット。読み取り、読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="afd87-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="afd87-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afd87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd87-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afd87-113">Not supported.</span></span> |
| <span data-ttu-id="afd87-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afd87-114">Application</span></span>                            | <span data-ttu-id="afd87-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="afd87-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd87-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afd87-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afd87-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="afd87-117">Optional query parameters</span></span>

<span data-ttu-id="afd87-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="afd87-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd87-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afd87-119">Request headers</span></span>

| <span data-ttu-id="afd87-120">名前</span><span class="sxs-lookup"><span data-stu-id="afd87-120">Name</span></span>      |<span data-ttu-id="afd87-121">説明</span><span class="sxs-lookup"><span data-stu-id="afd87-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afd87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afd87-122">Authorization</span></span> | <span data-ttu-id="afd87-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="afd87-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd87-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="afd87-124">Request body</span></span>

<span data-ttu-id="afd87-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="afd87-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd87-126">応答</span><span class="sxs-lookup"><span data-stu-id="afd87-126">Response</span></span>

<span data-ttu-id="afd87-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[chatmessage](../resources/chatmessage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="afd87-127">If successful, this method returns a `200 OK` response code and the requested [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afd87-128">例</span><span class="sxs-lookup"><span data-stu-id="afd87-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afd87-129">要求</span><span class="sxs-lookup"><span data-stu-id="afd87-129">Request</span></span>

<span data-ttu-id="afd87-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="afd87-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessage"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}
```

### <a name="response"></a><span data-ttu-id="afd87-131">応答</span><span class="sxs-lookup"><span data-stu-id="afd87-131">Response</span></span>

<span data-ttu-id="afd87-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="afd87-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="afd87-133">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="afd87-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="afd87-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="afd87-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "device": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "etag": "etag-value",
  "messageType": "messageType-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->