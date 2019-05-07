---
title: TimeOff の削除
description: スケジュールから timeOff インスタンスを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d55831167813d64e2bf010420320fc7d5f4be8d1
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637543"
---
# <a name="delete-timeoff"></a><span data-ttu-id="0ea95-103">TimeOff の削除</span><span class="sxs-lookup"><span data-stu-id="0ea95-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea95-104">[スケジュール](../resources/schedule.md)から[Timeoff](../resources/timeoff.md)インスタンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="0ea95-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea95-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ea95-105">Permissions</span></span>

<span data-ttu-id="0ea95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ea95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea95-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ea95-108">Permission type</span></span>      | <span data-ttu-id="0ea95-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ea95-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea95-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea95-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea95-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea95-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ea95-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea95-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea95-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea95-113">Not supported.</span></span>    |
|<span data-ttu-id="0ea95-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ea95-114">Application</span></span> | <span data-ttu-id="0ea95-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea95-115">Not supported.</span></span> |

> <span data-ttu-id="0ea95-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0ea95-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0ea95-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0ea95-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ea95-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ea95-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="0ea95-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea95-119">Request headers</span></span>

| <span data-ttu-id="0ea95-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea95-120">Header</span></span>       | <span data-ttu-id="0ea95-121">値</span><span class="sxs-lookup"><span data-stu-id="0ea95-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ea95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea95-122">Authorization</span></span>  | <span data-ttu-id="0ea95-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0ea95-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0ea95-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ea95-125">Content-Type</span></span>  | <span data-ttu-id="0ea95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ea95-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ea95-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ea95-127">Request body</span></span>
<span data-ttu-id="0ea95-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0ea95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea95-129">応答</span><span class="sxs-lookup"><span data-stu-id="0ea95-129">Response</span></span>

<span data-ttu-id="0ea95-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0ea95-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea95-132">例</span><span class="sxs-lookup"><span data-stu-id="0ea95-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0ea95-133">要求</span><span class="sxs-lookup"><span data-stu-id="0ea95-133">Request</span></span>

<span data-ttu-id="0ea95-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0ea95-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="0ea95-135">応答</span><span class="sxs-lookup"><span data-stu-id="0ea95-135">Response</span></span>

<span data-ttu-id="0ea95-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0ea95-136">The following is an example of the response.</span></span> 

><span data-ttu-id="0ea95-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0ea95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ea95-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0ea95-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ea95-140">Visual</span><span class="sxs-lookup"><span data-stu-id="0ea95-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ea95-141">Java</span><span class="sxs-lookup"><span data-stu-id="0ea95-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-delete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
