---
title: 返信の一覧表示
description: Chatmessage オブジェクトの一覧を取得します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fea842912644c30c7d6b401a4d609d8396f29a94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863529"
---
# <a name="list-replies"></a><span data-ttu-id="77b9a-103">返信の一覧表示</span><span class="sxs-lookup"><span data-stu-id="77b9a-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77b9a-104">Chatmessage オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="77b9a-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="77b9a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77b9a-105">Permissions</span></span>

<span data-ttu-id="77b9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77b9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77b9a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77b9a-108">Permission type</span></span>                        | <span data-ttu-id="77b9a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77b9a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77b9a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77b9a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="77b9a-111">チャット。読み取り、読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="77b9a-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="77b9a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77b9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77b9a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77b9a-113">Not supported.</span></span> |
| <span data-ttu-id="77b9a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77b9a-114">Application</span></span>                            | <span data-ttu-id="77b9a-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="77b9a-115">Chat.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="77b9a-116">アプリケーションのアクセス許可でこの API を呼び出す前に、アクセスを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77b9a-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="77b9a-117">詳細については、「 [Microsoft Teams の保護された api](/graph/teams-protected-apis)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77b9a-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="77b9a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77b9a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77b9a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="77b9a-119">Optional query parameters</span></span>

<span data-ttu-id="77b9a-120">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="77b9a-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77b9a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77b9a-121">Request headers</span></span>

| <span data-ttu-id="77b9a-122">名前</span><span class="sxs-lookup"><span data-stu-id="77b9a-122">Name</span></span>      |<span data-ttu-id="77b9a-123">説明</span><span class="sxs-lookup"><span data-stu-id="77b9a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77b9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77b9a-124">Authorization</span></span> | <span data-ttu-id="77b9a-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="77b9a-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77b9a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77b9a-126">Request body</span></span>

<span data-ttu-id="77b9a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77b9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77b9a-128">応答</span><span class="sxs-lookup"><span data-stu-id="77b9a-128">Response</span></span>

<span data-ttu-id="77b9a-129">このメソッドは、成功すると `200 OK` 応答コードと [chatMessage](../resources/chatmessage.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="77b9a-129">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77b9a-130">例</span><span class="sxs-lookup"><span data-stu-id="77b9a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77b9a-131">要求</span><span class="sxs-lookup"><span data-stu-id="77b9a-131">Request</span></span>

<span data-ttu-id="77b9a-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77b9a-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77b9a-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="77b9a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77b9a-134">C#</span><span class="sxs-lookup"><span data-stu-id="77b9a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77b9a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="77b9a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77b9a-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="77b9a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77b9a-137">Java</span><span class="sxs-lookup"><span data-stu-id="77b9a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77b9a-138">応答</span><span class="sxs-lookup"><span data-stu-id="77b9a-138">Response</span></span>

<span data-ttu-id="77b9a-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77b9a-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="77b9a-140">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="77b9a-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77b9a-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="77b9a-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
