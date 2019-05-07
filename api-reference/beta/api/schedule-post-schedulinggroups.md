---
title: schedulingGroup を作成する
description: 新しい schedulingGroup を作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7d1e2ce97233dc830da41fa895de7356524e60a4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638992"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="1d018-103">schedulingGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="1d018-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d018-104">新しい[schedulingGroup](../resources/schedulinggroup.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="1d018-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d018-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d018-105">Permissions</span></span>

<span data-ttu-id="1d018-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d018-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d018-108">Permission type</span></span>      | <span data-ttu-id="1d018-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d018-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d018-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d018-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d018-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d018-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d018-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d018-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d018-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d018-113">Not supported.</span></span>    |
|<span data-ttu-id="1d018-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d018-114">Application</span></span> | <span data-ttu-id="1d018-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d018-115">Not supported.</span></span> |

> <span data-ttu-id="1d018-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1d018-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1d018-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1d018-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d018-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d018-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="1d018-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d018-119">Request headers</span></span>

| <span data-ttu-id="1d018-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d018-120">Header</span></span>       | <span data-ttu-id="1d018-121">値</span><span class="sxs-lookup"><span data-stu-id="1d018-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d018-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d018-122">Authorization</span></span>  | <span data-ttu-id="1d018-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d018-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d018-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d018-125">Content-Type</span></span>  | <span data-ttu-id="1d018-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d018-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="1d018-127">応答</span><span class="sxs-lookup"><span data-stu-id="1d018-127">Response</span></span>

<span data-ttu-id="1d018-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[schedulingGroup](../resources/schedulinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d018-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d018-129">例</span><span class="sxs-lookup"><span data-stu-id="1d018-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1d018-130">要求</span><span class="sxs-lookup"><span data-stu-id="1d018-130">Request</span></span>

<span data-ttu-id="1d018-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d018-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="1d018-132">応答</span><span class="sxs-lookup"><span data-stu-id="1d018-132">Response</span></span>

<span data-ttu-id="1d018-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d018-133">The following is an example of the response.</span></span> 

><span data-ttu-id="1d018-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1d018-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1d018-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1d018-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1d018-137">Visual</span><span class="sxs-lookup"><span data-stu-id="1d018-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-post-schedulinggroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d018-138">Java</span><span class="sxs-lookup"><span data-stu-id="1d018-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-post-schedulinggroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-schedulinggroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-post-schedulinggroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
