---
title: PlannerUser を更新します。
description: PlannerUser オブジェクトのプロパティを更新します。 追加またはユーザーのお気に入りのプランの一覧からプランを削除するこの操作を使用することができ、ユーザーを計画することを示すには、最近表示しました。
localization_priority: Normal
ms.openlocfilehash: ae09deff65c5de08d80e34140abacd43d43a94b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889055"
---
# <a name="update-planneruser"></a><span data-ttu-id="af143-104">PlannerUser を更新します。</span><span class="sxs-lookup"><span data-stu-id="af143-104">Update plannerUser</span></span>

> <span data-ttu-id="af143-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af143-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af143-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af143-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af143-107">[PlannerUser](../resources/planneruser.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="af143-107">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="af143-108">追加またはユーザーのお気に入りのプランの一覧からプランを削除するこの操作を使用することができ、ユーザーを計画することを示すには、最近表示しました。</span><span class="sxs-lookup"><span data-stu-id="af143-108">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="af143-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af143-109">Permissions</span></span>
<span data-ttu-id="af143-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af143-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af143-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af143-112">Permission type</span></span>      | <span data-ttu-id="af143-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af143-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af143-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af143-114">Delegated (work or school account)</span></span> | <span data-ttu-id="af143-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af143-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af143-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af143-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af143-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af143-117">Not supported.</span></span>    |
|<span data-ttu-id="af143-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af143-118">Application</span></span> | <span data-ttu-id="af143-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af143-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af143-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af143-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="af143-121">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af143-121">Optional request headers</span></span>
| <span data-ttu-id="af143-122">名前</span><span class="sxs-lookup"><span data-stu-id="af143-122">Name</span></span>       | <span data-ttu-id="af143-123">説明</span><span class="sxs-lookup"><span data-stu-id="af143-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="af143-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="af143-124">Authorization</span></span>  | <span data-ttu-id="af143-p105">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="af143-p105">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="af143-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="af143-127">If-Match</span></span>  | <span data-ttu-id="af143-128">最後の既知の ETag 値を更新する**plannerUser**のです。</span><span class="sxs-lookup"><span data-stu-id="af143-128">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="af143-129">必須。</span><span class="sxs-lookup"><span data-stu-id="af143-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af143-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="af143-130">Request body</span></span>
<span data-ttu-id="af143-131">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="af143-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="af143-132">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="af143-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="af143-133">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="af143-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="af143-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af143-134">Property</span></span>     | <span data-ttu-id="af143-135">種類</span><span class="sxs-lookup"><span data-stu-id="af143-135">Type</span></span>   |<span data-ttu-id="af143-136">説明</span><span class="sxs-lookup"><span data-stu-id="af143-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af143-137">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="af143-137">favoritePlanReferences</span></span>|[<span data-ttu-id="af143-138">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="af143-138">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="af143-139">ユーザーは、お気に入りとしてマークする計画への参照が含まれているコレクションに変更します。</span><span class="sxs-lookup"><span data-stu-id="af143-139">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="af143-140">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="af143-140">recentPlanReferences</span></span>|[<span data-ttu-id="af143-141">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="af143-141">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="af143-142">ユーザーが最近閲覧した計画への参照を含むコレクションを変更します。</span><span class="sxs-lookup"><span data-stu-id="af143-142">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="af143-143">応答</span><span class="sxs-lookup"><span data-stu-id="af143-143">Response</span></span>
<span data-ttu-id="af143-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[plannerUser](../resources/planneruser.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="af143-144">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="af143-p108">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af143-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="af143-148">例</span><span class="sxs-lookup"><span data-stu-id="af143-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af143-149">要求</span><span class="sxs-lookup"><span data-stu-id="af143-149">Request</span></span>
<span data-ttu-id="af143-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="af143-150">The following is an example of the request.</span></span> <span data-ttu-id="af143-151">この要求では、ユーザーのために ID「jd8S5gOaFk2S8aWCIAJz42QAAxtD」と「次のリリースの説明」プランを追加し、お気に入りプラン一覧から ID が"L7RmQAGX2q-7oTB5aMIAE2rVo-1N"計画を削除します。</span><span class="sxs-lookup"><span data-stu-id="af143-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="af143-152">計画"jd8S5gOaFk2S8aWCIAJz42QAAxtD"の最後の表示時間も更新されます。</span><span class="sxs-lookup"><span data-stu-id="af143-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a><span data-ttu-id="af143-153">応答</span><span class="sxs-lookup"><span data-stu-id="af143-153">Response</span></span>
<span data-ttu-id="af143-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="af143-154">The following is an example of the response.</span></span> 

><span data-ttu-id="af143-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="af143-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
