---
title: Update plannerProgressTaskBoardTaskFormat
description: '**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2d34ff4a30f713c99089fc96421557af1c4ff363
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264373"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="e3061-103">Update plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e3061-103">Update plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3061-104">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3061-104">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3061-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3061-105">Permissions</span></span>
<span data-ttu-id="e3061-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3061-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3061-108">Permission type</span></span>      | <span data-ttu-id="e3061-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3061-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3061-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3061-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3061-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3061-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3061-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3061-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3061-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3061-113">Not supported.</span></span>    |
|<span data-ttu-id="e3061-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3061-114">Application</span></span> | <span data-ttu-id="e3061-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3061-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3061-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3061-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="e3061-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3061-117">Optional request headers</span></span>
| <span data-ttu-id="e3061-118">名前</span><span class="sxs-lookup"><span data-stu-id="e3061-118">Name</span></span>       | <span data-ttu-id="e3061-119">説明</span><span class="sxs-lookup"><span data-stu-id="e3061-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e3061-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3061-120">Authorization</span></span>  | <span data-ttu-id="e3061-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3061-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3061-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="e3061-123">If-Match</span></span>  | <span data-ttu-id="e3061-p103">更新する **plannerProgressTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="e3061-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3061-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3061-126">Request body</span></span>
<span data-ttu-id="e3061-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e3061-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e3061-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3061-130">Property</span></span>     | <span data-ttu-id="e3061-131">型</span><span class="sxs-lookup"><span data-stu-id="e3061-131">Type</span></span>   |<span data-ttu-id="e3061-132">説明</span><span class="sxs-lookup"><span data-stu-id="e3061-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3061-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="e3061-133">orderHint</span></span>|<span data-ttu-id="e3061-134">String</span><span class="sxs-lookup"><span data-stu-id="e3061-134">String</span></span>|<span data-ttu-id="e3061-135">タスクボードの進行状況ビューでタスクを順序付けするために使用されるヒントの値。</span><span class="sxs-lookup"><span data-stu-id="e3061-135">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="e3061-136">この形式は、 [Planner の order ヒントを使用し](../resources/planner-order-hint-format.md)て定義されます。</span><span class="sxs-lookup"><span data-stu-id="e3061-136">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e3061-137">応答</span><span class="sxs-lookup"><span data-stu-id="e3061-137">Response</span></span>

<span data-ttu-id="e3061-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3061-138">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e3061-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3061-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e3061-142">例</span><span class="sxs-lookup"><span data-stu-id="e3061-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3061-143">要求</span><span class="sxs-lookup"><span data-stu-id="e3061-143">Request</span></span>
<span data-ttu-id="e3061-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3061-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="e3061-145">応答</span><span class="sxs-lookup"><span data-stu-id="e3061-145">Response</span></span>
<span data-ttu-id="e3061-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3061-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3061-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e3061-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3061-150">C#</span><span class="sxs-lookup"><span data-stu-id="e3061-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerprogresstaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3061-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3061-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerprogresstaskboardtaskformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e3061-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3061-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerprogresstaskboardtaskformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
