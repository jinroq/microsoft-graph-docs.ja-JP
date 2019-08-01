---
title: イベントの削除
description: event オブジェクトを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 76fec8edbf1447240fdd37ff199b15360d1da3e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016407"
---
# <a name="delete-event"></a><span data-ttu-id="9583e-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="9583e-103">Delete event</span></span>
<span data-ttu-id="9583e-104">[event](../resources/event.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9583e-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9583e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9583e-105">Permissions</span></span>
<span data-ttu-id="9583e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9583e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9583e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9583e-108">Permission type</span></span>      | <span data-ttu-id="9583e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9583e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9583e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9583e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9583e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9583e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9583e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9583e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9583e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9583e-113">Not supported.</span></span>    |
|<span data-ttu-id="9583e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9583e-114">Application</span></span> | <span data-ttu-id="9583e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9583e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9583e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9583e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9583e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9583e-117">Request headers</span></span>
| <span data-ttu-id="9583e-118">名前</span><span class="sxs-lookup"><span data-stu-id="9583e-118">Name</span></span>       | <span data-ttu-id="9583e-119">型</span><span class="sxs-lookup"><span data-stu-id="9583e-119">Type</span></span> | <span data-ttu-id="9583e-120">説明</span><span class="sxs-lookup"><span data-stu-id="9583e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9583e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9583e-121">Authorization</span></span>  | <span data-ttu-id="9583e-122">string</span><span class="sxs-lookup"><span data-stu-id="9583e-122">string</span></span>  | <span data-ttu-id="9583e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9583e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9583e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9583e-125">Request body</span></span>
<span data-ttu-id="9583e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9583e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9583e-127">応答</span><span class="sxs-lookup"><span data-stu-id="9583e-127">Response</span></span>
<span data-ttu-id="9583e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9583e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9583e-130">例</span><span class="sxs-lookup"><span data-stu-id="9583e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9583e-131">要求</span><span class="sxs-lookup"><span data-stu-id="9583e-131">Request</span></span>
<span data-ttu-id="9583e-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9583e-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9583e-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9583e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9583e-134">C#</span><span class="sxs-lookup"><span data-stu-id="9583e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9583e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9583e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9583e-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="9583e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9583e-137">Java</span><span class="sxs-lookup"><span data-stu-id="9583e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9583e-138">応答</span><span class="sxs-lookup"><span data-stu-id="9583e-138">Response</span></span>
<span data-ttu-id="9583e-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9583e-139">The following is an example of the response.</span></span> 
><span data-ttu-id="9583e-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9583e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
