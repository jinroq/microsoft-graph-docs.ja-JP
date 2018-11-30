---
title: 'groupLifecyclePolicy: renewGroup'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
ms.openlocfilehash: 13e1713d3d00e7feac0b23eae8a314e55341e20e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069259"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="ae819-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="ae819-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="ae819-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae819-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae819-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae819-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae819-107">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="ae819-107">Renews a group's expiration.</span></span> <span data-ttu-id="ae819-108">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="ae819-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="ae819-109">**注:** V1.0 で[の要求を更新するグループ ・ リソースを使用](/graph/api/group-renew?view=graph-rest-1.0)します。</span><span class="sxs-lookup"><span data-stu-id="ae819-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae819-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae819-110">Permissions</span></span>

<span data-ttu-id="ae819-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae819-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="ae819-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae819-113">Permission type</span></span>      | <span data-ttu-id="ae819-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae819-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae819-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae819-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ae819-116">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae819-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae819-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae819-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae819-118">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="ae819-118">Not supported</span></span> |
|<span data-ttu-id="ae819-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae819-119">Application</span></span> | <span data-ttu-id="ae819-120">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae819-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae819-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae819-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="ae819-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae819-122">Request headers</span></span>

| <span data-ttu-id="ae819-123">名前</span><span class="sxs-lookup"><span data-stu-id="ae819-123">Name</span></span> | <span data-ttu-id="ae819-124">説明</span><span class="sxs-lookup"><span data-stu-id="ae819-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ae819-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae819-125">Authorization</span></span> | <span data-ttu-id="ae819-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae819-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae819-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae819-128">Content-Type</span></span>  | <span data-ttu-id="ae819-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ae819-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae819-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae819-130">Request body</span></span>
<span data-ttu-id="ae819-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae819-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae819-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae819-132">Parameter</span></span> | <span data-ttu-id="ae819-133">型</span><span class="sxs-lookup"><span data-stu-id="ae819-133">Type</span></span> | <span data-ttu-id="ae819-134">説明</span><span class="sxs-lookup"><span data-stu-id="ae819-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ae819-135">groupId</span><span class="sxs-lookup"><span data-stu-id="ae819-135">groupId</span></span>|<span data-ttu-id="ae819-136">Guid</span><span class="sxs-lookup"><span data-stu-id="ae819-136">Guid</span></span>| <span data-ttu-id="ae819-137">更新するグループの id。</span><span class="sxs-lookup"><span data-stu-id="ae819-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="ae819-138">応答</span><span class="sxs-lookup"><span data-stu-id="ae819-138">Response</span></span>

<span data-ttu-id="ae819-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ae819-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae819-141">例</span><span class="sxs-lookup"><span data-stu-id="ae819-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae819-142">要求</span><span class="sxs-lookup"><span data-stu-id="ae819-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="ae819-143">応答</span><span class="sxs-lookup"><span data-stu-id="ae819-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->