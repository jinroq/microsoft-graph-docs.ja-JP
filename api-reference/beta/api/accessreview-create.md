---
title: AccessReview を作成します。
description: Azure AD のレビュー機能にアクセス、新しい accessReview オブジェクトを作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 669b11a8f3b52e867d6b3e803c9419968924928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517800"
---
# <a name="create-accessreview"></a><span data-ttu-id="12542-103">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="12542-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12542-104">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[accessReview](../resources/accessreview.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="12542-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="12542-105">この要求を行う前に呼び出し元には以前[業務フローのテンプレートの一覧を取得](businessflowtemplate-list.md)するにはの値を設定する`businessFlowTemplateId`要求に含める。</span><span class="sxs-lookup"><span data-stu-id="12542-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="12542-106">呼び出し元では、この要求を行った後[、デバッギングを作成](programcontrol-create.md)、アクセス確認をプログラムにリンクする必要があります。</span><span class="sxs-lookup"><span data-stu-id="12542-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="12542-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12542-107">Permissions</span></span>
<span data-ttu-id="12542-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12542-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12542-110">Permission type</span></span>                        | <span data-ttu-id="12542-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12542-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="12542-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12542-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="12542-113">AccessReview.ReadWrite.All、デバッギングを作成する後続の呼び出しで完全なシナリオを ProgramControl.ReadWrite.All する必要があり、</span><span class="sxs-lookup"><span data-stu-id="12542-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="12542-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12542-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12542-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12542-115">Not supported.</span></span> |
|<span data-ttu-id="12542-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12542-116">Application</span></span>                            | <span data-ttu-id="12542-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12542-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12542-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12542-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="12542-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12542-119">Request headers</span></span>
| <span data-ttu-id="12542-120">名前</span><span class="sxs-lookup"><span data-stu-id="12542-120">Name</span></span>         | <span data-ttu-id="12542-121">型</span><span class="sxs-lookup"><span data-stu-id="12542-121">Type</span></span>        | <span data-ttu-id="12542-122">説明</span><span class="sxs-lookup"><span data-stu-id="12542-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="12542-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12542-123">Authorization</span></span> | <span data-ttu-id="12542-124">string</span><span class="sxs-lookup"><span data-stu-id="12542-124">string</span></span> | <span data-ttu-id="12542-125">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="12542-125">Bearer \{token\}.</span></span> <span data-ttu-id="12542-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="12542-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12542-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="12542-127">Request body</span></span>
<span data-ttu-id="12542-128">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="12542-128">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="12542-129">次の表は、accessReview を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12542-129">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="12542-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12542-130">Property</span></span>     | <span data-ttu-id="12542-131">型</span><span class="sxs-lookup"><span data-stu-id="12542-131">Type</span></span>        | <span data-ttu-id="12542-132">説明</span><span class="sxs-lookup"><span data-stu-id="12542-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="12542-133">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="12542-133">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="12542-134">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="12542-134">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="12542-135">将来の日付でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="12542-135">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="12542-136">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="12542-136">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="12542-137">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="12542-137">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="12542-138">校閲者を表示する説明します。</span><span class="sxs-lookup"><span data-stu-id="12542-138">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="12542-139">ビジネス フロー テンプレート識別子の[businessFlowTemplate](../resources/businessflowtemplate.md)から取得します。</span><span class="sxs-lookup"><span data-stu-id="12542-139">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="12542-140">リレーションシップの種類のいずれかの確認済みのオブジェクトのアクセス許可の校閲者の`self`、 `delegated`、または`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="12542-140">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="12542-141">アクセス確認を作成するため、グループのメンバーシップなどのユーザーがアプリケーションの割り当てオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="12542-141">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="12542-142">指定された reviewerType に値が設定されている場合`delegated`、呼び出し元は含める必要がありますし、`reviewers`プロパティは、一連の校閲者に[割り当てられていません](../resources/useridentity.md)。</span><span class="sxs-lookup"><span data-stu-id="12542-142">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="12542-143">さらに、呼び出し元は、一連の定期的なレビューを作成するか、既定の確認動作を変更する設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="12542-143">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="12542-144">具体的には、定期的なレビューを作成するには、呼び出し元する必要があります、 `accessReviewRecurrenceSettings` 、access 内で設定を確認します</span><span class="sxs-lookup"><span data-stu-id="12542-144">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="12542-145">応答</span><span class="sxs-lookup"><span data-stu-id="12542-145">Response</span></span>
<span data-ttu-id="12542-146">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="12542-146">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12542-147">例</span><span class="sxs-lookup"><span data-stu-id="12542-147">Example</span></span>

<span data-ttu-id="12542-148">これは、校閲者として、2 人のユーザーを明示的に指定する 1 回限り (定期ではない) アクセス確認を作成する例です。</span><span class="sxs-lookup"><span data-stu-id="12542-148">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="12542-149">要求</span><span class="sxs-lookup"><span data-stu-id="12542-149">Request</span></span>
<span data-ttu-id="12542-150">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="12542-150">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="12542-151">応答</span><span class="sxs-lookup"><span data-stu-id="12542-151">Response</span></span>
><span data-ttu-id="12542-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="12542-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
