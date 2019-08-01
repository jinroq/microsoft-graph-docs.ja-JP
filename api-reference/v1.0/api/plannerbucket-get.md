---
title: Get plannerBucket
description: '**plannerBucket** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 4277e94f84549547205c48b12cc6145450b9fe8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976181"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="1c520-103">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1c520-103">Get plannerBucket</span></span>

<span data-ttu-id="1c520-104">**plannerBucket** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="1c520-104">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c520-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c520-105">Permissions</span></span>
<span data-ttu-id="1c520-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c520-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c520-108">Permission type</span></span>      | <span data-ttu-id="1c520-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c520-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c520-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c520-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c520-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c520-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c520-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c520-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c520-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c520-113">Not supported.</span></span>    |
|<span data-ttu-id="1c520-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c520-114">Application</span></span> | <span data-ttu-id="1c520-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c520-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c520-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c520-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c520-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c520-117">Request headers</span></span>
| <span data-ttu-id="1c520-118">名前</span><span class="sxs-lookup"><span data-stu-id="1c520-118">Name</span></span>      |<span data-ttu-id="1c520-119">説明</span><span class="sxs-lookup"><span data-stu-id="1c520-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c520-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c520-120">Authorization</span></span>  | <span data-ttu-id="1c520-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c520-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c520-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c520-123">Request body</span></span>
<span data-ttu-id="1c520-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c520-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c520-125">応答</span><span class="sxs-lookup"><span data-stu-id="1c520-125">Response</span></span>

<span data-ttu-id="1c520-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c520-126">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="1c520-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c520-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="1c520-130">例</span><span class="sxs-lookup"><span data-stu-id="1c520-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c520-131">要求</span><span class="sxs-lookup"><span data-stu-id="1c520-131">Request</span></span>
<span data-ttu-id="1c520-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c520-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c520-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c520-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c520-134">C#</span><span class="sxs-lookup"><span data-stu-id="1c520-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c520-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c520-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c520-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c520-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c520-137">Java</span><span class="sxs-lookup"><span data-stu-id="1c520-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c520-138">応答</span><span class="sxs-lookup"><span data-stu-id="1c520-138">Response</span></span>
<span data-ttu-id="1c520-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c520-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
