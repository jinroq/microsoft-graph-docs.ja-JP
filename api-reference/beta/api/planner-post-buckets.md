---
title: Create plannerBucket
description: この API を使用して、新しい **plannerBucket** を作成します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b04dd3337f07930e8abd893bb34ea52937199146
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413539"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="34463-103">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="34463-103">Create plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34463-104">この API を使用して、新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="34463-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="34463-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34463-105">Permissions</span></span>
<span data-ttu-id="34463-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34463-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34463-108">Permission type</span></span>      | <span data-ttu-id="34463-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34463-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34463-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34463-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34463-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34463-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34463-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34463-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34463-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34463-113">Not supported.</span></span>    |
|<span data-ttu-id="34463-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34463-114">Application</span></span> | <span data-ttu-id="34463-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34463-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34463-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34463-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="34463-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34463-117">Request headers</span></span>
| <span data-ttu-id="34463-118">名前</span><span class="sxs-lookup"><span data-stu-id="34463-118">Name</span></span>       | <span data-ttu-id="34463-119">説明</span><span class="sxs-lookup"><span data-stu-id="34463-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34463-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="34463-120">Authorization</span></span>  | <span data-ttu-id="34463-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34463-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34463-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="34463-123">Request body</span></span>
<span data-ttu-id="34463-124">要求本文で、[plannerBucket](../resources/plannerbucket.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34463-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="34463-125">応答</span><span class="sxs-lookup"><span data-stu-id="34463-125">Response</span></span>

<span data-ttu-id="34463-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34463-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="34463-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34463-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="34463-130">例</span><span class="sxs-lookup"><span data-stu-id="34463-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34463-131">要求</span><span class="sxs-lookup"><span data-stu-id="34463-131">Request</span></span>
<span data-ttu-id="34463-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34463-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34463-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="34463-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34463-134">C#</span><span class="sxs-lookup"><span data-stu-id="34463-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerbucket-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34463-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34463-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerbucket-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34463-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="34463-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerbucket-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="34463-137">要求本文で、[plannerBucket](../resources/plannerbucket.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34463-137">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="34463-138">応答</span><span class="sxs-lookup"><span data-stu-id="34463-138">Response</span></span>
<span data-ttu-id="34463-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34463-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
