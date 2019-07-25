---
title: リスト recentPlans
description: ユーザーが最近閲覧した Plan プランの一覧を取得します。 プランのユーザーリソースを更新すると、最近表示されたプランを更新できます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: dd1aa46a8b270464c13373000967ec5114ca4674
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876146"
---
# <a name="list-recentplans"></a><span data-ttu-id="def66-104">リスト recentPlans</span><span class="sxs-lookup"><span data-stu-id="def66-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def66-105">ユーザーが最近閲覧した[Plan プラン](../resources/plannerplan.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="def66-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="def66-106">プラン[のユーザーリソースを更新](planneruser-update.md)すると、最近表示されたプランを更新できます。</span><span class="sxs-lookup"><span data-stu-id="def66-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="def66-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="def66-107">Permissions</span></span>
<span data-ttu-id="def66-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="def66-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def66-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="def66-110">Permission type</span></span>      | <span data-ttu-id="def66-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="def66-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="def66-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="def66-112">Delegated (work or school account)</span></span> | <span data-ttu-id="def66-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="def66-113">Group.Read.All</span></span>    |
|<span data-ttu-id="def66-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="def66-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def66-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="def66-115">Not supported.</span></span>    |
|<span data-ttu-id="def66-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="def66-116">Application</span></span> | <span data-ttu-id="def66-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="def66-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="def66-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="def66-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="def66-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="def66-119">Request headers</span></span>
| <span data-ttu-id="def66-120">名前</span><span class="sxs-lookup"><span data-stu-id="def66-120">Name</span></span>      |<span data-ttu-id="def66-121">説明</span><span class="sxs-lookup"><span data-stu-id="def66-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="def66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="def66-122">Authorization</span></span>  | <span data-ttu-id="def66-123">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="def66-123">Bearer {code}.</span></span> <span data-ttu-id="def66-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="def66-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="def66-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="def66-125">Request body</span></span>
<span data-ttu-id="def66-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="def66-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="def66-127">応答</span><span class="sxs-lookup"><span data-stu-id="def66-127">Response</span></span>
<span data-ttu-id="def66-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[プラン](../resources/plannerplan.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="def66-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="def66-129">例</span><span class="sxs-lookup"><span data-stu-id="def66-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="def66-130">要求</span><span class="sxs-lookup"><span data-stu-id="def66-130">Request</span></span>
<span data-ttu-id="def66-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="def66-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="def66-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="def66-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="def66-133">C#</span><span class="sxs-lookup"><span data-stu-id="def66-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def66-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="def66-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="def66-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="def66-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="def66-136">Java</span><span class="sxs-lookup"><span data-stu-id="def66-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recentplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="def66-137">応答</span><span class="sxs-lookup"><span data-stu-id="def66-137">Response</span></span>
<span data-ttu-id="def66-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="def66-138">The following is an example of the response.</span></span> 

><span data-ttu-id="def66-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="def66-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
