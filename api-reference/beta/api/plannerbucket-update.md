---
title: Update plannerbucket
description: '**plannerbucket** オブジェクトのプロパティを更新します。'
localization_priority: Normal
ms.openlocfilehash: c2a3e0daec852e4c871a42b1bbc88dcc950afa6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836044"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="f2484-103">Update plannerbucket</span><span class="sxs-lookup"><span data-stu-id="f2484-103">Update plannerbucket</span></span>

> <span data-ttu-id="f2484-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2484-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2484-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2484-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2484-106">**plannerbucket** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2484-106">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2484-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2484-107">Permissions</span></span>
<span data-ttu-id="f2484-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2484-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2484-110">Permission type</span></span>      | <span data-ttu-id="f2484-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2484-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2484-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2484-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2484-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2484-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2484-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2484-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2484-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2484-115">Not supported.</span></span>    |
|<span data-ttu-id="f2484-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2484-116">Application</span></span> | <span data-ttu-id="f2484-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2484-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2484-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2484-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="f2484-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2484-119">Optional request headers</span></span>
| <span data-ttu-id="f2484-120">名前</span><span class="sxs-lookup"><span data-stu-id="f2484-120">Name</span></span>       | <span data-ttu-id="f2484-121">説明</span><span class="sxs-lookup"><span data-stu-id="f2484-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2484-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2484-122">Authorization</span></span>  | <span data-ttu-id="f2484-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2484-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2484-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="f2484-125">If-Match</span></span>  | <span data-ttu-id="f2484-p104">更新する **plannerBucket** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="f2484-p104">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2484-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2484-128">Request body</span></span>
<span data-ttu-id="f2484-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f2484-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2484-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2484-132">Property</span></span>     | <span data-ttu-id="f2484-133">種類</span><span class="sxs-lookup"><span data-stu-id="f2484-133">Type</span></span>   |<span data-ttu-id="f2484-134">説明</span><span class="sxs-lookup"><span data-stu-id="f2484-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2484-135">名前</span><span class="sxs-lookup"><span data-stu-id="f2484-135">name</span></span>|<span data-ttu-id="f2484-136">String</span><span class="sxs-lookup"><span data-stu-id="f2484-136">String</span></span>|<span data-ttu-id="f2484-137">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="f2484-137">Name of the bucket.</span></span>|
|<span data-ttu-id="f2484-138">orderHint</span><span class="sxs-lookup"><span data-stu-id="f2484-138">orderHint</span></span>|<span data-ttu-id="f2484-139">String</span><span class="sxs-lookup"><span data-stu-id="f2484-139">String</span></span>|<span data-ttu-id="f2484-p106">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](../resources/planner-order-hint-format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="f2484-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f2484-142">planId</span><span class="sxs-lookup"><span data-stu-id="f2484-142">planId</span></span>|<span data-ttu-id="f2484-143">String</span><span class="sxs-lookup"><span data-stu-id="f2484-143">String</span></span>|<span data-ttu-id="f2484-144">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="f2484-144">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="f2484-145">応答</span><span class="sxs-lookup"><span data-stu-id="f2484-145">Response</span></span>

<span data-ttu-id="f2484-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerBucket](../resources/plannerbucket.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2484-146">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="f2484-p107">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2484-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f2484-150">例</span><span class="sxs-lookup"><span data-stu-id="f2484-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2484-151">要求</span><span class="sxs-lookup"><span data-stu-id="f2484-151">Request</span></span>
<span data-ttu-id="f2484-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2484-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="f2484-153">応答</span><span class="sxs-lookup"><span data-stu-id="f2484-153">Response</span></span>
<span data-ttu-id="f2484-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2484-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
