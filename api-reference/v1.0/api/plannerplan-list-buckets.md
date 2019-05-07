---
title: List buckets
description: plannerPlan オブジェクトに含まれている **plannerbucket** オブジェクトのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ecf8abb9c39f08a49af31d39244f1b079da73199
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608841"
---
# <a name="list-buckets"></a><span data-ttu-id="5a884-103">List buckets</span><span class="sxs-lookup"><span data-stu-id="5a884-103">List buckets</span></span>

<span data-ttu-id="5a884-104">[plannerPlan](../resources/plannerplan.md) オブジェクトに含まれている **plannerbucket** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a884-104">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a884-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a884-105">Permissions</span></span>
<span data-ttu-id="5a884-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a884-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a884-108">Permission type</span></span>      | <span data-ttu-id="5a884-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a884-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a884-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a884-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a884-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a884-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a884-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a884-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a884-113">Not supported.</span></span>    |
|<span data-ttu-id="5a884-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a884-114">Application</span></span> | <span data-ttu-id="5a884-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a884-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a884-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a884-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="5a884-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a884-117">Request headers</span></span>
| <span data-ttu-id="5a884-118">名前</span><span class="sxs-lookup"><span data-stu-id="5a884-118">Name</span></span>      |<span data-ttu-id="5a884-119">説明</span><span class="sxs-lookup"><span data-stu-id="5a884-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a884-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a884-120">Authorization</span></span>  | <span data-ttu-id="5a884-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a884-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a884-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a884-123">Request body</span></span>
<span data-ttu-id="5a884-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5a884-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a884-125">応答</span><span class="sxs-lookup"><span data-stu-id="5a884-125">Response</span></span>

<span data-ttu-id="5a884-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5a884-126">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="5a884-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a884-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="5a884-130">例</span><span class="sxs-lookup"><span data-stu-id="5a884-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a884-131">要求</span><span class="sxs-lookup"><span data-stu-id="5a884-131">Request</span></span>
<span data-ttu-id="5a884-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a884-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="5a884-133">応答</span><span class="sxs-lookup"><span data-stu-id="5a884-133">Response</span></span>
<span data-ttu-id="5a884-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a884-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a884-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="5a884-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a884-138">Visual</span><span class="sxs-lookup"><span data-stu-id="5a884-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_buckets-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a884-139">Java</span><span class="sxs-lookup"><span data-stu-id="5a884-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_buckets-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
