---
title: プランのユーザーを更新する
description: プランのユーザーオブジェクトのプロパティを更新します。 この操作を使用して、ユーザーのお気に入りのプランの一覧からプランを追加または削除したり、ユーザーが最近表示したプランを示したりすることができます。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538757"
---
# <a name="update-planneruser"></a><span data-ttu-id="a36db-104">プランのユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="a36db-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a36db-105">[プランのユーザー](../resources/planneruser.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a36db-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="a36db-106">この操作を使用して、ユーザーのお気に入りのプランの一覧からプランを追加または削除したり、ユーザーが最近表示したプランを示したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="a36db-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="a36db-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a36db-107">Permissions</span></span>
<span data-ttu-id="a36db-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a36db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a36db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a36db-110">Permission type</span></span>      | <span data-ttu-id="a36db-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a36db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a36db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a36db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a36db-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a36db-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a36db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a36db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a36db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36db-115">Not supported.</span></span>    |
|<span data-ttu-id="a36db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a36db-116">Application</span></span> | <span data-ttu-id="a36db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a36db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a36db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="a36db-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a36db-119">Optional request headers</span></span>
| <span data-ttu-id="a36db-120">名前</span><span class="sxs-lookup"><span data-stu-id="a36db-120">Name</span></span>       | <span data-ttu-id="a36db-121">説明</span><span class="sxs-lookup"><span data-stu-id="a36db-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a36db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a36db-122">Authorization</span></span>  | <span data-ttu-id="a36db-123">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="a36db-123">Bearer {code}.</span></span> <span data-ttu-id="a36db-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="a36db-124">Required.</span></span>|
| <span data-ttu-id="a36db-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="a36db-125">If-Match</span></span>  | <span data-ttu-id="a36db-126">更新する**プラン**の最後の既知の ETag 値。</span><span class="sxs-lookup"><span data-stu-id="a36db-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="a36db-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="a36db-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a36db-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a36db-128">Request body</span></span>
<span data-ttu-id="a36db-129">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a36db-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a36db-130">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="a36db-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a36db-131">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a36db-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a36db-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a36db-132">Property</span></span>     | <span data-ttu-id="a36db-133">型</span><span class="sxs-lookup"><span data-stu-id="a36db-133">Type</span></span>   |<span data-ttu-id="a36db-134">説明</span><span class="sxs-lookup"><span data-stu-id="a36db-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a36db-135">お気に入りプランの参照</span><span class="sxs-lookup"><span data-stu-id="a36db-135">favoritePlanReferences</span></span>|[<span data-ttu-id="a36db-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="a36db-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="a36db-137">ユーザーがお気に入りとしてマークしたプランへの参照が含まれているコレクションに対する変更。</span><span class="sxs-lookup"><span data-stu-id="a36db-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="a36db-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="a36db-138">recentPlanReferences</span></span>|[<span data-ttu-id="a36db-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="a36db-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="a36db-140">ユーザーが最近表示したプランへの参照が含まれているコレクションに対する変更。</span><span class="sxs-lookup"><span data-stu-id="a36db-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="a36db-141">応答</span><span class="sxs-lookup"><span data-stu-id="a36db-141">Response</span></span>
<span data-ttu-id="a36db-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[プランのユーザー](../resources/planneruser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a36db-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="a36db-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a36db-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="a36db-146">例</span><span class="sxs-lookup"><span data-stu-id="a36db-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a36db-147">要求</span><span class="sxs-lookup"><span data-stu-id="a36db-147">Request</span></span>
<span data-ttu-id="a36db-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a36db-148">The following is an example of the request.</span></span> <span data-ttu-id="a36db-149">この要求は、"jd8S5gOaFk2S8aWCIAJz42QAAxtD" という id を持つプラン "次のリリースディスカッション" をユーザーのお気に入りとして追加し、"7oTB5aMIAE2rVo-1n-L7RmQAGX2q" という id のプランを [お気に入りのプラン] の一覧から削除します。</span><span class="sxs-lookup"><span data-stu-id="a36db-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="a36db-150">また、"jd8S5gOaFk2S8aWCIAJz42QAAxtD" プランの最終ビュー時刻も更新します。</span><span class="sxs-lookup"><span data-stu-id="a36db-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="a36db-151">応答</span><span class="sxs-lookup"><span data-stu-id="a36db-151">Response</span></span>
<span data-ttu-id="a36db-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a36db-152">The following is an example of the response.</span></span> 

><span data-ttu-id="a36db-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a36db-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
