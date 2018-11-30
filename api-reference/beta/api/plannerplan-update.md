---
title: PlannerPlan を更新します。
description: '**PlannerPlan**オブジェクトのプロパティを更新します。'
ms.openlocfilehash: 477246b442971693c2748d9f2cde10ac46b8ef0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074389"
---
# <a name="update-plannerplan"></a><span data-ttu-id="3f3c5-103">PlannerPlan を更新します。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-103">Update plannerPlan</span></span>

> <span data-ttu-id="3f3c5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f3c5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f3c5-106">**PlannerPlan**オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-106">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f3c5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f3c5-107">Permissions</span></span>
<span data-ttu-id="3f3c5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f3c5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f3c5-110">Permission type</span></span>      | <span data-ttu-id="3f3c5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f3c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f3c5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f3c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f3c5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f3c5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f3c5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f3c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f3c5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-115">Not supported.</span></span>    |
|<span data-ttu-id="3f3c5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f3c5-116">Application</span></span> | <span data-ttu-id="3f3c5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f3c5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f3c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="3f3c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f3c5-119">Request headers</span></span>

| <span data-ttu-id="3f3c5-120">名前</span><span class="sxs-lookup"><span data-stu-id="3f3c5-120">Name</span></span>       | <span data-ttu-id="3f3c5-121">説明</span><span class="sxs-lookup"><span data-stu-id="3f3c5-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3f3c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f3c5-122">Authorization</span></span>  | <span data-ttu-id="3f3c5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f3c5-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="3f3c5-125">If-Match</span></span>  | <span data-ttu-id="3f3c5-p104">更新する plannerPlan の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p104">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f3c5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f3c5-128">Request body</span></span>
<span data-ttu-id="3f3c5-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3f3c5-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f3c5-132">Property</span></span>     | <span data-ttu-id="3f3c5-133">型</span><span class="sxs-lookup"><span data-stu-id="3f3c5-133">Type</span></span>   |<span data-ttu-id="3f3c5-134">説明</span><span class="sxs-lookup"><span data-stu-id="3f3c5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f3c5-135">owner</span><span class="sxs-lookup"><span data-stu-id="3f3c5-135">owner</span></span>|<span data-ttu-id="3f3c5-136">String</span><span class="sxs-lookup"><span data-stu-id="3f3c5-136">String</span></span>|<span data-ttu-id="3f3c5-p106">計画を所有する [グループ](../resources/group.md) `id`。このフィールドを設定するためには、有効なグループが存在していなければなりません。一度設定したら、所有者のみが更新できます。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p106">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="3f3c5-140">タイトル</span><span class="sxs-lookup"><span data-stu-id="3f3c5-140">title</span></span>|<span data-ttu-id="3f3c5-141">String</span><span class="sxs-lookup"><span data-stu-id="3f3c5-141">String</span></span>|<span data-ttu-id="3f3c5-142">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-142">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="3f3c5-143">応答</span><span class="sxs-lookup"><span data-stu-id="3f3c5-143">Response</span></span>

<span data-ttu-id="3f3c5-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-144">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="3f3c5-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3f3c5-148">例</span><span class="sxs-lookup"><span data-stu-id="3f3c5-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f3c5-149">要求</span><span class="sxs-lookup"><span data-stu-id="3f3c5-149">Request</span></span>
<span data-ttu-id="3f3c5-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="3f3c5-151">応答</span><span class="sxs-lookup"><span data-stu-id="3f3c5-151">Response</span></span>
<span data-ttu-id="3f3c5-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f3c5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->