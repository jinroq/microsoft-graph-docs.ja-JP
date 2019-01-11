---
title: グループの削除
description: グループを削除します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 9eb46ffbfe767accee457f9b5b6dc292891fb95c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865080"
---
# <a name="delete-group"></a><span data-ttu-id="9490a-103">グループの削除</span><span class="sxs-lookup"><span data-stu-id="9490a-103">Delete group</span></span>

> <span data-ttu-id="9490a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9490a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9490a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9490a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9490a-106">グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="9490a-106">Deletes a group.</span></span>

<span data-ttu-id="9490a-107">グループが削除されると、[削除済みアイテム](../resources/directory.md)にアイテムが追加されます。</span><span class="sxs-lookup"><span data-stu-id="9490a-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="9490a-108">グループは、最大 30 日間に削除済みアイテムに保持されます。</span><span class="sxs-lookup"><span data-stu-id="9490a-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="9490a-109">グループは、削除済みアイテムからで完全に 30 日間に復元できます。</span><span class="sxs-lookup"><span data-stu-id="9490a-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="9490a-110">、30 日後は、削除済みアイテムが完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="9490a-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="9490a-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9490a-111">Permissions</span></span>
<span data-ttu-id="9490a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9490a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9490a-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9490a-114">Permission type</span></span>      | <span data-ttu-id="9490a-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9490a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9490a-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9490a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9490a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9490a-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9490a-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9490a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9490a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9490a-119">Not supported.</span></span>    |
|<span data-ttu-id="9490a-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9490a-120">Application</span></span> | <span data-ttu-id="9490a-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9490a-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9490a-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9490a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9490a-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9490a-123">Request headers</span></span>
| <span data-ttu-id="9490a-124">名前</span><span class="sxs-lookup"><span data-stu-id="9490a-124">Name</span></span>       | <span data-ttu-id="9490a-125">種類</span><span class="sxs-lookup"><span data-stu-id="9490a-125">Type</span></span> | <span data-ttu-id="9490a-126">説明</span><span class="sxs-lookup"><span data-stu-id="9490a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9490a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9490a-127">Authorization</span></span>  | <span data-ttu-id="9490a-128">string</span><span class="sxs-lookup"><span data-stu-id="9490a-128">string</span></span>  | <span data-ttu-id="9490a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9490a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9490a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9490a-131">Request body</span></span>
<span data-ttu-id="9490a-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9490a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9490a-133">応答</span><span class="sxs-lookup"><span data-stu-id="9490a-133">Response</span></span>
<span data-ttu-id="9490a-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9490a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9490a-136">例</span><span class="sxs-lookup"><span data-stu-id="9490a-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9490a-137">要求</span><span class="sxs-lookup"><span data-stu-id="9490a-137">Request</span></span>
<span data-ttu-id="9490a-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9490a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="9490a-139">応答</span><span class="sxs-lookup"><span data-stu-id="9490a-139">Response</span></span>
<span data-ttu-id="9490a-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9490a-140">The following is an example of the response.</span></span> 
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
