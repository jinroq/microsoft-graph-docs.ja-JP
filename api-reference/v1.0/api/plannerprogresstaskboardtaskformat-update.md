---
title: Update plannerProgressTaskBoardTaskFormat
description: '**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c21e364d292dfa446b4b5441ad9d1f8d3020a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987231"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="ee912-103">Update plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ee912-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="ee912-104">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee912-104">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee912-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee912-105">Permissions</span></span>
<span data-ttu-id="ee912-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee912-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee912-108">Permission type</span></span>      | <span data-ttu-id="ee912-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee912-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee912-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee912-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee912-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee912-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee912-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee912-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee912-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee912-113">Not supported.</span></span>    |
|<span data-ttu-id="ee912-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee912-114">Application</span></span> | <span data-ttu-id="ee912-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee912-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee912-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee912-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="ee912-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee912-117">Optional request headers</span></span>
| <span data-ttu-id="ee912-118">名前</span><span class="sxs-lookup"><span data-stu-id="ee912-118">Name</span></span>       | <span data-ttu-id="ee912-119">説明</span><span class="sxs-lookup"><span data-stu-id="ee912-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee912-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee912-120">Authorization</span></span>  | <span data-ttu-id="ee912-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee912-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee912-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="ee912-123">If-Match</span></span>  | <span data-ttu-id="ee912-p103">更新する **plannerProgressTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="ee912-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee912-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee912-126">Request body</span></span>
<span data-ttu-id="ee912-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ee912-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee912-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee912-130">Property</span></span>     | <span data-ttu-id="ee912-131">型</span><span class="sxs-lookup"><span data-stu-id="ee912-131">Type</span></span>   |<span data-ttu-id="ee912-132">説明</span><span class="sxs-lookup"><span data-stu-id="ee912-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee912-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="ee912-133">orderHint</span></span>|<span data-ttu-id="ee912-134">String</span><span class="sxs-lookup"><span data-stu-id="ee912-134">String</span></span>|<span data-ttu-id="ee912-p105">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](../resources/planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="ee912-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ee912-137">応答</span><span class="sxs-lookup"><span data-stu-id="ee912-137">Response</span></span>

<span data-ttu-id="ee912-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee912-138">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="ee912-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee912-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ee912-142">例</span><span class="sxs-lookup"><span data-stu-id="ee912-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee912-143">要求</span><span class="sxs-lookup"><span data-stu-id="ee912-143">Request</span></span>
<span data-ttu-id="ee912-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee912-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="ee912-145">応答</span><span class="sxs-lookup"><span data-stu-id="ee912-145">Response</span></span>
<span data-ttu-id="ee912-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee912-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
