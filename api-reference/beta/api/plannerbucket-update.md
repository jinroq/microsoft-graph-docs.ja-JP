---
title: Update plannerbucket
description: '**plannerbucket** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a041df5f7acf26a5e8df2a8d050e7f27d3b5d8a4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349492"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="9a643-103">Update plannerbucket</span><span class="sxs-lookup"><span data-stu-id="9a643-103">Update plannerbucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a643-104">**plannerbucket** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a643-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a643-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a643-105">Permissions</span></span>
<span data-ttu-id="9a643-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a643-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a643-108">Permission type</span></span>      | <span data-ttu-id="9a643-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a643-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a643-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a643-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a643-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a643-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a643-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a643-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a643-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a643-113">Not supported.</span></span>    |
|<span data-ttu-id="9a643-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a643-114">Application</span></span> | <span data-ttu-id="9a643-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a643-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a643-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a643-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a643-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a643-117">Optional request headers</span></span>
| <span data-ttu-id="9a643-118">名前</span><span class="sxs-lookup"><span data-stu-id="9a643-118">Name</span></span>       | <span data-ttu-id="9a643-119">説明</span><span class="sxs-lookup"><span data-stu-id="9a643-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a643-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a643-120">Authorization</span></span>  | <span data-ttu-id="9a643-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a643-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a643-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="9a643-123">If-Match</span></span>  | <span data-ttu-id="9a643-p103">更新する **plannerBucket** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="9a643-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a643-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a643-126">Request body</span></span>
<span data-ttu-id="9a643-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9a643-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a643-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a643-130">Property</span></span>     | <span data-ttu-id="9a643-131">型</span><span class="sxs-lookup"><span data-stu-id="9a643-131">Type</span></span>   |<span data-ttu-id="9a643-132">説明</span><span class="sxs-lookup"><span data-stu-id="9a643-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a643-133">name</span><span class="sxs-lookup"><span data-stu-id="9a643-133">name</span></span>|<span data-ttu-id="9a643-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9a643-134">String</span></span>|<span data-ttu-id="9a643-135">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="9a643-135">Name of the bucket.</span></span>|
|<span data-ttu-id="9a643-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="9a643-136">orderHint</span></span>|<span data-ttu-id="9a643-137">String</span><span class="sxs-lookup"><span data-stu-id="9a643-137">String</span></span>|<span data-ttu-id="9a643-p105">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](../resources/planner-order-hint-format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="9a643-p105">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9a643-140">planId</span><span class="sxs-lookup"><span data-stu-id="9a643-140">planId</span></span>|<span data-ttu-id="9a643-141">String</span><span class="sxs-lookup"><span data-stu-id="9a643-141">String</span></span>|<span data-ttu-id="9a643-142">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="9a643-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="9a643-143">応答</span><span class="sxs-lookup"><span data-stu-id="9a643-143">Response</span></span>

<span data-ttu-id="9a643-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerBucket](../resources/plannerbucket.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9a643-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="9a643-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a643-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9a643-148">例</span><span class="sxs-lookup"><span data-stu-id="9a643-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a643-149">要求</span><span class="sxs-lookup"><span data-stu-id="9a643-149">Request</span></span>
<span data-ttu-id="9a643-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a643-150">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a643-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9a643-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a643-152">C#</span><span class="sxs-lookup"><span data-stu-id="9a643-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a643-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a643-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a643-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="9a643-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a643-155">Java</span><span class="sxs-lookup"><span data-stu-id="9a643-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a643-156">応答</span><span class="sxs-lookup"><span data-stu-id="9a643-156">Response</span></span>
<span data-ttu-id="9a643-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a643-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "name": "Development",
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
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
