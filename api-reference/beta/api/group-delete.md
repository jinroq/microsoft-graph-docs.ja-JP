---
title: グループの削除
description: グループを削除します。
ms.openlocfilehash: 92a15366fefb6ab70c45f664daa28b75bcea5891
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069512"
---
# <a name="delete-group"></a><span data-ttu-id="5d3c1-103">グループの削除</span><span class="sxs-lookup"><span data-stu-id="5d3c1-103">Delete group</span></span>

> <span data-ttu-id="5d3c1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d3c1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d3c1-106">グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-106">Deletes a group.</span></span>

<span data-ttu-id="5d3c1-107">グループが削除されると、[削除済みアイテム](../resources/directory.md)にアイテムが追加されます。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="5d3c1-108">グループは、最大 30 日間に削除済みアイテムに保持されます。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="5d3c1-109">グループは、削除済みアイテムからで完全に 30 日間に復元できます。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="5d3c1-110">、30 日後は、削除済みアイテムが完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3c1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d3c1-111">Permissions</span></span>
<span data-ttu-id="5d3c1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3c1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d3c1-114">Permission type</span></span>      | <span data-ttu-id="5d3c1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d3c1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d3c1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d3c1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5d3c1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3c1-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d3c1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d3c1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3c1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-119">Not supported.</span></span>    |
|<span data-ttu-id="5d3c1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d3c1-120">Application</span></span> | <span data-ttu-id="5d3c1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3c1-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3c1-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d3c1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d3c1-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d3c1-123">Request headers</span></span>
| <span data-ttu-id="5d3c1-124">名前</span><span class="sxs-lookup"><span data-stu-id="5d3c1-124">Name</span></span>       | <span data-ttu-id="5d3c1-125">型</span><span class="sxs-lookup"><span data-stu-id="5d3c1-125">Type</span></span> | <span data-ttu-id="5d3c1-126">説明</span><span class="sxs-lookup"><span data-stu-id="5d3c1-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d3c1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3c1-127">Authorization</span></span>  | <span data-ttu-id="5d3c1-128">string</span><span class="sxs-lookup"><span data-stu-id="5d3c1-128">string</span></span>  | <span data-ttu-id="5d3c1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d3c1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d3c1-131">Request body</span></span>
<span data-ttu-id="5d3c1-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3c1-133">応答</span><span class="sxs-lookup"><span data-stu-id="5d3c1-133">Response</span></span>
<span data-ttu-id="5d3c1-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d3c1-136">例</span><span class="sxs-lookup"><span data-stu-id="5d3c1-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5d3c1-137">要求</span><span class="sxs-lookup"><span data-stu-id="5d3c1-137">Request</span></span>
<span data-ttu-id="5d3c1-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="5d3c1-139">応答</span><span class="sxs-lookup"><span data-stu-id="5d3c1-139">Response</span></span>
<span data-ttu-id="5d3c1-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d3c1-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->