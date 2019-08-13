---
title: プランを更新する plan
description: '**Plan**オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a88d8e7df9bc5d113c0cdd04fe0ef53ba4153435
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375920"
---
# <a name="update-plannerplan"></a><span data-ttu-id="7acf6-103">プランを更新する plan</span><span class="sxs-lookup"><span data-stu-id="7acf6-103">Update plannerPlan</span></span>

<span data-ttu-id="7acf6-104">**Plan**オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7acf6-104">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7acf6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7acf6-105">Permissions</span></span>
<span data-ttu-id="7acf6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7acf6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7acf6-108">Permission type</span></span>      | <span data-ttu-id="7acf6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7acf6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7acf6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7acf6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7acf6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7acf6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7acf6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7acf6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7acf6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7acf6-113">Not supported.</span></span>    |
|<span data-ttu-id="7acf6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7acf6-114">Application</span></span> | <span data-ttu-id="7acf6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7acf6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7acf6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7acf6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="7acf6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7acf6-117">Request headers</span></span>

| <span data-ttu-id="7acf6-118">名前</span><span class="sxs-lookup"><span data-stu-id="7acf6-118">Name</span></span>       | <span data-ttu-id="7acf6-119">説明</span><span class="sxs-lookup"><span data-stu-id="7acf6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7acf6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7acf6-120">Authorization</span></span>  | <span data-ttu-id="7acf6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7acf6-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="7acf6-123">If-Match</span></span>  | <span data-ttu-id="7acf6-p103">更新する plannerPlan の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7acf6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7acf6-126">Request body</span></span>
<span data-ttu-id="7acf6-127">要求本文で、関連するフィールドの値を [更新済み] に指定します。</span><span class="sxs-lookup"><span data-stu-id="7acf6-127">In the request body, supply the values for relevant fields to updated.</span></span> <span data-ttu-id="7acf6-128">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="7acf6-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7acf6-129">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7acf6-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7acf6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7acf6-130">Property</span></span>     | <span data-ttu-id="7acf6-131">型</span><span class="sxs-lookup"><span data-stu-id="7acf6-131">Type</span></span>   |<span data-ttu-id="7acf6-132">説明</span><span class="sxs-lookup"><span data-stu-id="7acf6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7acf6-133">owner</span><span class="sxs-lookup"><span data-stu-id="7acf6-133">owner</span></span>|<span data-ttu-id="7acf6-134">String</span><span class="sxs-lookup"><span data-stu-id="7acf6-134">String</span></span>|<span data-ttu-id="7acf6-p105">計画を所有する [グループ](../resources/group.md) `id`。このフィールドを設定するためには、有効なグループが存在していなければなりません。一度設定したら、所有者のみが更新できます。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="7acf6-138">title</span><span class="sxs-lookup"><span data-stu-id="7acf6-138">title</span></span>|<span data-ttu-id="7acf6-139">String</span><span class="sxs-lookup"><span data-stu-id="7acf6-139">String</span></span>|<span data-ttu-id="7acf6-140">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="7acf6-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="7acf6-141">応答</span><span class="sxs-lookup"><span data-stu-id="7acf6-141">Response</span></span>

<span data-ttu-id="7acf6-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[プランのプラン](../resources/plannerplan.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7acf6-142">If successful, this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="7acf6-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7acf6-146">例</span><span class="sxs-lookup"><span data-stu-id="7acf6-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7acf6-147">要求</span><span class="sxs-lookup"><span data-stu-id="7acf6-147">Request</span></span>
<span data-ttu-id="7acf6-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7acf6-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7acf6-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7acf6-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7acf6-150">C#</span><span class="sxs-lookup"><span data-stu-id="7acf6-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7acf6-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7acf6-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7acf6-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="7acf6-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7acf6-153">Java</span><span class="sxs-lookup"><span data-stu-id="7acf6-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7acf6-154">応答</span><span class="sxs-lookup"><span data-stu-id="7acf6-154">Response</span></span>
<span data-ttu-id="7acf6-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7acf6-155">Here is an example of the response.</span></span> 

><span data-ttu-id="7acf6-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7acf6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
