---
title: AccessReview を更新する
description: Azure AD access レビュー機能で、既存の accessReview オブジェクトを更新して、そのプロパティの1つ以上を変更します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e290d7343fb7c5c34ce4952a97796dc94d080ae
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855908"
---
# <a name="update-accessreview"></a><span data-ttu-id="bfd4b-103">AccessReview を更新する</span><span class="sxs-lookup"><span data-stu-id="bfd4b-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfd4b-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、そのプロパティの1つ以上を変更します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="bfd4b-105">この API は、レビュー担当者またはレビューの決定を変更するためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="bfd4b-106">レビュー担当者を変更するには、 [Addreviewer](accessreview-addreviewer.md)または[removereviewer](accessreview-removereviewer.md) api を使用します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="bfd4b-107">既に開始した1回限りのレビュー、または定期的なレビューの事前に開始されているインスタンスを停止するには、 [stop](accessreview-stop.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="bfd4b-108">目的のグループまたはアプリのアクセス権に決定を適用するには、[API の[適用](accessreview-apply.md)] を使用します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="bfd4b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bfd4b-109">Permissions</span></span>
<span data-ttu-id="bfd4b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfd4b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bfd4b-112">Permission type</span></span>                        | <span data-ttu-id="bfd4b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bfd4b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfd4b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bfd4b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfd4b-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfd4b-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="bfd4b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bfd4b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfd4b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-117">Not supported.</span></span> |
|<span data-ttu-id="bfd4b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bfd4b-118">Application</span></span>                            | <span data-ttu-id="bfd4b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfd4b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bfd4b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="bfd4b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfd4b-121">Request headers</span></span>
| <span data-ttu-id="bfd4b-122">名前</span><span class="sxs-lookup"><span data-stu-id="bfd4b-122">Name</span></span>         | <span data-ttu-id="bfd4b-123">型</span><span class="sxs-lookup"><span data-stu-id="bfd4b-123">Type</span></span>        | <span data-ttu-id="bfd4b-124">説明</span><span class="sxs-lookup"><span data-stu-id="bfd4b-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bfd4b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfd4b-125">Authorization</span></span> | <span data-ttu-id="bfd4b-126">string</span><span class="sxs-lookup"><span data-stu-id="bfd4b-126">string</span></span> | <span data-ttu-id="bfd4b-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfd4b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bfd4b-129">Request body</span></span>
<span data-ttu-id="bfd4b-130">要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="bfd4b-131">次の表に、accessReview の更新時に提供できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="bfd4b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfd4b-132">Property</span></span>     | <span data-ttu-id="bfd4b-133">型</span><span class="sxs-lookup"><span data-stu-id="bfd4b-133">Type</span></span>        | <span data-ttu-id="bfd4b-134">説明</span><span class="sxs-lookup"><span data-stu-id="bfd4b-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="bfd4b-135">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="bfd4b-136">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="bfd4b-137">これは、将来の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="bfd4b-138">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="bfd4b-139">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="bfd4b-140">レビュー担当者に表示する説明。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="bfd4b-141">応答</span><span class="sxs-lookup"><span data-stu-id="bfd4b-141">Response</span></span>
<span data-ttu-id="bfd4b-142">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfd4b-143">例</span><span class="sxs-lookup"><span data-stu-id="bfd4b-143">Example</span></span>

<span data-ttu-id="bfd4b-144">これは、1回限り (定期的でない) アクセスレビューを更新する例です。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="bfd4b-145">要求</span><span class="sxs-lookup"><span data-stu-id="bfd4b-145">Request</span></span>
<span data-ttu-id="bfd4b-146">要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bfd4b-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bfd4b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bfd4b-148">C#</span><span class="sxs-lookup"><span data-stu-id="bfd4b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfd4b-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfd4b-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfd4b-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="bfd4b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bfd4b-151">Java</span><span class="sxs-lookup"><span data-stu-id="bfd4b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bfd4b-152">応答</span><span class="sxs-lookup"><span data-stu-id="bfd4b-152">Response</span></span>
><span data-ttu-id="bfd4b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bfd4b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
