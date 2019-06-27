---
title: TimeOff の削除
description: スケジュールから timeOff インスタンスを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ee20d51fe5cf2c3cc01db23e65398deba2263e68
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270589"
---
# <a name="delete-timeoff"></a><span data-ttu-id="5f819-103">TimeOff の削除</span><span class="sxs-lookup"><span data-stu-id="5f819-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f819-104">[スケジュール](../resources/schedule.md)から[timeoff](../resources/timeoff.md)インスタンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="5f819-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f819-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f819-105">Permissions</span></span>

<span data-ttu-id="5f819-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f819-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f819-108">Permission type</span></span>      | <span data-ttu-id="5f819-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f819-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f819-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f819-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f819-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f819-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f819-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f819-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f819-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f819-113">Not supported.</span></span>    |
|<span data-ttu-id="5f819-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f819-114">Application</span></span> | <span data-ttu-id="5f819-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f819-115">Not supported.</span></span> |

> <span data-ttu-id="5f819-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5f819-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5f819-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5f819-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f819-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f819-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="5f819-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f819-119">Request headers</span></span>

| <span data-ttu-id="5f819-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f819-120">Header</span></span>       | <span data-ttu-id="5f819-121">値</span><span class="sxs-lookup"><span data-stu-id="5f819-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f819-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f819-122">Authorization</span></span>  | <span data-ttu-id="5f819-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f819-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f819-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f819-125">Content-Type</span></span>  | <span data-ttu-id="5f819-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f819-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f819-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f819-127">Request body</span></span>
<span data-ttu-id="5f819-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f819-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f819-129">応答</span><span class="sxs-lookup"><span data-stu-id="5f819-129">Response</span></span>

<span data-ttu-id="5f819-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5f819-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f819-132">例</span><span class="sxs-lookup"><span data-stu-id="5f819-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f819-133">要求</span><span class="sxs-lookup"><span data-stu-id="5f819-133">Request</span></span>

<span data-ttu-id="5f819-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f819-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="5f819-135">応答</span><span class="sxs-lookup"><span data-stu-id="5f819-135">Response</span></span>

<span data-ttu-id="5f819-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f819-136">The following is an example of the response.</span></span> 

><span data-ttu-id="5f819-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5f819-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5f819-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5f819-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5f819-140">C#</span><span class="sxs-lookup"><span data-stu-id="5f819-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f819-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="5f819-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5f819-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="5f819-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoff-delete-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
