---
title: Update plannerProgressTaskBoardTaskFormat
description: '**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。'
ms.openlocfilehash: 628b17075e02bfad5859f68c118f742a11691a53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067007"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="fa5ea-103">Update plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="fa5ea-103">Update plannerProgressTaskBoardTaskFormat</span></span>

> <span data-ttu-id="fa5ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa5ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa5ea-106">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-106">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa5ea-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa5ea-107">Permissions</span></span>
<span data-ttu-id="fa5ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa5ea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa5ea-110">Permission type</span></span>      | <span data-ttu-id="fa5ea-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa5ea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa5ea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa5ea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa5ea-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa5ea-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa5ea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa5ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa5ea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-115">Not supported.</span></span>    |
|<span data-ttu-id="fa5ea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa5ea-116">Application</span></span> | <span data-ttu-id="fa5ea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa5ea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa5ea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="fa5ea-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa5ea-119">Optional request headers</span></span>
| <span data-ttu-id="fa5ea-120">名前</span><span class="sxs-lookup"><span data-stu-id="fa5ea-120">Name</span></span>       | <span data-ttu-id="fa5ea-121">説明</span><span class="sxs-lookup"><span data-stu-id="fa5ea-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fa5ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa5ea-122">Authorization</span></span>  | <span data-ttu-id="fa5ea-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa5ea-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="fa5ea-125">If-Match</span></span>  | <span data-ttu-id="fa5ea-p104">更新する **plannerProgressTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p104">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa5ea-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa5ea-128">Request body</span></span>
<span data-ttu-id="fa5ea-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa5ea-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa5ea-132">Property</span></span>     | <span data-ttu-id="fa5ea-133">型</span><span class="sxs-lookup"><span data-stu-id="fa5ea-133">Type</span></span>   |<span data-ttu-id="fa5ea-134">説明</span><span class="sxs-lookup"><span data-stu-id="fa5ea-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa5ea-135">orderHint</span><span class="sxs-lookup"><span data-stu-id="fa5ea-135">orderHint</span></span>|<span data-ttu-id="fa5ea-136">String</span><span class="sxs-lookup"><span data-stu-id="fa5ea-136">String</span></span>|<span data-ttu-id="fa5ea-137">ヒントの値を使用してタスクの掲示板の進行状況のビューで、タスクを注文します。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-137">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="fa5ea-138">[プランナーで使用する順序のヒント](../resources/planner-order-hint-format.md)の形式が定義されています。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-138">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="fa5ea-139">応答</span><span class="sxs-lookup"><span data-stu-id="fa5ea-139">Response</span></span>

<span data-ttu-id="fa5ea-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-140">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="fa5ea-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fa5ea-144">例</span><span class="sxs-lookup"><span data-stu-id="fa5ea-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa5ea-145">要求</span><span class="sxs-lookup"><span data-stu-id="fa5ea-145">Request</span></span>
<span data-ttu-id="fa5ea-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-146">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fa5ea-147">応答</span><span class="sxs-lookup"><span data-stu-id="fa5ea-147">Response</span></span>
<span data-ttu-id="fa5ea-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa5ea-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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