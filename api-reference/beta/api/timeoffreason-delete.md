---
title: timeoffreason の削除
description: isActive プロパティを設定して timeoffreason を非アクティブとしてマークする
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: adf5c7b25f2a0fada834f5d865958cba89673df3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657680"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="a75ba-103">timeoffreason の削除</span><span class="sxs-lookup"><span data-stu-id="a75ba-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a75ba-104">**isActive**プロパティを設定して、 [timeoffreason](../resources/timeoffreason.md)を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="a75ba-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="a75ba-105">このメソッドでは、指定した[timeoffreason](../resources/timeoffreason.md)インスタンスは削除されません。</span><span class="sxs-lookup"><span data-stu-id="a75ba-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="a75ba-106">この理由が割り当てられた[timeoffitem](../resources/timeoffitem.md)インスタンスは、この理由に割り当てられたままになります。</span><span class="sxs-lookup"><span data-stu-id="a75ba-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="a75ba-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a75ba-107">Permissions</span></span>

<span data-ttu-id="a75ba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a75ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a75ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a75ba-110">Permission type</span></span>      | <span data-ttu-id="a75ba-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a75ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a75ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a75ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a75ba-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75ba-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a75ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a75ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a75ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a75ba-115">Not supported.</span></span>    |
|<span data-ttu-id="a75ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a75ba-116">Application</span></span> | <span data-ttu-id="a75ba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a75ba-117">Not supported.</span></span> |

> <span data-ttu-id="a75ba-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a75ba-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a75ba-119">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a75ba-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a75ba-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a75ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="a75ba-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a75ba-121">Request headers</span></span>

| <span data-ttu-id="a75ba-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a75ba-122">Header</span></span>       | <span data-ttu-id="a75ba-123">値</span><span class="sxs-lookup"><span data-stu-id="a75ba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a75ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a75ba-124">Authorization</span></span>  | <span data-ttu-id="a75ba-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a75ba-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a75ba-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a75ba-127">Content-Type</span></span>  | <span data-ttu-id="a75ba-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a75ba-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a75ba-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a75ba-129">Request body</span></span>
<span data-ttu-id="a75ba-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a75ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a75ba-131">応答</span><span class="sxs-lookup"><span data-stu-id="a75ba-131">Response</span></span>

<span data-ttu-id="a75ba-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a75ba-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a75ba-134">例</span><span class="sxs-lookup"><span data-stu-id="a75ba-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a75ba-135">要求</span><span class="sxs-lookup"><span data-stu-id="a75ba-135">Request</span></span>

<span data-ttu-id="a75ba-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a75ba-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="a75ba-137">応答</span><span class="sxs-lookup"><span data-stu-id="a75ba-137">Response</span></span>

<span data-ttu-id="a75ba-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a75ba-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a75ba-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a75ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
