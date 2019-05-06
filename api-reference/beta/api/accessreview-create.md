---
title: AccessReview を作成する
description: Azure AD access レビュー機能で、新しい accessReview オブジェクトを作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8a462398903a821bba1022cde07f45f99817356c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586462"
---
# <a name="create-accessreview"></a><span data-ttu-id="c09ba-103">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="c09ba-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c09ba-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[accessreview](../resources/accessreview.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c09ba-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c09ba-105">この要求を行う前に、発信者は以前に[ビジネスフローテンプレートの一覧を取得](businessflowtemplate-list.md)して、の`businessFlowTemplateId`値を要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="c09ba-106">この要求を行った後、呼び出し元は、プログラムにアクセスレビューをリンクするために[programControl を作成](programcontrol-create.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c09ba-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c09ba-107">Permissions</span></span>
<span data-ttu-id="c09ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c09ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c09ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c09ba-110">Permission type</span></span>                        | <span data-ttu-id="c09ba-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c09ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c09ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c09ba-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c09ba-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c09ba-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c09ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c09ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c09ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c09ba-115">Not supported.</span></span> |
|<span data-ttu-id="c09ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c09ba-116">Application</span></span>                            | <span data-ttu-id="c09ba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c09ba-117">Not supported.</span></span> |

<span data-ttu-id="c09ba-118">また、呼び出し元は、アクセスレビューを作成した後、プログラムの[制御](../resources/programcontrol.md)を作成できるようにするために、プログラムによる制御が必要になります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-118">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="c09ba-119">さらに、サインインしているユーザーも、アクセスレビューを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-119">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="c09ba-120">詳細については、「[アクセスレビュー](../resources/accessreviews-root.md)の役割とアクセス許可の要件」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c09ba-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="c09ba-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c09ba-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="c09ba-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c09ba-122">Request headers</span></span>
| <span data-ttu-id="c09ba-123">名前</span><span class="sxs-lookup"><span data-stu-id="c09ba-123">Name</span></span>         | <span data-ttu-id="c09ba-124">型</span><span class="sxs-lookup"><span data-stu-id="c09ba-124">Type</span></span>        | <span data-ttu-id="c09ba-125">説明</span><span class="sxs-lookup"><span data-stu-id="c09ba-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c09ba-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c09ba-126">Authorization</span></span> | <span data-ttu-id="c09ba-127">string</span><span class="sxs-lookup"><span data-stu-id="c09ba-127">string</span></span> | <span data-ttu-id="c09ba-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="c09ba-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c09ba-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="c09ba-130">Request body</span></span>
<span data-ttu-id="c09ba-131">要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c09ba-131">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c09ba-132">次の表に、accessReview の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c09ba-132">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="c09ba-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c09ba-133">Property</span></span>     | <span data-ttu-id="c09ba-134">型</span><span class="sxs-lookup"><span data-stu-id="c09ba-134">Type</span></span>        | <span data-ttu-id="c09ba-135">説明</span><span class="sxs-lookup"><span data-stu-id="c09ba-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c09ba-136">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="c09ba-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c09ba-137">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="c09ba-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c09ba-138">これは、将来の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c09ba-139">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="c09ba-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c09ba-140">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c09ba-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c09ba-141">レビュー担当者に表示する説明。</span><span class="sxs-lookup"><span data-stu-id="c09ba-141">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="c09ba-142">[Businessflowtemplate](../resources/businessflowtemplate.md)から取得したビジネスフローテンプレートの識別子。</span><span class="sxs-lookup"><span data-stu-id="c09ba-142">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="c09ba-143">レビュー対象のオブジェクトのアクセス権に対するレビュー担当者の関係の種類`self`、 `delegated`いずれか`entityOwners`、または。</span><span class="sxs-lookup"><span data-stu-id="c09ba-143">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="c09ba-144">アクセスレビューが作成されるオブジェクト (グループのメンバーシップ、アプリケーションに対するユーザーの割り当てなど)。</span><span class="sxs-lookup"><span data-stu-id="c09ba-144">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="c09ba-145">指定した reviewerType に値`delegated`がある場合は、レビュー担当者にも`reviewers`プロパティが含まれている必要があります。これには、レビューアーの[useridentity](../resources/useridentity.md)のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c09ba-145">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="c09ba-146">アプリが、サインインしているユーザーなしでこの API を呼び出している場合は、発信者にも**createdBy**プロパティが含まれている必要があります。この値は、レビューの作成者として識別されるユーザーの[useridentity](../resources/useridentity.md)です。</span><span class="sxs-lookup"><span data-stu-id="c09ba-146">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="c09ba-147">また、呼び出し元には、定期的なレビューのシリーズを作成したり、既定のレビュー動作から変更したりするための設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c09ba-147">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="c09ba-148">特に、定期的なレビューを作成するには、呼び出し元`accessReviewRecurrenceSettings`に、アクセスレビュー設定内にを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="c09ba-148">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="c09ba-149">応答</span><span class="sxs-lookup"><span data-stu-id="c09ba-149">Response</span></span>
<span data-ttu-id="c09ba-150">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c09ba-150">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c09ba-151">例</span><span class="sxs-lookup"><span data-stu-id="c09ba-151">Example</span></span>

<span data-ttu-id="c09ba-152">これは、1回限り (繰り返しではない) アクセスレビューを作成し、2人のユーザーをレビュー担当者として明示的に指定する例です。</span><span class="sxs-lookup"><span data-stu-id="c09ba-152">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="c09ba-153">要求</span><span class="sxs-lookup"><span data-stu-id="c09ba-153">Request</span></span>
<span data-ttu-id="c09ba-154">要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c09ba-154">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```

##### <a name="response"></a><span data-ttu-id="c09ba-155">応答</span><span class="sxs-lookup"><span data-stu-id="c09ba-155">Response</span></span>
><span data-ttu-id="c09ba-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c09ba-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c09ba-158">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c09ba-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c09ba-159">Visual</span><span class="sxs-lookup"><span data-stu-id="c09ba-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_accessReview_from_accessReviews-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c09ba-160">Java</span><span class="sxs-lookup"><span data-stu-id="c09ba-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_accessReview_from_accessReviews-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
