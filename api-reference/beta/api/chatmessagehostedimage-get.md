---
title: ChatMessageHostedImage を取得する
description: ChatMessage 内のホストされた画像を取得します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a8bf0fe79df064c7d53b987e1b9aa5ccddbc1cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943597"
---
# <a name="get-chatmessagehostedimage"></a><span data-ttu-id="b8bee-103">ChatMessageHostedImage を取得する</span><span class="sxs-lookup"><span data-stu-id="b8bee-103">Get chatMessageHostedImage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8bee-104">[Chatmessage](../resources/chatmessage.md)内のホストされている[イメージ](../resources/chatmessagehostedimage.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8bee-104">Retrieve a [hosted image](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8bee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8bee-105">Permissions</span></span>

<span data-ttu-id="b8bee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8bee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8bee-108">Permission Type</span></span>|<span data-ttu-id="b8bee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8bee-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b8bee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8bee-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b8bee-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bee-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="b8bee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8bee-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8bee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8bee-113">Not supported.</span></span>|
|<span data-ttu-id="b8bee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8bee-114">Application</span></span>| <span data-ttu-id="b8bee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8bee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8bee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8bee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}
GET /chats/{id}/messages/{id}/hostedImages/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8bee-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b8bee-117">Optional query parameters</span></span>

<span data-ttu-id="b8bee-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="b8bee-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8bee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8bee-119">Request headers</span></span>

| <span data-ttu-id="b8bee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8bee-120">Header</span></span>       | <span data-ttu-id="b8bee-121">値</span><span class="sxs-lookup"><span data-stu-id="b8bee-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8bee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8bee-122">Authorization</span></span>  | <span data-ttu-id="b8bee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8bee-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8bee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8bee-125">Request body</span></span>

<span data-ttu-id="b8bee-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b8bee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8bee-127">応答</span><span class="sxs-lookup"><span data-stu-id="b8bee-127">Response</span></span>

<span data-ttu-id="b8bee-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文でホストされた[image](../resources/chatmessagehostedimage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8bee-128">If successful, this method returns a `200 OK` response code and a [hosted image](../resources/chatmessagehostedimage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8bee-129">例</span><span class="sxs-lookup"><span data-stu-id="b8bee-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8bee-130">要求</span><span class="sxs-lookup"><span data-stu-id="b8bee-130">Request</span></span>

<span data-ttu-id="b8bee-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8bee-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8bee-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b8bee-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8bee-133">C#</span><span class="sxs-lookup"><span data-stu-id="b8bee-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8bee-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8bee-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8bee-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="b8bee-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8bee-136">Java</span><span class="sxs-lookup"><span data-stu-id="b8bee-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b8bee-137">応答</span><span class="sxs-lookup"><span data-stu-id="b8bee-137">Response</span></span>

<span data-ttu-id="b8bee-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b8bee-138">Here is an example of the response.</span></span> 

><span data-ttu-id="b8bee-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b8bee-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
