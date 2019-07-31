---
title: Update plannerAssignedToTaskBoardTaskFormat
description: '**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a99b4c8596feea684d4f9d1edf7b053a1cd391cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983482"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="061c0-103">Update plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="061c0-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="061c0-104">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="061c0-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="061c0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="061c0-105">Permissions</span></span>
<span data-ttu-id="061c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="061c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="061c0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="061c0-108">Permission type</span></span>      | <span data-ttu-id="061c0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="061c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="061c0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="061c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="061c0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="061c0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="061c0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="061c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="061c0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="061c0-113">Not supported.</span></span>    |
|<span data-ttu-id="061c0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="061c0-114">Application</span></span> | <span data-ttu-id="061c0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="061c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="061c0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="061c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="061c0-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="061c0-117">Optional request headers</span></span>
| <span data-ttu-id="061c0-118">名前</span><span class="sxs-lookup"><span data-stu-id="061c0-118">Name</span></span>       | <span data-ttu-id="061c0-119">説明</span><span class="sxs-lookup"><span data-stu-id="061c0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="061c0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="061c0-120">Authorization</span></span>  | <span data-ttu-id="061c0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="061c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="061c0-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="061c0-123">If-Match</span></span>  | <span data-ttu-id="061c0-p103">更新する **plannerAssignedToTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="061c0-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="061c0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="061c0-126">Request body</span></span>
<span data-ttu-id="061c0-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="061c0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="061c0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="061c0-130">Property</span></span>     | <span data-ttu-id="061c0-131">型</span><span class="sxs-lookup"><span data-stu-id="061c0-131">Type</span></span>   |<span data-ttu-id="061c0-132">説明</span><span class="sxs-lookup"><span data-stu-id="061c0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="061c0-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="061c0-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="061c0-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="061c0-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="061c0-135">タスクボードの担当者ビューでタスクの順序付けに使用されるヒントの辞書。</span><span class="sxs-lookup"><span data-stu-id="061c0-135">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="061c0-136">各エントリのキーは、タスクが割り当てられているユーザーの1人で、値は order ヒントです。</span><span class="sxs-lookup"><span data-stu-id="061c0-136">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="061c0-137">各値の形式は、[プランナーの order ヒントを使用して定義されています (../resources/プラン (英語) (英語)。</span><span class="sxs-lookup"><span data-stu-id="061c0-137">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="061c0-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="061c0-138">unassignedOrderHint</span></span>|<span data-ttu-id="061c0-139">String</span><span class="sxs-lookup"><span data-stu-id="061c0-139">String</span></span>|<span data-ttu-id="061c0-140">タスクが他のユーザーに割り当てられていない場合、または orderHintsByAssignee 辞書がタスクを割り当てられているユーザーのための order ヒントを提供していない場合に、タスクボードの担当者ビューでタスクを順序付けるために使用されるヒント値。</span><span class="sxs-lookup"><span data-stu-id="061c0-140">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="061c0-141">この形式は、 [Planner の order ヒントを使用し](../resources/planner-order-hint-format.md)て定義されます。</span><span class="sxs-lookup"><span data-stu-id="061c0-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="061c0-142">応答</span><span class="sxs-lookup"><span data-stu-id="061c0-142">Response</span></span>

<span data-ttu-id="061c0-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="061c0-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="061c0-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="061c0-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="061c0-147">例</span><span class="sxs-lookup"><span data-stu-id="061c0-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="061c0-148">要求</span><span class="sxs-lookup"><span data-stu-id="061c0-148">Request</span></span>
<span data-ttu-id="061c0-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="061c0-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="061c0-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="061c0-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="061c0-151">C#</span><span class="sxs-lookup"><span data-stu-id="061c0-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="061c0-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="061c0-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="061c0-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="061c0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="061c0-154">Java</span><span class="sxs-lookup"><span data-stu-id="061c0-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="061c0-155">応答</span><span class="sxs-lookup"><span data-stu-id="061c0-155">Response</span></span>
<span data-ttu-id="061c0-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="061c0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
