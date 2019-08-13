---
title: Update plannerplandetails
description: '**plannerplandetails** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a4a4bf9aeb26b3e9a0108260c0d83f8eca7e0cfe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361549"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="f0245-103">Update plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="f0245-103">Update plannerplandetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0245-104">**plannerplandetails** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0245-104">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0245-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0245-105">Permissions</span></span>
<span data-ttu-id="f0245-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0245-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0245-108">Permission type</span></span>      | <span data-ttu-id="f0245-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0245-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0245-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0245-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0245-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0245-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0245-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0245-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0245-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0245-113">Not supported.</span></span>    |
|<span data-ttu-id="f0245-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0245-114">Application</span></span> | <span data-ttu-id="f0245-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0245-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0245-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0245-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="f0245-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0245-117">Optional request headers</span></span>
| <span data-ttu-id="f0245-118">名前</span><span class="sxs-lookup"><span data-stu-id="f0245-118">Name</span></span>       | <span data-ttu-id="f0245-119">説明</span><span class="sxs-lookup"><span data-stu-id="f0245-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f0245-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0245-120">Authorization</span></span>  | <span data-ttu-id="f0245-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0245-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0245-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="f0245-123">If-Match</span></span>  | <span data-ttu-id="f0245-p103">更新する plannerPlanDetails の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="f0245-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0245-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0245-126">Request body</span></span>
<span data-ttu-id="f0245-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f0245-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0245-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0245-130">Property</span></span>     | <span data-ttu-id="f0245-131">型</span><span class="sxs-lookup"><span data-stu-id="f0245-131">Type</span></span>   |<span data-ttu-id="f0245-132">説明</span><span class="sxs-lookup"><span data-stu-id="f0245-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0245-133">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="f0245-133">categoryDescriptions</span></span>|[<span data-ttu-id="f0245-134">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="f0245-134">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="f0245-135">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="f0245-135">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="f0245-136">sharedWith</span><span class="sxs-lookup"><span data-stu-id="f0245-136">sharedWith</span></span>|[<span data-ttu-id="f0245-137">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="f0245-137">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="f0245-p105">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](../resources/group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="f0245-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="f0245-141">応答</span><span class="sxs-lookup"><span data-stu-id="f0245-141">Response</span></span>

<span data-ttu-id="f0245-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerPlanDetails](../resources/plannerplandetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0245-142">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="f0245-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0245-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f0245-146">例</span><span class="sxs-lookup"><span data-stu-id="f0245-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0245-147">要求</span><span class="sxs-lookup"><span data-stu-id="f0245-147">Request</span></span>
<span data-ttu-id="f0245-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0245-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0245-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f0245-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0245-150">C#</span><span class="sxs-lookup"><span data-stu-id="f0245-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0245-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0245-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0245-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="f0245-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f0245-153">Java</span><span class="sxs-lookup"><span data-stu-id="f0245-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0245-154">応答</span><span class="sxs-lookup"><span data-stu-id="f0245-154">Response</span></span>
<span data-ttu-id="f0245-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0245-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
