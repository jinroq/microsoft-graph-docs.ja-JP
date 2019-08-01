---
title: List buckets
description: '**plannerbucket** オブジェクトのリストを取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 74ff036e3819b40ff9336806d49d9c7bb73d488b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022503"
---
# <a name="list-buckets"></a><span data-ttu-id="5b4f1-103">List buckets</span><span class="sxs-lookup"><span data-stu-id="5b4f1-103">List buckets</span></span>

<span data-ttu-id="5b4f1-104">**plannerbucket** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-104">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4f1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b4f1-105">Permissions</span></span>
<span data-ttu-id="5b4f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4f1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b4f1-108">Permission type</span></span>      | <span data-ttu-id="5b4f1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b4f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b4f1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b4f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b4f1-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4f1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b4f1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b4f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b4f1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-113">Not supported.</span></span>    |
|<span data-ttu-id="5b4f1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b4f1-114">Application</span></span> | <span data-ttu-id="5b4f1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b4f1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b4f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b4f1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b4f1-117">Optional query parameters</span></span>
<span data-ttu-id="5b4f1-118">このメソッドでは planId [フィルター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b4f1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b4f1-119">Request headers</span></span>
| <span data-ttu-id="5b4f1-120">名前</span><span class="sxs-lookup"><span data-stu-id="5b4f1-120">Name</span></span>      |<span data-ttu-id="5b4f1-121">説明</span><span class="sxs-lookup"><span data-stu-id="5b4f1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b4f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b4f1-122">Authorization</span></span>  | <span data-ttu-id="5b4f1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b4f1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b4f1-125">Request body</span></span>
<span data-ttu-id="5b4f1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4f1-127">応答</span><span class="sxs-lookup"><span data-stu-id="5b4f1-127">Response</span></span>

<span data-ttu-id="5b4f1-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="5b4f1-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="5b4f1-132">例</span><span class="sxs-lookup"><span data-stu-id="5b4f1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b4f1-133">要求</span><span class="sxs-lookup"><span data-stu-id="5b4f1-133">Request</span></span>
<span data-ttu-id="5b4f1-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b4f1-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5b4f1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b4f1-136">C#</span><span class="sxs-lookup"><span data-stu-id="5b4f1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b4f1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b4f1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b4f1-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="5b4f1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5b4f1-139">Java</span><span class="sxs-lookup"><span data-stu-id="5b4f1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b4f1-140">応答</span><span class="sxs-lookup"><span data-stu-id="5b4f1-140">Response</span></span>
<span data-ttu-id="5b4f1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b4f1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
