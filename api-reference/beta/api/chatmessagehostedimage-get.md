---
title: ChatMessageHostedImage を取得する
description: ChatMessage 内のホストされた画像を取得します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f25f2e407426d5754b5d648cf27d1b9c78a82544
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418076"
---
# <a name="get-chatmessagehostedimage"></a><span data-ttu-id="9e8f7-103">ChatMessageHostedImage を取得する</span><span class="sxs-lookup"><span data-stu-id="9e8f7-103">Get chatMessageHostedImage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e8f7-104">[Chatmessage](../resources/chatmessage.md)内のホストされている[イメージ](../resources/chatmessagehostedimage.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-104">Retrieve a [hosted image](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e8f7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9e8f7-105">Permissions</span></span>

<span data-ttu-id="9e8f7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e8f7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e8f7-108">Permission Type</span></span>|<span data-ttu-id="9e8f7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e8f7-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9e8f7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e8f7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9e8f7-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e8f7-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="9e8f7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e8f7-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e8f7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-113">Not supported.</span></span>|
|<span data-ttu-id="9e8f7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e8f7-114">Application</span></span>| <span data-ttu-id="9e8f7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e8f7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e8f7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}
GET /chats/{id}/messages/{id}/hostedImages/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e8f7-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e8f7-117">Optional query parameters</span></span>

<span data-ttu-id="9e8f7-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e8f7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e8f7-119">Request headers</span></span>

| <span data-ttu-id="9e8f7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e8f7-120">Header</span></span>       | <span data-ttu-id="9e8f7-121">値</span><span class="sxs-lookup"><span data-stu-id="9e8f7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e8f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e8f7-122">Authorization</span></span>  | <span data-ttu-id="9e8f7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e8f7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e8f7-125">Request body</span></span>

<span data-ttu-id="9e8f7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e8f7-127">応答</span><span class="sxs-lookup"><span data-stu-id="9e8f7-127">Response</span></span>

<span data-ttu-id="9e8f7-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文でホストされた[image](../resources/chatmessagehostedimage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-128">If successful, this method returns a `200 OK` response code and a [hosted image](../resources/chatmessagehostedimage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e8f7-129">例</span><span class="sxs-lookup"><span data-stu-id="9e8f7-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9e8f7-130">要求</span><span class="sxs-lookup"><span data-stu-id="9e8f7-130">Request</span></span>

<span data-ttu-id="9e8f7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9e8f7-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9e8f7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e8f7-133">C#</span><span class="sxs-lookup"><span data-stu-id="9e8f7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e8f7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e8f7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e8f7-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="9e8f7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e8f7-136">応答</span><span class="sxs-lookup"><span data-stu-id="9e8f7-136">Response</span></span>

<span data-ttu-id="9e8f7-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-137">Here is an example of the response.</span></span> 

><span data-ttu-id="9e8f7-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9e8f7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "url": "url-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat message image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
