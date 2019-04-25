---
title: shift を削除する
description: スケジュールからシフトを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8bf6483663607767550a48fa801619b8d2842c63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537504"
---
# <a name="delete-shift"></a><span data-ttu-id="d7dc7-103">shift を削除する</span><span class="sxs-lookup"><span data-stu-id="d7dc7-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7dc7-104">スケジュールから[シフト](../resources/shift.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7dc7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7dc7-105">Permissions</span></span>

<span data-ttu-id="d7dc7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7dc7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7dc7-108">Permission type</span></span>      | <span data-ttu-id="d7dc7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7dc7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7dc7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7dc7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7dc7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7dc7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7dc7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7dc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7dc7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-113">Not supported.</span></span>    |
|<span data-ttu-id="d7dc7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7dc7-114">Application</span></span> | <span data-ttu-id="d7dc7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-115">Not supported.</span></span> |

> <span data-ttu-id="d7dc7-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d7dc7-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d7dc7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7dc7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="d7dc7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7dc7-119">Request headers</span></span>

| <span data-ttu-id="d7dc7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7dc7-120">Header</span></span>       | <span data-ttu-id="d7dc7-121">値</span><span class="sxs-lookup"><span data-stu-id="d7dc7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7dc7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7dc7-122">Authorization</span></span>  | <span data-ttu-id="d7dc7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7dc7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7dc7-125">Content-Type</span></span>  | <span data-ttu-id="d7dc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7dc7-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7dc7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7dc7-127">Request body</span></span>
<span data-ttu-id="d7dc7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7dc7-129">応答</span><span class="sxs-lookup"><span data-stu-id="d7dc7-129">Response</span></span>

<span data-ttu-id="d7dc7-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7dc7-132">例</span><span class="sxs-lookup"><span data-stu-id="d7dc7-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d7dc7-133">要求</span><span class="sxs-lookup"><span data-stu-id="d7dc7-133">Request</span></span>

<span data-ttu-id="d7dc7-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="d7dc7-135">応答</span><span class="sxs-lookup"><span data-stu-id="d7dc7-135">Response</span></span>

<span data-ttu-id="d7dc7-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-136">The following is an example of the response.</span></span> 

><span data-ttu-id="d7dc7-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d7dc7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
