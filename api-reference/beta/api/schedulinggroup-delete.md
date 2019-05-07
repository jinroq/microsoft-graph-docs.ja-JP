---
title: Delete schedulingGroup
description: IsActive プロパティを設定して、schedulingGroup を非アクティブとしてマークする
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5e4f4526164b78d7025a8cee097565670e12304e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639062"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="20034-103">Delete schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="20034-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20034-104">**IsActive**プロパティを設定して、 [schedulingGroup](../resources/schedulinggroup.md)を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="20034-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="20034-105">このメソッドでは、スケジュールから[schedulingGroup](../resources/schedulinggroup.md)が削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="20034-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="20034-106">スケジュールグループに割り当てられている既存の[シフト](../resources/shift.md)インスタンスは、グループの一部として残ります。</span><span class="sxs-lookup"><span data-stu-id="20034-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="20034-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20034-107">Permissions</span></span>

<span data-ttu-id="20034-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20034-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20034-110">Permission type</span></span>      | <span data-ttu-id="20034-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20034-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20034-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20034-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20034-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20034-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="20034-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20034-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20034-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20034-115">Not supported.</span></span>    |
|<span data-ttu-id="20034-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20034-116">Application</span></span> | <span data-ttu-id="20034-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20034-117">Not supported.</span></span> |

> <span data-ttu-id="20034-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="20034-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="20034-119">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="20034-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="20034-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20034-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="20034-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20034-121">Request headers</span></span>

| <span data-ttu-id="20034-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20034-122">Header</span></span>       | <span data-ttu-id="20034-123">値</span><span class="sxs-lookup"><span data-stu-id="20034-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="20034-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20034-124">Authorization</span></span>  | <span data-ttu-id="20034-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20034-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="20034-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20034-127">Content-Type</span></span>  | <span data-ttu-id="20034-128">application/json</span><span class="sxs-lookup"><span data-stu-id="20034-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="20034-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="20034-129">Request body</span></span>
<span data-ttu-id="20034-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="20034-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20034-131">応答</span><span class="sxs-lookup"><span data-stu-id="20034-131">Response</span></span>

<span data-ttu-id="20034-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="20034-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20034-134">例</span><span class="sxs-lookup"><span data-stu-id="20034-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="20034-135">要求</span><span class="sxs-lookup"><span data-stu-id="20034-135">Request</span></span>

<span data-ttu-id="20034-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20034-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="20034-137">応答</span><span class="sxs-lookup"><span data-stu-id="20034-137">Response</span></span>

<span data-ttu-id="20034-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20034-138">The following is an example of the response.</span></span> 

><span data-ttu-id="20034-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="20034-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="20034-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="20034-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20034-142">Visual</span><span class="sxs-lookup"><span data-stu-id="20034-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-delete-schedulinggroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20034-143">Java</span><span class="sxs-lookup"><span data-stu-id="20034-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-delete-schedulinggroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedulinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedulinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
