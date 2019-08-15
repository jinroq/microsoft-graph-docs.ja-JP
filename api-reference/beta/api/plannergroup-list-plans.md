---
title: 計画を一覧表示する
description: グループ オブジェクトが所有する **plannerPlan** オブジェクトのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a1d2c677f8ee61f0afdb3190f3abb53eb803156f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413378"
---
# <a name="list-plans"></a><span data-ttu-id="f6026-103">計画をリストする</span><span class="sxs-lookup"><span data-stu-id="f6026-103">List plans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6026-104">[group](../resources/group.md) オブジェクトが所有する **plannerPlan** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f6026-104">Retrieve a list of **plannerPlan** objects owned by a [group](../resources/group.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6026-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6026-105">Permissions</span></span>
<span data-ttu-id="f6026-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6026-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6026-108">Permission type</span></span>      | <span data-ttu-id="f6026-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6026-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6026-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6026-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6026-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6026-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6026-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6026-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6026-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6026-113">Not supported.</span></span>    |
|<span data-ttu-id="f6026-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6026-114">Application</span></span> | <span data-ttu-id="f6026-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6026-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6026-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6026-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="f6026-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6026-117">Request headers</span></span>
| <span data-ttu-id="f6026-118">名前</span><span class="sxs-lookup"><span data-stu-id="f6026-118">Name</span></span>      |<span data-ttu-id="f6026-119">説明</span><span class="sxs-lookup"><span data-stu-id="f6026-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6026-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6026-120">Authorization</span></span>  | <span data-ttu-id="f6026-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6026-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6026-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6026-123">Request body</span></span>
<span data-ttu-id="f6026-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f6026-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6026-125">応答</span><span class="sxs-lookup"><span data-stu-id="f6026-125">Response</span></span>

<span data-ttu-id="f6026-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f6026-126">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="f6026-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6026-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="f6026-130">例</span><span class="sxs-lookup"><span data-stu-id="f6026-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6026-131">要求</span><span class="sxs-lookup"><span data-stu-id="f6026-131">Request</span></span>
<span data-ttu-id="f6026-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6026-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6026-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f6026-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6026-134">C#</span><span class="sxs-lookup"><span data-stu-id="f6026-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6026-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6026-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6026-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="f6026-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6026-137">応答</span><span class="sxs-lookup"><span data-stu-id="f6026-137">Response</span></span>
<span data-ttu-id="f6026-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6026-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
