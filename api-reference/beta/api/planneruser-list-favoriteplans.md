---
title: お気に入りのプランを一覧表示する
description: ユーザーによってお気に入りとしてマークされているプランの一覧を取得します。 プランをお気に入りとしてマークするには、プランのユーザーリソースを更新します。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8ffbd1ea494f62cec2e00596feab5d8d3cb9cfb2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268265"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="f0361-104">お気に入りのプランを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0361-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0361-105">ユーザーによってお気に入りとしてマークされている[プラン](../resources/plannerplan.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f0361-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="f0361-106">プランをお気に入りとしてマークするには、プランの[ユーザーリソースを更新](planneruser-update.md)します。</span><span class="sxs-lookup"><span data-stu-id="f0361-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0361-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0361-107">Permissions</span></span>
<span data-ttu-id="f0361-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0361-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0361-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0361-110">Permission type</span></span>      | <span data-ttu-id="f0361-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0361-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0361-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0361-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0361-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0361-113">Group.Read.All</span></span>    |
|<span data-ttu-id="f0361-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0361-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0361-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0361-115">Not supported.</span></span>    |
|<span data-ttu-id="f0361-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0361-116">Application</span></span> | <span data-ttu-id="f0361-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0361-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0361-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0361-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0361-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0361-119">Optional query parameters</span></span>
<span data-ttu-id="f0361-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0361-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0361-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0361-121">Request headers</span></span>
| <span data-ttu-id="f0361-122">名前</span><span class="sxs-lookup"><span data-stu-id="f0361-122">Name</span></span>      |<span data-ttu-id="f0361-123">説明</span><span class="sxs-lookup"><span data-stu-id="f0361-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0361-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0361-124">Authorization</span></span>  | <span data-ttu-id="f0361-125">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="f0361-125">Bearer {code}.</span></span> <span data-ttu-id="f0361-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="f0361-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0361-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0361-127">Request body</span></span>
<span data-ttu-id="f0361-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0361-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f0361-129">応答</span><span class="sxs-lookup"><span data-stu-id="f0361-129">Response</span></span>
<span data-ttu-id="f0361-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[プラン](../resources/plannerplan.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f0361-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0361-131">例</span><span class="sxs-lookup"><span data-stu-id="f0361-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0361-132">要求</span><span class="sxs-lookup"><span data-stu-id="f0361-132">Request</span></span>
<span data-ttu-id="f0361-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0361-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="f0361-134">応答</span><span class="sxs-lookup"><span data-stu-id="f0361-134">Response</span></span>
<span data-ttu-id="f0361-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0361-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f0361-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f0361-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f0361-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f0361-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f0361-139">C#</span><span class="sxs-lookup"><span data-stu-id="f0361-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_favoriteplans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0361-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f0361-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_favoriteplans-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f0361-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="f0361-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_favoriteplans-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
