---
title: ChatMessageHostedContent を取得する
description: ChatMessageHostedContent オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1cf0aa6bcca49921d90117be71f4cdc5af28372a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261363"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="9d8db-103">ChatMessageHostedContent を取得する</span><span class="sxs-lookup"><span data-stu-id="9d8db-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d8db-104">[ChatMessageHostedContent](../resources/chatmessagehostedcontent.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9d8db-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d8db-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d8db-105">Permissions</span></span>

<span data-ttu-id="9d8db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d8db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d8db-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d8db-108">Permission type</span></span>                        | <span data-ttu-id="9d8db-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d8db-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d8db-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d8db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d8db-111">チャット。読み取り、読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="9d8db-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="9d8db-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d8db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d8db-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d8db-113">Not supported.</span></span> |
| <span data-ttu-id="9d8db-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d8db-114">Application</span></span>                            | <span data-ttu-id="9d8db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d8db-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d8db-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d8db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d8db-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d8db-117">Optional query parameters</span></span>

<span data-ttu-id="9d8db-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="9d8db-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d8db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d8db-119">Request headers</span></span>

| <span data-ttu-id="9d8db-120">名前</span><span class="sxs-lookup"><span data-stu-id="9d8db-120">Name</span></span>      |<span data-ttu-id="9d8db-121">説明</span><span class="sxs-lookup"><span data-stu-id="9d8db-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d8db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d8db-122">Authorization</span></span> | <span data-ttu-id="9d8db-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9d8db-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d8db-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d8db-124">Request body</span></span>

<span data-ttu-id="9d8db-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d8db-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d8db-126">応答</span><span class="sxs-lookup"><span data-stu-id="9d8db-126">Response</span></span>

<span data-ttu-id="9d8db-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d8db-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d8db-128">例</span><span class="sxs-lookup"><span data-stu-id="9d8db-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d8db-129">要求</span><span class="sxs-lookup"><span data-stu-id="9d8db-129">Request</span></span>

<span data-ttu-id="9d8db-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d8db-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```

### <a name="response"></a><span data-ttu-id="9d8db-131">応答</span><span class="sxs-lookup"><span data-stu-id="9d8db-131">Response</span></span>

<span data-ttu-id="9d8db-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d8db-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9d8db-133">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d8db-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d8db-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d8db-134">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9d8db-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9d8db-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="9d8db-136">C#</span><span class="sxs-lookup"><span data-stu-id="9d8db-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d8db-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d8db-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9d8db-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="9d8db-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
