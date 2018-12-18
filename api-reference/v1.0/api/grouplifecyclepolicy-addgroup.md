---
title: 'groupLifecyclePolicy: addGroup'
description: ライフ サイクル ポリシーにグループを追加します。
author: dkershaw10
ms.openlocfilehash: 1ee36dd824d41c0a37c818d1e42e29a912857d20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321148"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="b85ee-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="b85ee-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="b85ee-104">ライフ サイクル ポリシーにグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="b85ee-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b85ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b85ee-105">Permissions</span></span>

<span data-ttu-id="b85ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b85ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b85ee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b85ee-108">Permission type</span></span>      | <span data-ttu-id="b85ee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b85ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b85ee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b85ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b85ee-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b85ee-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b85ee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b85ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b85ee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b85ee-113">Not supported.</span></span>    |
|<span data-ttu-id="b85ee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b85ee-114">Application</span></span> | <span data-ttu-id="b85ee-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b85ee-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b85ee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b85ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="b85ee-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b85ee-117">Request headers</span></span>

| <span data-ttu-id="b85ee-118">名前</span><span class="sxs-lookup"><span data-stu-id="b85ee-118">Name</span></span> | <span data-ttu-id="b85ee-119">説明</span><span class="sxs-lookup"><span data-stu-id="b85ee-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b85ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b85ee-120">Authorization</span></span> | <span data-ttu-id="b85ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b85ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b85ee-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b85ee-123">Content-Type</span></span>  | <span data-ttu-id="b85ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b85ee-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b85ee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b85ee-125">Request body</span></span>
<span data-ttu-id="b85ee-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b85ee-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b85ee-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b85ee-127">Parameter</span></span> | <span data-ttu-id="b85ee-128">種類</span><span class="sxs-lookup"><span data-stu-id="b85ee-128">Type</span></span> | <span data-ttu-id="b85ee-129">説明</span><span class="sxs-lookup"><span data-stu-id="b85ee-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b85ee-130">groupId</span><span class="sxs-lookup"><span data-stu-id="b85ee-130">groupId</span></span>|<span data-ttu-id="b85ee-131">Guid</span><span class="sxs-lookup"><span data-stu-id="b85ee-131">Guid</span></span>| <span data-ttu-id="b85ee-132">ポリシーに追加するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="b85ee-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="b85ee-133">応答</span><span class="sxs-lookup"><span data-stu-id="b85ee-133">Response</span></span>

<span data-ttu-id="b85ee-134">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b85ee-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="b85ee-135">グループがポリシーに追加された場合、応答本体で、**true** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="b85ee-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="b85ee-136">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="b85ee-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="b85ee-137">例</span><span class="sxs-lookup"><span data-stu-id="b85ee-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b85ee-138">要求</span><span class="sxs-lookup"><span data-stu-id="b85ee-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="b85ee-139">応答</span><span class="sxs-lookup"><span data-stu-id="b85ee-139">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->