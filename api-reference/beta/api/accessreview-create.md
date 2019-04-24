---
title: accessreview を作成する
description: Azure AD access レビュー機能で、新しい accessreview オブジェクトを作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 669b11a8f3b52e867d6b3e803c9419968924928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456823"
---
# <a name="create-accessreview"></a><span data-ttu-id="739f7-103">accessreview を作成する</span><span class="sxs-lookup"><span data-stu-id="739f7-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="739f7-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[accessreview](../resources/accessreview.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="739f7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="739f7-105">この要求を行う前に、発信者は以前に[ビジネスフローテンプレートの一覧を取得](businessflowtemplate-list.md)して、の`businessFlowTemplateId`値を要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="739f7-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="739f7-106">この要求を行った後、呼び出し元は、プログラムにアクセスレビューをリンクするために[programcontrol を作成](programcontrol-create.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="739f7-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="739f7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="739f7-107">Permissions</span></span>
<span data-ttu-id="739f7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="739f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="739f7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="739f7-110">Permission type</span></span>                        | <span data-ttu-id="739f7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="739f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="739f7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="739f7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="739f7-113">programcontrol を使用して、次の方法でプログラムを完全に実行することにより、プログラムを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="739f7-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="739f7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="739f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="739f7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="739f7-115">Not supported.</span></span> |
|<span data-ttu-id="739f7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="739f7-116">Application</span></span>                            | <span data-ttu-id="739f7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="739f7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="739f7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="739f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="739f7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="739f7-119">Request headers</span></span>
| <span data-ttu-id="739f7-120">名前</span><span class="sxs-lookup"><span data-stu-id="739f7-120">Name</span></span>         | <span data-ttu-id="739f7-121">型</span><span class="sxs-lookup"><span data-stu-id="739f7-121">Type</span></span>        | <span data-ttu-id="739f7-122">説明</span><span class="sxs-lookup"><span data-stu-id="739f7-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="739f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="739f7-123">Authorization</span></span> | <span data-ttu-id="739f7-124">string</span><span class="sxs-lookup"><span data-stu-id="739f7-124">string</span></span> | <span data-ttu-id="739f7-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="739f7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="739f7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="739f7-127">Request body</span></span>
<span data-ttu-id="739f7-128">要求本文で、 [accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="739f7-128">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="739f7-129">次の表に、accessreview の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="739f7-129">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="739f7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="739f7-130">Property</span></span>     | <span data-ttu-id="739f7-131">型</span><span class="sxs-lookup"><span data-stu-id="739f7-131">Type</span></span>        | <span data-ttu-id="739f7-132">説明</span><span class="sxs-lookup"><span data-stu-id="739f7-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="739f7-133">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="739f7-133">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="739f7-134">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="739f7-134">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="739f7-135">これは、将来の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="739f7-135">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="739f7-136">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="739f7-136">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="739f7-137">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="739f7-137">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="739f7-138">レビュー担当者に表示する説明。</span><span class="sxs-lookup"><span data-stu-id="739f7-138">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="739f7-139">[businessflowtemplate](../resources/businessflowtemplate.md)から取得したビジネスフローテンプレートの識別子。</span><span class="sxs-lookup"><span data-stu-id="739f7-139">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="739f7-140">レビュー対象のオブジェクトのアクセス権に対するレビュー担当者の関係の種類`self`、 `delegated`いずれか`entityOwners`、または。</span><span class="sxs-lookup"><span data-stu-id="739f7-140">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="739f7-141">アクセスレビューが作成されるオブジェクト (グループのメンバーシップ、アプリケーションに対するユーザーの割り当てなど)。</span><span class="sxs-lookup"><span data-stu-id="739f7-141">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="739f7-142">指定した reviewerType に値`delegated`がある場合は、レビュー担当者にも`reviewers`プロパティが含まれている必要があります。これには、レビューアーの[useridentity](../resources/useridentity.md)のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="739f7-142">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="739f7-143">また、呼び出し元には、定期的なレビューのシリーズを作成したり、既定のレビュー動作から変更したりするための設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="739f7-143">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="739f7-144">特に、定期的なレビューを作成するには、呼び出し元`accessReviewRecurrenceSettings`に、アクセスレビュー設定内にを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="739f7-144">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="739f7-145">応答</span><span class="sxs-lookup"><span data-stu-id="739f7-145">Response</span></span>
<span data-ttu-id="739f7-146">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="739f7-146">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="739f7-147">例</span><span class="sxs-lookup"><span data-stu-id="739f7-147">Example</span></span>

<span data-ttu-id="739f7-148">これは、1回限り (繰り返しではない) アクセスレビューを作成し、2人のユーザーをレビュー担当者として明示的に指定する例です。</span><span class="sxs-lookup"><span data-stu-id="739f7-148">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="739f7-149">要求</span><span class="sxs-lookup"><span data-stu-id="739f7-149">Request</span></span>
<span data-ttu-id="739f7-150">要求本文で、 [accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="739f7-150">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="739f7-151">応答</span><span class="sxs-lookup"><span data-stu-id="739f7-151">Response</span></span>
><span data-ttu-id="739f7-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="739f7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
