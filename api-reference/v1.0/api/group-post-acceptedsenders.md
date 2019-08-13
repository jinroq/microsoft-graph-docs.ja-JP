---
title: AcceptedSender の作成
description: AcceptedSender リストに新しいユーザーやグループを追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: eafe458bc9e290a982395efe21cc2d87a29a4411
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337175"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="5a286-103">AcceptedSender の作成</span><span class="sxs-lookup"><span data-stu-id="5a286-103">Create acceptedSender</span></span>
<span data-ttu-id="5a286-104">AcceptedSender リストに新しいユーザーやグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="5a286-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="5a286-p101">`@odata.id` 内のユーザーやグループを要求の本文で指定します。承諾済み送信者リスト内のユーザーは、グループに会話を投稿できません。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="5a286-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a286-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a286-108">Permissions</span></span>
<span data-ttu-id="5a286-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a286-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a286-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a286-111">Permission type</span></span>      | <span data-ttu-id="5a286-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a286-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a286-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a286-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5a286-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a286-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a286-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a286-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a286-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a286-116">Not supported.</span></span>    |
|<span data-ttu-id="5a286-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a286-117">Application</span></span> | <span data-ttu-id="5a286-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a286-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a286-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a286-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5a286-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a286-120">Request headers</span></span>
| <span data-ttu-id="5a286-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a286-121">Header</span></span>       | <span data-ttu-id="5a286-122">値</span><span class="sxs-lookup"><span data-stu-id="5a286-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a286-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a286-123">Authorization</span></span>  | <span data-ttu-id="5a286-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a286-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a286-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a286-126">Request body</span></span>
<span data-ttu-id="5a286-127">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a286-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="5a286-128">応答</span><span class="sxs-lookup"><span data-stu-id="5a286-128">Response</span></span>
<span data-ttu-id="5a286-129">このメソッドは `204 No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="5a286-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a286-130">例</span><span class="sxs-lookup"><span data-stu-id="5a286-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5a286-131">要求</span><span class="sxs-lookup"><span data-stu-id="5a286-131">Request</span></span>
<span data-ttu-id="5a286-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a286-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5a286-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5a286-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a286-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a286-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a286-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="5a286-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="5a286-136">C#</span><span class="sxs-lookup"><span data-stu-id="5a286-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5a286-137">Java</span><span class="sxs-lookup"><span data-stu-id="5a286-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acceptedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a286-138">応答</span><span class="sxs-lookup"><span data-stu-id="5a286-138">Response</span></span>
<span data-ttu-id="5a286-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a286-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
