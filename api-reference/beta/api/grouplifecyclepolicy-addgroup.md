---
title: 'groupLifecyclePolicy: addGroup'
description: ライフ サイクル ポリシーにグループを追加します。
author: dkershaw10
ms.openlocfilehash: 57af4383c471832acbffb4136a057c91a1d061d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327910"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="47a4d-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="47a4d-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="47a4d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47a4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a4d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47a4d-106">ライフ サイクル ポリシーにグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="47a4d-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="47a4d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="47a4d-107">Permissions</span></span>

<span data-ttu-id="47a4d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47a4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="47a4d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47a4d-110">Permission type</span></span>      | <span data-ttu-id="47a4d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="47a4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a4d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47a4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47a4d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47a4d-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="47a4d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47a4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a4d-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="47a4d-115">Not supported</span></span> |
|<span data-ttu-id="47a4d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47a4d-116">Application</span></span> | <span data-ttu-id="47a4d-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47a4d-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a4d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47a4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="47a4d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47a4d-119">Request headers</span></span>

| <span data-ttu-id="47a4d-120">名前</span><span class="sxs-lookup"><span data-stu-id="47a4d-120">Name</span></span> | <span data-ttu-id="47a4d-121">説明</span><span class="sxs-lookup"><span data-stu-id="47a4d-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="47a4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47a4d-122">Authorization</span></span> | <span data-ttu-id="47a4d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="47a4d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47a4d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47a4d-125">Content-Type</span></span>  | <span data-ttu-id="47a4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47a4d-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="47a4d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="47a4d-127">Request body</span></span>
<span data-ttu-id="47a4d-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="47a4d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47a4d-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="47a4d-129">Parameter</span></span> | <span data-ttu-id="47a4d-130">種類</span><span class="sxs-lookup"><span data-stu-id="47a4d-130">Type</span></span> | <span data-ttu-id="47a4d-131">説明</span><span class="sxs-lookup"><span data-stu-id="47a4d-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="47a4d-132">groupId</span><span class="sxs-lookup"><span data-stu-id="47a4d-132">groupId</span></span>|<span data-ttu-id="47a4d-133">Guid</span><span class="sxs-lookup"><span data-stu-id="47a4d-133">Guid</span></span>| <span data-ttu-id="47a4d-134">ポリシーに追加するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="47a4d-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="47a4d-135">応答</span><span class="sxs-lookup"><span data-stu-id="47a4d-135">Response</span></span>

<span data-ttu-id="47a4d-136">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="47a4d-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="47a4d-137">グループがポリシーに追加された場合、応答本体で、**true** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="47a4d-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="47a4d-138">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="47a4d-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="47a4d-139">例</span><span class="sxs-lookup"><span data-stu-id="47a4d-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="47a4d-140">要求</span><span class="sxs-lookup"><span data-stu-id="47a4d-140">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="47a4d-141">応答</span><span class="sxs-lookup"><span data-stu-id="47a4d-141">Response</span></span>
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