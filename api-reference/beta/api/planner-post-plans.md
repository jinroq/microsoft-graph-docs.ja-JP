---
title: Create plannerPlan
description: この API を使用して、新しい **plannerPlan** を作成します。
ms.openlocfilehash: 685b05cc271aaebfdb198eace416883c52ad28a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072021"
---
# <a name="create-plannerplan"></a><span data-ttu-id="3bc65-103">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3bc65-103">Create plannerPlan</span></span>

> <span data-ttu-id="3bc65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3bc65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bc65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bc65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bc65-106">この API を使用して、新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="3bc65-106">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bc65-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bc65-107">Permissions</span></span>

<span data-ttu-id="3bc65-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bc65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bc65-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bc65-110">Permission type</span></span>                        | <span data-ttu-id="3bc65-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bc65-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3bc65-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bc65-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bc65-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc65-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="3bc65-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bc65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc65-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bc65-115">Not supported.</span></span>                              |
| <span data-ttu-id="3bc65-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bc65-116">Application</span></span>                            | <span data-ttu-id="3bc65-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bc65-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3bc65-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bc65-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="3bc65-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bc65-119">Request headers</span></span>

| <span data-ttu-id="3bc65-120">名前</span><span class="sxs-lookup"><span data-stu-id="3bc65-120">Name</span></span>          | <span data-ttu-id="3bc65-121">説明</span><span class="sxs-lookup"><span data-stu-id="3bc65-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3bc65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bc65-122">Authorization</span></span> | <span data-ttu-id="3bc65-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3bc65-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bc65-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bc65-125">Request body</span></span>

<span data-ttu-id="3bc65-p104">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。**plannerPlan** 所有者プロパティは、[group](../resources/group.md) オブジェクトの ID に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bc65-p104">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="3bc65-128">**注:** 計画を作成しているユーザーは、計画を所有するグループのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bc65-128">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="3bc65-129">[グループの作成](../api/group-post-groups.md)を使用して新しいグループを作成するときにいない追加されますグループにメンバーとして。</span><span class="sxs-lookup"><span data-stu-id="3bc65-129">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="3bc65-130">グループが作成されると、自分自身を追加メンバーとして[グループのメンバーの投稿](../api/group-post-members.md)を使用しています。</span><span class="sxs-lookup"><span data-stu-id="3bc65-130">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="3bc65-131">応答</span><span class="sxs-lookup"><span data-stu-id="3bc65-131">Response</span></span>

<span data-ttu-id="3bc65-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3bc65-132">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="3bc65-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bc65-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3bc65-136">例</span><span class="sxs-lookup"><span data-stu-id="3bc65-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bc65-137">要求</span><span class="sxs-lookup"><span data-stu-id="3bc65-137">Request</span></span>

<span data-ttu-id="3bc65-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bc65-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="3bc65-139">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bc65-139">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="3bc65-140">応答</span><span class="sxs-lookup"><span data-stu-id="3bc65-140">Response</span></span>

<span data-ttu-id="3bc65-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bc65-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->