---
title: Create plannerPlan
description: この API を使用して、新しい **plannerPlan** を作成します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 94956443d88237c8df9bc06e6e237fbac2a288ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456163"
---
# <a name="create-plannerplan"></a><span data-ttu-id="ed020-103">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ed020-103">Create plannerPlan</span></span>

<span data-ttu-id="ed020-104">この API を使用して、新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="ed020-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed020-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed020-105">Permissions</span></span>

<span data-ttu-id="ed020-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed020-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed020-108">Permission type</span></span>                        | <span data-ttu-id="ed020-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed020-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ed020-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed020-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed020-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed020-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="ed020-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed020-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed020-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed020-113">Not supported.</span></span>                              |
| <span data-ttu-id="ed020-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed020-114">Application</span></span>                            | <span data-ttu-id="ed020-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed020-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="ed020-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed020-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="ed020-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed020-117">Request headers</span></span>

| <span data-ttu-id="ed020-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed020-118">Name</span></span>          | <span data-ttu-id="ed020-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed020-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ed020-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed020-120">Authorization</span></span> | <span data-ttu-id="ed020-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed020-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed020-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed020-123">Request body</span></span>

<span data-ttu-id="ed020-p103">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。**plannerPlan** 所有者プロパティは、[group](../resources/group.md) オブジェクトの ID に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed020-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="ed020-126">**注意:** プランを作成するユーザーは、プランを所有するグループのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed020-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="ed020-127">あなたが新しいグループを[グループの作成](../api/group-post-groups.md)を使用して作成しても、メンバーとしてそのグループに追加されることはありません。</span><span class="sxs-lookup"><span data-stu-id="ed020-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="ed020-128">グループを作成したら、[グループ投稿メンバー](../api/group-post-members.md)を使用して自分自身をメンバーとして追加します。</span><span class="sxs-lookup"><span data-stu-id="ed020-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="ed020-129">応答</span><span class="sxs-lookup"><span data-stu-id="ed020-129">Response</span></span>

<span data-ttu-id="ed020-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed020-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="ed020-p105">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed020-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ed020-134">例</span><span class="sxs-lookup"><span data-stu-id="ed020-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed020-135">要求</span><span class="sxs-lookup"><span data-stu-id="ed020-135">Request</span></span>

<span data-ttu-id="ed020-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed020-136">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ed020-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ed020-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed020-138">C#</span><span class="sxs-lookup"><span data-stu-id="ed020-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed020-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed020-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed020-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="ed020-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ed020-141">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed020-141">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="ed020-142">応答</span><span class="sxs-lookup"><span data-stu-id="ed020-142">Response</span></span>

<span data-ttu-id="ed020-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed020-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
