---
title: 'groupLifecyclePolicy: removeGroup'
description: ライフ サイクル ポリシーからグループを削除します。
author: dkershaw10
ms.openlocfilehash: f1fcd8aedc74353d2224b7a670c40b43deb4cd16
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362658"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="ad4f1-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="ad4f1-103">groupLifecyclePolicy: removeGroup</span></span>

> <span data-ttu-id="ad4f1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad4f1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad4f1-106">ライフ サイクル ポリシーからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-106">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad4f1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad4f1-107">Permissions</span></span>

<span data-ttu-id="ad4f1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad4f1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad4f1-110">Permission type</span></span>      | <span data-ttu-id="ad4f1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad4f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad4f1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad4f1-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4f1-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad4f1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad4f1-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="ad4f1-115">Not supported</span></span> |
|<span data-ttu-id="ad4f1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad4f1-116">Application</span></span> |  <span data-ttu-id="ad4f1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4f1-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad4f1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad4f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="ad4f1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad4f1-119">Request headers</span></span>

| <span data-ttu-id="ad4f1-120">名前</span><span class="sxs-lookup"><span data-stu-id="ad4f1-120">Name</span></span> | <span data-ttu-id="ad4f1-121">説明</span><span class="sxs-lookup"><span data-stu-id="ad4f1-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ad4f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4f1-122">Authorization</span></span> | <span data-ttu-id="ad4f1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad4f1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad4f1-125">Content-Type</span></span>  | <span data-ttu-id="ad4f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad4f1-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad4f1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad4f1-127">Request body</span></span>
<span data-ttu-id="ad4f1-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ad4f1-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad4f1-129">Parameter</span></span> | <span data-ttu-id="ad4f1-130">種類</span><span class="sxs-lookup"><span data-stu-id="ad4f1-130">Type</span></span> | <span data-ttu-id="ad4f1-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad4f1-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ad4f1-132">groupId</span><span class="sxs-lookup"><span data-stu-id="ad4f1-132">groupId</span></span>|<span data-ttu-id="ad4f1-133">Guid</span><span class="sxs-lookup"><span data-stu-id="ad4f1-133">Guid</span></span>| <span data-ttu-id="ad4f1-134">ポリシーから削除するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-134">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="ad4f1-135">応答</span><span class="sxs-lookup"><span data-stu-id="ad4f1-135">Response</span></span>

<span data-ttu-id="ad4f1-136">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="ad4f1-137">グループがポリシーから削除された場合、応答本体で、**true**値が返されます。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-137">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="ad4f1-138">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="ad4f1-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="ad4f1-139">例</span><span class="sxs-lookup"><span data-stu-id="ad4f1-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ad4f1-140">要求</span><span class="sxs-lookup"><span data-stu-id="ad4f1-140">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="ad4f1-141">応答</span><span class="sxs-lookup"><span data-stu-id="ad4f1-141">Response</span></span>
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