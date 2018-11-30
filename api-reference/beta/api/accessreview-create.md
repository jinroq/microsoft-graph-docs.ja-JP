---
title: AccessReview を作成します。
description: Azure AD のレビュー機能にアクセス、新しい accessReview オブジェクトを作成します。
ms.openlocfilehash: 9d8e8b246c3c43e4f69172ea59715a8718d39d1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067041"
---
# <a name="create-accessreview"></a><span data-ttu-id="c1395-103">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="c1395-103">Create accessReview</span></span>

> <span data-ttu-id="c1395-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1395-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1395-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1395-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1395-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[accessReview](../resources/accessreview.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c1395-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c1395-107">この要求を行う前に呼び出し元には以前[業務フローのテンプレートの一覧を取得](businessflowtemplate-list.md)するにはの値を設定する`businessFlowTemplateId`要求に含める。</span><span class="sxs-lookup"><span data-stu-id="c1395-107">Prior to making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="c1395-108">呼び出し元では、この要求を行った後[、デバッギングを作成](programcontrol-create.md)、アクセス確認をプログラムにリンクする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1395-108">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c1395-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1395-109">Permissions</span></span>
<span data-ttu-id="c1395-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1395-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1395-112">Permission type</span></span>                        | <span data-ttu-id="c1395-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1395-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1395-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1395-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1395-115">AccessReview.ReadWrite.All、デバッギングを作成する後続の呼び出しで完全なシナリオを ProgramControl.ReadWrite.All する必要があり、</span><span class="sxs-lookup"><span data-stu-id="c1395-115">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="c1395-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1395-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1395-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1395-117">Not supported.</span></span> |
|<span data-ttu-id="c1395-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1395-118">Application</span></span>                            | <span data-ttu-id="c1395-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1395-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1395-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1395-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="c1395-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1395-121">Request headers</span></span>
| <span data-ttu-id="c1395-122">名前</span><span class="sxs-lookup"><span data-stu-id="c1395-122">Name</span></span>         | <span data-ttu-id="c1395-123">型</span><span class="sxs-lookup"><span data-stu-id="c1395-123">Type</span></span>        | <span data-ttu-id="c1395-124">説明</span><span class="sxs-lookup"><span data-stu-id="c1395-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c1395-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1395-125">Authorization</span></span> | <span data-ttu-id="c1395-126">string</span><span class="sxs-lookup"><span data-stu-id="c1395-126">string</span></span> | <span data-ttu-id="c1395-127">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="c1395-127">Bearer \{token\}.</span></span> <span data-ttu-id="c1395-128">必須。</span><span class="sxs-lookup"><span data-stu-id="c1395-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1395-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1395-129">Request body</span></span>
<span data-ttu-id="c1395-130">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1395-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c1395-131">次の表は、accessReview を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c1395-131">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="c1395-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1395-132">Property</span></span>     | <span data-ttu-id="c1395-133">型</span><span class="sxs-lookup"><span data-stu-id="c1395-133">Type</span></span>        | <span data-ttu-id="c1395-134">説明</span><span class="sxs-lookup"><span data-stu-id="c1395-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c1395-135">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="c1395-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c1395-136">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="c1395-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c1395-137">将来の日付でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c1395-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c1395-138">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="c1395-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c1395-139">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c1395-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c1395-140">校閲者を表示する説明します。</span><span class="sxs-lookup"><span data-stu-id="c1395-140">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="c1395-141">ビジネス フロー テンプレート識別子の[businessFlowTemplate](../resources/businessflowtemplate.md)から取得します。</span><span class="sxs-lookup"><span data-stu-id="c1395-141">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="c1395-142">リレーションシップの種類のいずれかの確認済みのオブジェクトのアクセス許可の校閲者の`self`、`delegate`または`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="c1395-142">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegate` or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="c1395-143">アクセス確認を作成するため、グループのメンバーシップなどのユーザーがアプリケーションの割り当てオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c1395-143">The object for which an access review is created, such as a memberships of an group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="c1395-144">指定された reviewerType に値が設定されている場合`delegate`、呼び出し元は含める必要がありますし、`reviewers`プロパティは、一連の校閲者に[割り当てられていません](../resources/useridentity.md)。</span><span class="sxs-lookup"><span data-stu-id="c1395-144">If the reviewerType being supplied has the value `delegate`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="c1395-145">さらに、呼び出し元は、一連の定期的なレビューを作成するか、既定の確認動作を変更する設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c1395-145">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="c1395-146">具体的には、定期的なレビューを作成するには、呼び出し元する必要があります、 `accessReviewRecurrenceSettings` 、access 内で設定を確認します</span><span class="sxs-lookup"><span data-stu-id="c1395-146">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="c1395-147">応答</span><span class="sxs-lookup"><span data-stu-id="c1395-147">Response</span></span>
<span data-ttu-id="c1395-148">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c1395-148">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1395-149">使用例</span><span class="sxs-lookup"><span data-stu-id="c1395-149">Example</span></span>

<span data-ttu-id="c1395-150">これは、校閲者として、2 人のユーザーを明示的に指定する 1 回限り (定期ではない) アクセス確認を作成する例です。</span><span class="sxs-lookup"><span data-stu-id="c1395-150">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="c1395-151">要求</span><span class="sxs-lookup"><span data-stu-id="c1395-151">Request</span></span>
<span data-ttu-id="c1395-152">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1395-152">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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
    "reviewerType" : "delegate",
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
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
    }
}
```

##### <a name="response"></a><span data-ttu-id="c1395-153">応答</span><span class="sxs-lookup"><span data-stu-id="c1395-153">Response</span></span>
><span data-ttu-id="c1395-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c1395-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
