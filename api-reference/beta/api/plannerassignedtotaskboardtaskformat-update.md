---
title: Update plannerAssignedToTaskBoardTaskFormat
description: '**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
localization_priority: Normal
ms.openlocfilehash: 2586e0d413ce6debcc90b720c2ec45773518507e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856806"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="d5fe7-103">Update plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d5fe7-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

> <span data-ttu-id="d5fe7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5fe7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5fe7-106">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-106">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5fe7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5fe7-107">Permissions</span></span>
<span data-ttu-id="d5fe7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5fe7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5fe7-110">Permission type</span></span>      | <span data-ttu-id="d5fe7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5fe7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5fe7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5fe7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5fe7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5fe7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5fe7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5fe7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5fe7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-115">Not supported.</span></span>    |
|<span data-ttu-id="d5fe7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5fe7-116">Application</span></span> | <span data-ttu-id="d5fe7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5fe7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5fe7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="d5fe7-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5fe7-119">Optional request headers</span></span>
| <span data-ttu-id="d5fe7-120">名前</span><span class="sxs-lookup"><span data-stu-id="d5fe7-120">Name</span></span>       | <span data-ttu-id="d5fe7-121">説明</span><span class="sxs-lookup"><span data-stu-id="d5fe7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d5fe7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5fe7-122">Authorization</span></span>  | <span data-ttu-id="d5fe7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5fe7-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="d5fe7-125">If-Match</span></span>  | <span data-ttu-id="d5fe7-p104">更新する **plannerAssignedToTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p104">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5fe7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5fe7-128">Request body</span></span>
<span data-ttu-id="d5fe7-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d5fe7-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5fe7-132">Property</span></span>     | <span data-ttu-id="d5fe7-133">種類</span><span class="sxs-lookup"><span data-stu-id="d5fe7-133">Type</span></span>   |<span data-ttu-id="d5fe7-134">説明</span><span class="sxs-lookup"><span data-stu-id="d5fe7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5fe7-135">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d5fe7-135">orderHintsByAssignee</span></span>|[<span data-ttu-id="d5fe7-136">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d5fe7-136">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="d5fe7-137">担当者、タスク掲示板のビューでタスクを注文するために使用するヒントのディクショナリ。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-137">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="d5fe7-138">タスクが割り当てられているユーザーの 1 つは、各エントリのキーと値は、order ヒントです。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-138">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="d5fe7-139">各値の形式が定義されている [プランナー] の [順序のヒントを使用して (../resources/planner_order_hint_format.md)。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-139">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="d5fe7-140">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d5fe7-140">unassignedOrderHint</span></span>|<span data-ttu-id="d5fe7-141">String</span><span class="sxs-lookup"><span data-stu-id="d5fe7-141">String</span></span>|<span data-ttu-id="d5fe7-142">すべてのユーザーにタスクが割り当てられていない場合、または orderHintsByAssignee の辞書は、タスクのユーザーの order ヒントを提供していない場合、担当者の作業掲示板のビューでタスクを注文するために使用するヒントの値が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-142">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="d5fe7-143">[プランナーで使用する順序のヒント](../resources/planner-order-hint-format.md)の形式が定義されています。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-143">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d5fe7-144">応答</span><span class="sxs-lookup"><span data-stu-id="d5fe7-144">Response</span></span>

<span data-ttu-id="d5fe7-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-145">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="d5fe7-p108">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d5fe7-149">例</span><span class="sxs-lookup"><span data-stu-id="d5fe7-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5fe7-150">要求</span><span class="sxs-lookup"><span data-stu-id="d5fe7-150">Request</span></span>
<span data-ttu-id="d5fe7-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-151">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d5fe7-152">応答</span><span class="sxs-lookup"><span data-stu-id="d5fe7-152">Response</span></span>
<span data-ttu-id="d5fe7-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5fe7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
