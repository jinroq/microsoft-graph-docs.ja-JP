---
title: Get plannerBucketTaskBoardTaskFormat
description: '**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: de0092d36f9ceef3d42b1157273930874ddb1fc6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264457"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="95fda-103">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="95fda-103">Get plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95fda-104">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="95fda-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="95fda-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95fda-105">Permissions</span></span>
<span data-ttu-id="95fda-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95fda-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95fda-108">Permission type</span></span>      | <span data-ttu-id="95fda-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95fda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95fda-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95fda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95fda-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fda-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95fda-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95fda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95fda-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fda-113">Not supported.</span></span>    |
|<span data-ttu-id="95fda-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95fda-114">Application</span></span> | <span data-ttu-id="95fda-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fda-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95fda-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95fda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="95fda-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95fda-117">Request headers</span></span>
| <span data-ttu-id="95fda-118">名前</span><span class="sxs-lookup"><span data-stu-id="95fda-118">Name</span></span>      |<span data-ttu-id="95fda-119">説明</span><span class="sxs-lookup"><span data-stu-id="95fda-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="95fda-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95fda-120">Authorization</span></span>  | <span data-ttu-id="95fda-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95fda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95fda-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="95fda-123">Request body</span></span>
<span data-ttu-id="95fda-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95fda-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95fda-125">応答</span><span class="sxs-lookup"><span data-stu-id="95fda-125">Response</span></span>

<span data-ttu-id="95fda-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95fda-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="95fda-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95fda-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="95fda-130">例</span><span class="sxs-lookup"><span data-stu-id="95fda-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95fda-131">要求</span><span class="sxs-lookup"><span data-stu-id="95fda-131">Request</span></span>
<span data-ttu-id="95fda-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95fda-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="95fda-133">応答</span><span class="sxs-lookup"><span data-stu-id="95fda-133">Response</span></span>
<span data-ttu-id="95fda-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95fda-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="95fda-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="95fda-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="95fda-138">C#</span><span class="sxs-lookup"><span data-stu-id="95fda-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95fda-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="95fda-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="95fda-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="95fda-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
