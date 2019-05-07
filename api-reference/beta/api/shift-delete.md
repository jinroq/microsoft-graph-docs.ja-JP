---
title: Shift を削除する
description: スケジュールからシフトを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eee9b102ee64bb02b4a13b476a07781c5f3493c0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638621"
---
# <a name="delete-shift"></a><span data-ttu-id="82e69-103">Shift を削除する</span><span class="sxs-lookup"><span data-stu-id="82e69-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82e69-104">スケジュールから[シフト](../resources/shift.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="82e69-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="82e69-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82e69-105">Permissions</span></span>

<span data-ttu-id="82e69-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82e69-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82e69-108">Permission type</span></span>      | <span data-ttu-id="82e69-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82e69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82e69-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82e69-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82e69-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82e69-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82e69-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82e69-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82e69-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82e69-113">Not supported.</span></span>    |
|<span data-ttu-id="82e69-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82e69-114">Application</span></span> | <span data-ttu-id="82e69-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82e69-115">Not supported.</span></span> |

> <span data-ttu-id="82e69-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="82e69-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="82e69-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="82e69-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="82e69-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82e69-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="82e69-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82e69-119">Request headers</span></span>

| <span data-ttu-id="82e69-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82e69-120">Header</span></span>       | <span data-ttu-id="82e69-121">値</span><span class="sxs-lookup"><span data-stu-id="82e69-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82e69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82e69-122">Authorization</span></span>  | <span data-ttu-id="82e69-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82e69-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82e69-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82e69-125">Content-Type</span></span>  | <span data-ttu-id="82e69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82e69-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82e69-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="82e69-127">Request body</span></span>
<span data-ttu-id="82e69-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82e69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82e69-129">応答</span><span class="sxs-lookup"><span data-stu-id="82e69-129">Response</span></span>

<span data-ttu-id="82e69-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="82e69-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82e69-132">例</span><span class="sxs-lookup"><span data-stu-id="82e69-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="82e69-133">要求</span><span class="sxs-lookup"><span data-stu-id="82e69-133">Request</span></span>

<span data-ttu-id="82e69-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82e69-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="82e69-135">応答</span><span class="sxs-lookup"><span data-stu-id="82e69-135">Response</span></span>

<span data-ttu-id="82e69-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82e69-136">The following is an example of the response.</span></span> 

><span data-ttu-id="82e69-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="82e69-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="82e69-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="82e69-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82e69-140">Visual</span><span class="sxs-lookup"><span data-stu-id="82e69-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e69-141">Java</span><span class="sxs-lookup"><span data-stu-id="82e69-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-delete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
