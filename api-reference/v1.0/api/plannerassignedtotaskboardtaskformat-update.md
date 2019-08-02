---
title: Update plannerAssignedToTaskBoardTaskFormat
description: '**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: b250b3d2a3bc611b6d188222197b9d7de47944bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976216"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="a594c-103">Update plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a594c-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="a594c-104">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a594c-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a594c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a594c-105">Permissions</span></span>
<span data-ttu-id="a594c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a594c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a594c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a594c-108">Permission type</span></span>      | <span data-ttu-id="a594c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a594c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a594c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a594c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a594c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a594c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a594c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a594c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a594c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a594c-113">Not supported.</span></span>    |
|<span data-ttu-id="a594c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a594c-114">Application</span></span> | <span data-ttu-id="a594c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a594c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a594c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a594c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="a594c-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a594c-117">Optional request headers</span></span>
| <span data-ttu-id="a594c-118">名前</span><span class="sxs-lookup"><span data-stu-id="a594c-118">Name</span></span>       | <span data-ttu-id="a594c-119">説明</span><span class="sxs-lookup"><span data-stu-id="a594c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a594c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a594c-120">Authorization</span></span>  | <span data-ttu-id="a594c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a594c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a594c-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="a594c-123">If-Match</span></span>  | <span data-ttu-id="a594c-p103">更新する **plannerAssignedToTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="a594c-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a594c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a594c-126">Request body</span></span>
<span data-ttu-id="a594c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a594c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a594c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a594c-130">Property</span></span>     | <span data-ttu-id="a594c-131">型</span><span class="sxs-lookup"><span data-stu-id="a594c-131">Type</span></span>   |<span data-ttu-id="a594c-132">説明</span><span class="sxs-lookup"><span data-stu-id="a594c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a594c-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="a594c-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="a594c-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="a594c-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="a594c-p105">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](../resources/planner-order-hint-format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="a594c-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="a594c-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="a594c-138">unassignedOrderHint</span></span>|<span data-ttu-id="a594c-139">String</span><span class="sxs-lookup"><span data-stu-id="a594c-139">String</span></span>|<span data-ttu-id="a594c-p106">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](../resources/planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="a594c-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a594c-142">応答</span><span class="sxs-lookup"><span data-stu-id="a594c-142">Response</span></span>

<span data-ttu-id="a594c-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a594c-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="a594c-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a594c-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a594c-147">例</span><span class="sxs-lookup"><span data-stu-id="a594c-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a594c-148">要求</span><span class="sxs-lookup"><span data-stu-id="a594c-148">Request</span></span>
<span data-ttu-id="a594c-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a594c-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a594c-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a594c-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a594c-151">C#</span><span class="sxs-lookup"><span data-stu-id="a594c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a594c-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="a594c-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a594c-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="a594c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a594c-154">Java</span><span class="sxs-lookup"><span data-stu-id="a594c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a594c-155">応答</span><span class="sxs-lookup"><span data-stu-id="a594c-155">Response</span></span>
<span data-ttu-id="a594c-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a594c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
