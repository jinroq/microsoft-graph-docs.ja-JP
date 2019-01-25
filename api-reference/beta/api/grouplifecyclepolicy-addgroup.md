---
title: 'groupLifecyclePolicy: addGroup'
description: ライフ サイクル ポリシーにグループを追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f5aee25421dea76b5bdb10f141d4e640c2196b94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515511"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="e21e9-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="e21e9-103">groupLifecyclePolicy: addGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e21e9-104">ライフ サイクル ポリシーにグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="e21e9-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e21e9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e21e9-105">Permissions</span></span>

<span data-ttu-id="e21e9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e21e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e21e9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e21e9-108">Permission type</span></span>      | <span data-ttu-id="e21e9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e21e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e21e9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e21e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e21e9-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21e9-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e21e9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e21e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e21e9-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e21e9-113">Not supported</span></span> |
|<span data-ttu-id="e21e9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e21e9-114">Application</span></span> | <span data-ttu-id="e21e9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21e9-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e21e9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e21e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="e21e9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e21e9-117">Request headers</span></span>

| <span data-ttu-id="e21e9-118">名前</span><span class="sxs-lookup"><span data-stu-id="e21e9-118">Name</span></span> | <span data-ttu-id="e21e9-119">説明</span><span class="sxs-lookup"><span data-stu-id="e21e9-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e21e9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e21e9-120">Authorization</span></span> | <span data-ttu-id="e21e9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e21e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e21e9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e21e9-123">Content-Type</span></span>  | <span data-ttu-id="e21e9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e21e9-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e21e9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e21e9-125">Request body</span></span>
<span data-ttu-id="e21e9-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e21e9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e21e9-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e21e9-127">Parameter</span></span> | <span data-ttu-id="e21e9-128">型</span><span class="sxs-lookup"><span data-stu-id="e21e9-128">Type</span></span> | <span data-ttu-id="e21e9-129">説明</span><span class="sxs-lookup"><span data-stu-id="e21e9-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e21e9-130">groupId</span><span class="sxs-lookup"><span data-stu-id="e21e9-130">groupId</span></span>|<span data-ttu-id="e21e9-131">Guid</span><span class="sxs-lookup"><span data-stu-id="e21e9-131">Guid</span></span>| <span data-ttu-id="e21e9-132">ポリシーに追加するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="e21e9-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="e21e9-133">応答</span><span class="sxs-lookup"><span data-stu-id="e21e9-133">Response</span></span>

<span data-ttu-id="e21e9-134">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e21e9-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="e21e9-135">グループがポリシーに追加された場合、応答本体で、**true** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="e21e9-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="e21e9-136">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="e21e9-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="e21e9-137">例</span><span class="sxs-lookup"><span data-stu-id="e21e9-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e21e9-138">要求</span><span class="sxs-lookup"><span data-stu-id="e21e9-138">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e21e9-139">応答</span><span class="sxs-lookup"><span data-stu-id="e21e9-139">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-addgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
