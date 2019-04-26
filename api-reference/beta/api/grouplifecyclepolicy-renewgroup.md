---
title: 'groupLifecyclePolicy: renewgroup'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 60c940f20063db6ae764e632cdf4a69edc65df2a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328640"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="039ba-104">groupLifecyclePolicy: renewgroup</span><span class="sxs-lookup"><span data-stu-id="039ba-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="039ba-105">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="039ba-105">Renews a group's expiration.</span></span> <span data-ttu-id="039ba-106">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="039ba-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="039ba-107">**注:** v 1.0 で[は、グループリソースを使用して更新要求を行い](/graph/api/group-renew?view=graph-rest-1.0)ます。</span><span class="sxs-lookup"><span data-stu-id="039ba-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="039ba-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="039ba-108">Permissions</span></span>

<span data-ttu-id="039ba-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="039ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="039ba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="039ba-111">Permission type</span></span>      | <span data-ttu-id="039ba-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="039ba-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="039ba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="039ba-113">Delegated (work or school account)</span></span> | <span data-ttu-id="039ba-114">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039ba-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="039ba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="039ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="039ba-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="039ba-116">Not supported</span></span> |
|<span data-ttu-id="039ba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="039ba-117">Application</span></span> | <span data-ttu-id="039ba-118">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039ba-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="039ba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="039ba-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="039ba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="039ba-120">Request headers</span></span>

| <span data-ttu-id="039ba-121">名前</span><span class="sxs-lookup"><span data-stu-id="039ba-121">Name</span></span> | <span data-ttu-id="039ba-122">説明</span><span class="sxs-lookup"><span data-stu-id="039ba-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="039ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="039ba-123">Authorization</span></span> | <span data-ttu-id="039ba-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="039ba-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="039ba-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="039ba-126">Content-Type</span></span>  | <span data-ttu-id="039ba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="039ba-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="039ba-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="039ba-128">Request body</span></span>
<span data-ttu-id="039ba-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="039ba-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="039ba-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="039ba-130">Parameter</span></span> | <span data-ttu-id="039ba-131">型</span><span class="sxs-lookup"><span data-stu-id="039ba-131">Type</span></span> | <span data-ttu-id="039ba-132">説明</span><span class="sxs-lookup"><span data-stu-id="039ba-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="039ba-133">groupId</span><span class="sxs-lookup"><span data-stu-id="039ba-133">groupId</span></span>|<span data-ttu-id="039ba-134">Guid</span><span class="sxs-lookup"><span data-stu-id="039ba-134">Guid</span></span>| <span data-ttu-id="039ba-135">更新するグループの id。</span><span class="sxs-lookup"><span data-stu-id="039ba-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="039ba-136">応答</span><span class="sxs-lookup"><span data-stu-id="039ba-136">Response</span></span>

<span data-ttu-id="039ba-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="039ba-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039ba-139">例</span><span class="sxs-lookup"><span data-stu-id="039ba-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="039ba-140">要求</span><span class="sxs-lookup"><span data-stu-id="039ba-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="039ba-141">応答</span><span class="sxs-lookup"><span data-stu-id="039ba-141">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
