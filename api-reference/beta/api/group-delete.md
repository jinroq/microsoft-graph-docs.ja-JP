---
title: グループの削除
description: グループを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 349900cffa4b0df1763e1ed8b8213ce81ec27351
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529965"
---
# <a name="delete-group"></a><span data-ttu-id="204de-103">グループの削除</span><span class="sxs-lookup"><span data-stu-id="204de-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="204de-104">グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="204de-104">Deletes a group.</span></span>

<span data-ttu-id="204de-105">グループが削除されると、[削除済みアイテム](../resources/directory.md)にアイテムが追加されます。</span><span class="sxs-lookup"><span data-stu-id="204de-105">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="204de-106">グループは、最大 30 日間に削除済みアイテムに保持されます。</span><span class="sxs-lookup"><span data-stu-id="204de-106">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="204de-107">グループは、削除済みアイテムからで完全に 30 日間に復元できます。</span><span class="sxs-lookup"><span data-stu-id="204de-107">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="204de-108">、30 日後は、削除済みアイテムが完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="204de-108">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="204de-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="204de-109">Permissions</span></span>
<span data-ttu-id="204de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="204de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="204de-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="204de-112">Permission type</span></span>      | <span data-ttu-id="204de-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="204de-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="204de-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="204de-114">Delegated (work or school account)</span></span> | <span data-ttu-id="204de-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="204de-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="204de-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="204de-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="204de-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="204de-117">Not supported.</span></span>    |
|<span data-ttu-id="204de-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="204de-118">Application</span></span> | <span data-ttu-id="204de-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="204de-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="204de-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="204de-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="204de-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="204de-121">Request headers</span></span>
| <span data-ttu-id="204de-122">名前</span><span class="sxs-lookup"><span data-stu-id="204de-122">Name</span></span>       | <span data-ttu-id="204de-123">型</span><span class="sxs-lookup"><span data-stu-id="204de-123">Type</span></span> | <span data-ttu-id="204de-124">説明</span><span class="sxs-lookup"><span data-stu-id="204de-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="204de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="204de-125">Authorization</span></span>  | <span data-ttu-id="204de-126">string</span><span class="sxs-lookup"><span data-stu-id="204de-126">string</span></span>  | <span data-ttu-id="204de-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="204de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="204de-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="204de-129">Request body</span></span>
<span data-ttu-id="204de-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="204de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="204de-131">応答</span><span class="sxs-lookup"><span data-stu-id="204de-131">Response</span></span>
<span data-ttu-id="204de-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="204de-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="204de-134">例</span><span class="sxs-lookup"><span data-stu-id="204de-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="204de-135">要求</span><span class="sxs-lookup"><span data-stu-id="204de-135">Request</span></span>
<span data-ttu-id="204de-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="204de-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="204de-137">応答</span><span class="sxs-lookup"><span data-stu-id="204de-137">Response</span></span>
<span data-ttu-id="204de-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="204de-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
