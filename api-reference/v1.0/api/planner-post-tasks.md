---
title: Create plannerTask
description: この API を使用して、新しい **plannerTask** を作成します。
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 115973cd54d6e995c02dd4ff172e7cd4e15cab46
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976188"
---
# <a name="create-plannertask"></a><span data-ttu-id="7aacd-103">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="7aacd-103">Create plannerTask</span></span>

<span data-ttu-id="7aacd-104">この API を使用して、新しい **plannerTask** を作成します。</span><span class="sxs-lookup"><span data-stu-id="7aacd-104">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="7aacd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7aacd-105">Permissions</span></span>
<span data-ttu-id="7aacd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aacd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7aacd-108">Permission type</span></span>      | <span data-ttu-id="7aacd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7aacd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aacd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7aacd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aacd-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aacd-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aacd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7aacd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aacd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aacd-113">Not supported.</span></span>    |
|<span data-ttu-id="7aacd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7aacd-114">Application</span></span> | <span data-ttu-id="7aacd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aacd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aacd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7aacd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="7aacd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aacd-117">Request headers</span></span>
| <span data-ttu-id="7aacd-118">名前</span><span class="sxs-lookup"><span data-stu-id="7aacd-118">Name</span></span>       | <span data-ttu-id="7aacd-119">説明</span><span class="sxs-lookup"><span data-stu-id="7aacd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7aacd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aacd-120">Authorization</span></span>  | <span data-ttu-id="7aacd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7aacd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aacd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7aacd-123">Request body</span></span>
<span data-ttu-id="7aacd-p103">要求本文で、[plannerTask](../resources/plannertask.md) オブジェクトの JSON 表記を指定します。**plannerTask** planId プロパティは、既存の [plannerPlan](../resources/plannerplan.md) オブジェクトの ID に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7aacd-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="7aacd-126">応答</span><span class="sxs-lookup"><span data-stu-id="7aacd-126">Response</span></span>

<span data-ttu-id="7aacd-127">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerTask](../resources/plannertask.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7aacd-127">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="7aacd-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aacd-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7aacd-131">例</span><span class="sxs-lookup"><span data-stu-id="7aacd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7aacd-132">要求</span><span class="sxs-lookup"><span data-stu-id="7aacd-132">Request</span></span>
<span data-ttu-id="7aacd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7aacd-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7aacd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aacd-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  },
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aacd-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7aacd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7aacd-136">要求本文で、[plannerTask](../resources/plannertask.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7aacd-136">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7aacd-137">応答</span><span class="sxs-lookup"><span data-stu-id="7aacd-137">Response</span></span>
<span data-ttu-id="7aacd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7aacd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
