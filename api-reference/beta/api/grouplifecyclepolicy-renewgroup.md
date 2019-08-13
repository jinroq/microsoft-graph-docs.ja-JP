---
title: 'groupLifecyclePolicy: renewGroup'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 57179bdc1d542e58cbf5ffa8411dcf3b1eed4ce4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322994"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="08cb3-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="08cb3-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08cb3-105">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="08cb3-105">Renews a group's expiration.</span></span> <span data-ttu-id="08cb3-106">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="08cb3-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="08cb3-107">**注:** V 1.0 で[は、グループリソースを使用して更新要求を行い](/graph/api/group-renew?view=graph-rest-1.0)ます。</span><span class="sxs-lookup"><span data-stu-id="08cb3-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="08cb3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08cb3-108">Permissions</span></span>

<span data-ttu-id="08cb3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08cb3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="08cb3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08cb3-111">Permission type</span></span>      | <span data-ttu-id="08cb3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08cb3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08cb3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08cb3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08cb3-114">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cb3-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="08cb3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08cb3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08cb3-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="08cb3-116">Not supported</span></span> |
|<span data-ttu-id="08cb3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08cb3-117">Application</span></span> | <span data-ttu-id="08cb3-118">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cb3-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08cb3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08cb3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="08cb3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08cb3-120">Request headers</span></span>

| <span data-ttu-id="08cb3-121">名前</span><span class="sxs-lookup"><span data-stu-id="08cb3-121">Name</span></span> | <span data-ttu-id="08cb3-122">説明</span><span class="sxs-lookup"><span data-stu-id="08cb3-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="08cb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08cb3-123">Authorization</span></span> | <span data-ttu-id="08cb3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08cb3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08cb3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08cb3-126">Content-Type</span></span>  | <span data-ttu-id="08cb3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="08cb3-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08cb3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="08cb3-128">Request body</span></span>
<span data-ttu-id="08cb3-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="08cb3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08cb3-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="08cb3-130">Parameter</span></span> | <span data-ttu-id="08cb3-131">型</span><span class="sxs-lookup"><span data-stu-id="08cb3-131">Type</span></span> | <span data-ttu-id="08cb3-132">説明</span><span class="sxs-lookup"><span data-stu-id="08cb3-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="08cb3-133">groupId</span><span class="sxs-lookup"><span data-stu-id="08cb3-133">groupId</span></span>|<span data-ttu-id="08cb3-134">Guid</span><span class="sxs-lookup"><span data-stu-id="08cb3-134">Guid</span></span>| <span data-ttu-id="08cb3-135">更新するグループの id。</span><span class="sxs-lookup"><span data-stu-id="08cb3-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="08cb3-136">応答</span><span class="sxs-lookup"><span data-stu-id="08cb3-136">Response</span></span>

<span data-ttu-id="08cb3-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="08cb3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08cb3-139">例</span><span class="sxs-lookup"><span data-stu-id="08cb3-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08cb3-140">要求</span><span class="sxs-lookup"><span data-stu-id="08cb3-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="08cb3-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08cb3-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="08cb3-142">C#</span><span class="sxs-lookup"><span data-stu-id="08cb3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08cb3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08cb3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08cb3-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="08cb3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08cb3-145">Java</span><span class="sxs-lookup"><span data-stu-id="08cb3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08cb3-146">応答</span><span class="sxs-lookup"><span data-stu-id="08cb3-146">Response</span></span>

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
  "suppressions": [
  ]
}
-->
