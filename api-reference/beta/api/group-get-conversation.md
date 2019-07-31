---
title: Get conversation
description: conversation オブジェクトを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dadccbf721b9a596f256ca9bd648b62f32d996dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953893"
---
# <a name="get-conversation"></a><span data-ttu-id="949fc-103">Get conversation</span><span class="sxs-lookup"><span data-stu-id="949fc-103">Get conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949fc-104">[conversation](../resources/conversation.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="949fc-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="949fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="949fc-105">Permissions</span></span>
<span data-ttu-id="949fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="949fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="949fc-108">Permission type</span></span>      | <span data-ttu-id="949fc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="949fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="949fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="949fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="949fc-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949fc-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="949fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="949fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949fc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="949fc-113">Not supported.</span></span>    |
|<span data-ttu-id="949fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="949fc-114">Application</span></span> | <span data-ttu-id="949fc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="949fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="949fc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="949fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="949fc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="949fc-117">Optional query parameters</span></span>
<span data-ttu-id="949fc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="949fc-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="949fc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="949fc-119">Request headers</span></span>
| <span data-ttu-id="949fc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="949fc-120">Header</span></span>       | <span data-ttu-id="949fc-121">値</span><span class="sxs-lookup"><span data-stu-id="949fc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="949fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="949fc-122">Authorization</span></span>  | <span data-ttu-id="949fc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="949fc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="949fc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="949fc-125">Request body</span></span>
<span data-ttu-id="949fc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="949fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949fc-127">応答</span><span class="sxs-lookup"><span data-stu-id="949fc-127">Response</span></span>
<span data-ttu-id="949fc-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversation](../resources/conversation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="949fc-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949fc-129">例</span><span class="sxs-lookup"><span data-stu-id="949fc-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="949fc-130">要求</span><span class="sxs-lookup"><span data-stu-id="949fc-130">Request</span></span>
<span data-ttu-id="949fc-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="949fc-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="949fc-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="949fc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="949fc-133">C#</span><span class="sxs-lookup"><span data-stu-id="949fc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="949fc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="949fc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="949fc-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="949fc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="949fc-136">Java</span><span class="sxs-lookup"><span data-stu-id="949fc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="949fc-137">応答</span><span class="sxs-lookup"><span data-stu-id="949fc-137">Response</span></span>
<span data-ttu-id="949fc-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="949fc-138">The following is an example of the response.</span></span>
><span data-ttu-id="949fc-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="949fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
