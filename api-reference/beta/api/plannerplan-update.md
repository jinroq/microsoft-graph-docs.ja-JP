---
title: プランを更新する plan
description: '**plan**オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 86f486ceb5b2adca66049e5370dc0b6fa5c670ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538939"
---
# <a name="update-plannerplan"></a><span data-ttu-id="0b2b8-103">プランを更新する plan</span><span class="sxs-lookup"><span data-stu-id="0b2b8-103">Update plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b2b8-104">**plan**オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b2b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b2b8-105">Permissions</span></span>
<span data-ttu-id="0b2b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b2b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b2b8-108">Permission type</span></span>      | <span data-ttu-id="0b2b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b2b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b2b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b2b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b2b8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b2b8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b2b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b2b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b2b8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-113">Not supported.</span></span>    |
|<span data-ttu-id="0b2b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b2b8-114">Application</span></span> | <span data-ttu-id="0b2b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b2b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b2b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="0b2b8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b2b8-117">Request headers</span></span>

| <span data-ttu-id="0b2b8-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b2b8-118">Name</span></span>       | <span data-ttu-id="0b2b8-119">説明</span><span class="sxs-lookup"><span data-stu-id="0b2b8-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b2b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b2b8-120">Authorization</span></span>  | <span data-ttu-id="0b2b8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b2b8-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="0b2b8-123">If-Match</span></span>  | <span data-ttu-id="0b2b8-p103">更新する plannerPlan の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b2b8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b2b8-126">Request body</span></span>
<span data-ttu-id="0b2b8-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b2b8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b2b8-130">Property</span></span>     | <span data-ttu-id="0b2b8-131">型</span><span class="sxs-lookup"><span data-stu-id="0b2b8-131">Type</span></span>   |<span data-ttu-id="0b2b8-132">説明</span><span class="sxs-lookup"><span data-stu-id="0b2b8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b2b8-133">owner</span><span class="sxs-lookup"><span data-stu-id="0b2b8-133">owner</span></span>|<span data-ttu-id="0b2b8-134">String</span><span class="sxs-lookup"><span data-stu-id="0b2b8-134">String</span></span>|<span data-ttu-id="0b2b8-p105">計画を所有する [グループ](../resources/group.md) `id`。このフィールドを設定するためには、有効なグループが存在していなければなりません。一度設定したら、所有者のみが更新できます。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="0b2b8-138">title</span><span class="sxs-lookup"><span data-stu-id="0b2b8-138">title</span></span>|<span data-ttu-id="0b2b8-139">String</span><span class="sxs-lookup"><span data-stu-id="0b2b8-139">String</span></span>|<span data-ttu-id="0b2b8-140">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="0b2b8-141">応答</span><span class="sxs-lookup"><span data-stu-id="0b2b8-141">Response</span></span>

<span data-ttu-id="0b2b8-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="0b2b8-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0b2b8-146">例</span><span class="sxs-lookup"><span data-stu-id="0b2b8-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b2b8-147">要求</span><span class="sxs-lookup"><span data-stu-id="0b2b8-147">Request</span></span>
<span data-ttu-id="0b2b8-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0b2b8-149">応答</span><span class="sxs-lookup"><span data-stu-id="0b2b8-149">Response</span></span>
<span data-ttu-id="0b2b8-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b2b8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerplan-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
