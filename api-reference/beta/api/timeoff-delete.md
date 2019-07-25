---
title: TimeOff の削除
description: スケジュールから timeOff インスタンスを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ffc2068041a86ac452913dcfe5255222c4bfe59d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868082"
---
# <a name="delete-timeoff"></a><span data-ttu-id="2b209-103">TimeOff の削除</span><span class="sxs-lookup"><span data-stu-id="2b209-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b209-104">[スケジュール](../resources/schedule.md)から[timeoff](../resources/timeoff.md)インスタンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b209-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b209-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b209-105">Permissions</span></span>

<span data-ttu-id="2b209-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b209-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b209-108">Permission type</span></span>      | <span data-ttu-id="2b209-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b209-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b209-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b209-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b209-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b209-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b209-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b209-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b209-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b209-113">Not supported.</span></span>    |
|<span data-ttu-id="2b209-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b209-114">Application</span></span> | <span data-ttu-id="2b209-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b209-115">Not supported.</span></span> |

> <span data-ttu-id="2b209-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b209-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2b209-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2b209-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b209-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b209-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="2b209-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b209-119">Request headers</span></span>

| <span data-ttu-id="2b209-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b209-120">Header</span></span>       | <span data-ttu-id="2b209-121">値</span><span class="sxs-lookup"><span data-stu-id="2b209-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b209-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b209-122">Authorization</span></span>  | <span data-ttu-id="2b209-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b209-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b209-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b209-125">Content-Type</span></span>  | <span data-ttu-id="2b209-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b209-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b209-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b209-127">Request body</span></span>
<span data-ttu-id="2b209-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b209-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b209-129">応答</span><span class="sxs-lookup"><span data-stu-id="2b209-129">Response</span></span>

<span data-ttu-id="2b209-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2b209-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b209-132">例</span><span class="sxs-lookup"><span data-stu-id="2b209-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2b209-133">要求</span><span class="sxs-lookup"><span data-stu-id="2b209-133">Request</span></span>

<span data-ttu-id="2b209-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b209-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b209-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2b209-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b209-136">C#</span><span class="sxs-lookup"><span data-stu-id="2b209-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b209-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b209-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b209-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="2b209-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2b209-139">Java</span><span class="sxs-lookup"><span data-stu-id="2b209-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b209-140">応答</span><span class="sxs-lookup"><span data-stu-id="2b209-140">Response</span></span>

<span data-ttu-id="2b209-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b209-141">The following is an example of the response.</span></span> 

><span data-ttu-id="2b209-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2b209-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
