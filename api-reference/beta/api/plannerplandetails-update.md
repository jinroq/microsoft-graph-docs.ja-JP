---
title: Update plannerplandetails
description: '**plannerplandetails** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd42196238fb103021debf8a4fee2f658053a255
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950138"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="92ada-103">Update plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="92ada-103">Update plannerplandetails</span></span>

> <span data-ttu-id="92ada-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92ada-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92ada-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92ada-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92ada-106">**plannerplandetails** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="92ada-106">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="92ada-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92ada-107">Permissions</span></span>
<span data-ttu-id="92ada-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92ada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ada-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92ada-110">Permission type</span></span>      | <span data-ttu-id="92ada-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92ada-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ada-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92ada-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92ada-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ada-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92ada-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92ada-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ada-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92ada-115">Not supported.</span></span>    |
|<span data-ttu-id="92ada-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92ada-116">Application</span></span> | <span data-ttu-id="92ada-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92ada-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92ada-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92ada-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="92ada-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92ada-119">Optional request headers</span></span>
| <span data-ttu-id="92ada-120">名前</span><span class="sxs-lookup"><span data-stu-id="92ada-120">Name</span></span>       | <span data-ttu-id="92ada-121">説明</span><span class="sxs-lookup"><span data-stu-id="92ada-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="92ada-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ada-122">Authorization</span></span>  | <span data-ttu-id="92ada-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="92ada-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92ada-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="92ada-125">If-Match</span></span>  | <span data-ttu-id="92ada-p104">更新する plannerPlanDetails の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="92ada-p104">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ada-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="92ada-128">Request body</span></span>
<span data-ttu-id="92ada-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="92ada-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="92ada-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92ada-132">Property</span></span>     | <span data-ttu-id="92ada-133">種類</span><span class="sxs-lookup"><span data-stu-id="92ada-133">Type</span></span>   |<span data-ttu-id="92ada-134">説明</span><span class="sxs-lookup"><span data-stu-id="92ada-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92ada-135">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="92ada-135">categoryDescriptions</span></span>|[<span data-ttu-id="92ada-136">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="92ada-136">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="92ada-137">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="92ada-137">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="92ada-138">sharedWith</span><span class="sxs-lookup"><span data-stu-id="92ada-138">sharedWith</span></span>|[<span data-ttu-id="92ada-139">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="92ada-139">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="92ada-p106">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](../resources/group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="92ada-p106">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="92ada-143">応答</span><span class="sxs-lookup"><span data-stu-id="92ada-143">Response</span></span>

<span data-ttu-id="92ada-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerPlanDetails](../resources/plannerplandetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="92ada-144">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="92ada-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92ada-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="92ada-148">例</span><span class="sxs-lookup"><span data-stu-id="92ada-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92ada-149">要求</span><span class="sxs-lookup"><span data-stu-id="92ada-149">Request</span></span>
<span data-ttu-id="92ada-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92ada-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="92ada-151">応答</span><span class="sxs-lookup"><span data-stu-id="92ada-151">Response</span></span>
<span data-ttu-id="92ada-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92ada-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
