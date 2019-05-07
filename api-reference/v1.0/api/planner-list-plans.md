---
title: 計画を一覧表示する
description: '**plannerplan** オブジェクトのリストを取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: c783a09ba7cef3dc2cf5a7d329d183ff2dae1e4e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611500"
---
# <a name="list-plans"></a><span data-ttu-id="e2786-103">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e2786-103">List plans</span></span>

<span data-ttu-id="e2786-104">**plannerplan** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2786-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2786-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2786-105">Permissions</span></span>
<span data-ttu-id="e2786-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2786-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2786-108">Permission type</span></span>      | <span data-ttu-id="e2786-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2786-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2786-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2786-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2786-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2786-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2786-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2786-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2786-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2786-113">Not supported.</span></span>    |
|<span data-ttu-id="e2786-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2786-114">Application</span></span> | <span data-ttu-id="e2786-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2786-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2786-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2786-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2786-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2786-117">Optional query parameters</span></span>
<span data-ttu-id="e2786-118">このメソッドでは owner [フィルター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2786-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2786-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2786-119">Request headers</span></span>
| <span data-ttu-id="e2786-120">名前</span><span class="sxs-lookup"><span data-stu-id="e2786-120">Name</span></span>      |<span data-ttu-id="e2786-121">説明</span><span class="sxs-lookup"><span data-stu-id="e2786-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2786-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2786-122">Authorization</span></span>  | <span data-ttu-id="e2786-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2786-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2786-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2786-125">Request body</span></span>
<span data-ttu-id="e2786-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2786-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2786-127">応答</span><span class="sxs-lookup"><span data-stu-id="e2786-127">Response</span></span>

<span data-ttu-id="e2786-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e2786-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="e2786-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2786-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e2786-132">例</span><span class="sxs-lookup"><span data-stu-id="e2786-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2786-133">要求</span><span class="sxs-lookup"><span data-stu-id="e2786-133">Request</span></span>
<span data-ttu-id="e2786-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2786-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
##### <a name="response"></a><span data-ttu-id="e2786-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2786-135">Response</span></span>
<span data-ttu-id="e2786-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2786-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2786-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e2786-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2786-140">Visual</span><span class="sxs-lookup"><span data-stu-id="e2786-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2786-141">Java</span><span class="sxs-lookup"><span data-stu-id="e2786-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plans-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
