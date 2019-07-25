---
title: 計画を一覧表示する
description: user オブジェクトで共有する **plannerplan** オブジェクトのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2b016f006aebe39e0916cdc06b50bc0039081b38
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887027"
---
# <a name="list-plans"></a><span data-ttu-id="30948-103">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="30948-103">List plans</span></span>

<span data-ttu-id="30948-104">[user](../resources/user.md) オブジェクトで共有する **plannerplan** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="30948-104">Retrieve a list of **plannerplan** objects shared with a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30948-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="30948-105">Permissions</span></span>
<span data-ttu-id="30948-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30948-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30948-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30948-108">Permission type</span></span>      | <span data-ttu-id="30948-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="30948-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30948-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30948-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30948-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30948-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="30948-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30948-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30948-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30948-113">Not supported.</span></span>    |
|<span data-ttu-id="30948-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30948-114">Application</span></span> | <span data-ttu-id="30948-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30948-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30948-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30948-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/plans
GET /users/{id}/planner/plans
GET /drive/root/createdByUser/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="30948-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30948-117">Request headers</span></span>
| <span data-ttu-id="30948-118">名前</span><span class="sxs-lookup"><span data-stu-id="30948-118">Name</span></span>      |<span data-ttu-id="30948-119">説明</span><span class="sxs-lookup"><span data-stu-id="30948-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30948-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="30948-120">Authorization</span></span>  | <span data-ttu-id="30948-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="30948-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30948-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="30948-123">Request body</span></span>
<span data-ttu-id="30948-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="30948-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30948-125">応答</span><span class="sxs-lookup"><span data-stu-id="30948-125">Response</span></span>

<span data-ttu-id="30948-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="30948-126">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="30948-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30948-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="30948-130">例</span><span class="sxs-lookup"><span data-stu-id="30948-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30948-131">要求</span><span class="sxs-lookup"><span data-stu-id="30948-131">Request</span></span>
<span data-ttu-id="30948-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30948-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30948-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="30948-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/planner/plans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30948-134">C#</span><span class="sxs-lookup"><span data-stu-id="30948-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30948-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="30948-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30948-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="30948-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30948-137">Java</span><span class="sxs-lookup"><span data-stu-id="30948-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30948-138">応答</span><span class="sxs-lookup"><span data-stu-id="30948-138">Response</span></span>
<span data-ttu-id="30948-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30948-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 438

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
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
