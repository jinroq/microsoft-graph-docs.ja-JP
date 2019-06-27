---
title: Get plannerTaskDetails
description: '**plannertaskdetails** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75645b01e8f5ff5528791854bfe3219445ae41b5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276483"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="af8d7-103">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="af8d7-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="af8d7-104">**plannertaskdetails** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="af8d7-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="af8d7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af8d7-105">Permissions</span></span>
<span data-ttu-id="af8d7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af8d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8d7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af8d7-108">Permission type</span></span>      | <span data-ttu-id="af8d7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af8d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8d7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af8d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af8d7-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8d7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af8d7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af8d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8d7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8d7-113">Not supported.</span></span>    |
|<span data-ttu-id="af8d7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af8d7-114">Application</span></span> | <span data-ttu-id="af8d7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8d7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8d7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af8d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="af8d7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af8d7-117">Request headers</span></span>
| <span data-ttu-id="af8d7-118">名前</span><span class="sxs-lookup"><span data-stu-id="af8d7-118">Name</span></span>      |<span data-ttu-id="af8d7-119">説明</span><span class="sxs-lookup"><span data-stu-id="af8d7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af8d7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="af8d7-120">Authorization</span></span>  | <span data-ttu-id="af8d7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af8d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af8d7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="af8d7-123">Request body</span></span>
<span data-ttu-id="af8d7-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="af8d7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af8d7-125">応答</span><span class="sxs-lookup"><span data-stu-id="af8d7-125">Response</span></span>

<span data-ttu-id="af8d7-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerTaskDetails](../resources/plannertaskdetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="af8d7-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="af8d7-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af8d7-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="af8d7-130">例</span><span class="sxs-lookup"><span data-stu-id="af8d7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af8d7-131">要求</span><span class="sxs-lookup"><span data-stu-id="af8d7-131">Request</span></span>
<span data-ttu-id="af8d7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af8d7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="af8d7-133">応答</span><span class="sxs-lookup"><span data-stu-id="af8d7-133">Response</span></span>
<span data-ttu-id="af8d7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af8d7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="af8d7-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="af8d7-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="af8d7-138">C#</span><span class="sxs-lookup"><span data-stu-id="af8d7-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af8d7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="af8d7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="af8d7-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="af8d7-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_plannertaskdetails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannertaskdetails-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
