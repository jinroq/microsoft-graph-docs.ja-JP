---
title: 'groupLifecyclePolicy: removeGroup'
description: ライフ サイクル ポリシーからグループを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b6f5e7b736ad1467d9cdf0f20e9d5626b6d950c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014558"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="5d802-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="5d802-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="5d802-104">ライフ サイクル ポリシーからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="5d802-104">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d802-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d802-105">Permissions</span></span>

<span data-ttu-id="5d802-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d802-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d802-108">Permission type</span></span>      | <span data-ttu-id="5d802-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d802-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d802-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d802-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d802-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d802-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d802-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d802-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d802-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d802-113">Not supported.</span></span>    |
|<span data-ttu-id="5d802-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d802-114">Application</span></span> | <span data-ttu-id="5d802-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d802-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d802-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d802-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="5d802-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d802-117">Request headers</span></span>

| <span data-ttu-id="5d802-118">名前</span><span class="sxs-lookup"><span data-stu-id="5d802-118">Name</span></span> | <span data-ttu-id="5d802-119">説明</span><span class="sxs-lookup"><span data-stu-id="5d802-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5d802-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d802-120">Authorization</span></span> | <span data-ttu-id="5d802-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d802-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d802-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d802-123">Content-Type</span></span>  | <span data-ttu-id="5d802-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d802-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d802-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d802-125">Request body</span></span>
<span data-ttu-id="5d802-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5d802-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d802-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d802-127">Parameter</span></span> | <span data-ttu-id="5d802-128">型</span><span class="sxs-lookup"><span data-stu-id="5d802-128">Type</span></span> | <span data-ttu-id="5d802-129">説明</span><span class="sxs-lookup"><span data-stu-id="5d802-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5d802-130">groupId</span><span class="sxs-lookup"><span data-stu-id="5d802-130">groupId</span></span>|<span data-ttu-id="5d802-131">Guid</span><span class="sxs-lookup"><span data-stu-id="5d802-131">Guid</span></span>| <span data-ttu-id="5d802-132">ポリシーから削除するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="5d802-132">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="5d802-133">応答</span><span class="sxs-lookup"><span data-stu-id="5d802-133">Response</span></span>

<span data-ttu-id="5d802-134">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5d802-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="5d802-135">グループがポリシーから削除された場合、応答本体で、**true**値が返されます。</span><span class="sxs-lookup"><span data-stu-id="5d802-135">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="5d802-136">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="5d802-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="5d802-137">例</span><span class="sxs-lookup"><span data-stu-id="5d802-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d802-138">要求</span><span class="sxs-lookup"><span data-stu-id="5d802-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="5d802-139">応答</span><span class="sxs-lookup"><span data-stu-id="5d802-139">Response</span></span>
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
