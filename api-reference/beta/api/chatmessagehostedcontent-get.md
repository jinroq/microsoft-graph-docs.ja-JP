---
title: ChatMessageHostedContent を取得する
description: ChatMessageHostedContent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce939461df3d0ded354b1a32d6ea87ad904625e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319889"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="c7e09-103">ChatMessageHostedContent を取得する</span><span class="sxs-lookup"><span data-stu-id="c7e09-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e09-104">[ChatMessageHostedContent](../resources/chatmessagehostedcontent.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7e09-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7e09-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7e09-105">Permissions</span></span>

<span data-ttu-id="c7e09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7e09-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7e09-108">Permission type</span></span>                        | <span data-ttu-id="c7e09-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7e09-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7e09-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7e09-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7e09-111">チャット。読み取り、読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="c7e09-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="c7e09-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7e09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7e09-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7e09-113">Not supported.</span></span> |
| <span data-ttu-id="c7e09-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7e09-114">Application</span></span>                            | <span data-ttu-id="c7e09-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7e09-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7e09-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7e09-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7e09-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c7e09-117">Optional query parameters</span></span>

<span data-ttu-id="c7e09-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="c7e09-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7e09-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7e09-119">Request headers</span></span>

| <span data-ttu-id="c7e09-120">名前</span><span class="sxs-lookup"><span data-stu-id="c7e09-120">Name</span></span>      |<span data-ttu-id="c7e09-121">説明</span><span class="sxs-lookup"><span data-stu-id="c7e09-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7e09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e09-122">Authorization</span></span> | <span data-ttu-id="c7e09-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c7e09-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7e09-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7e09-124">Request body</span></span>

<span data-ttu-id="c7e09-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c7e09-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e09-126">応答</span><span class="sxs-lookup"><span data-stu-id="c7e09-126">Response</span></span>

<span data-ttu-id="c7e09-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7e09-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7e09-128">例</span><span class="sxs-lookup"><span data-stu-id="c7e09-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7e09-129">要求</span><span class="sxs-lookup"><span data-stu-id="c7e09-129">Request</span></span>

<span data-ttu-id="c7e09-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7e09-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c7e09-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c7e09-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7e09-132">C#</span><span class="sxs-lookup"><span data-stu-id="c7e09-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7e09-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7e09-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7e09-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="c7e09-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c7e09-135">Java</span><span class="sxs-lookup"><span data-stu-id="c7e09-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7e09-136">応答</span><span class="sxs-lookup"><span data-stu-id="c7e09-136">Response</span></span>

<span data-ttu-id="c7e09-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7e09-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c7e09-138">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c7e09-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7e09-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c7e09-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
