---
title: チームを更新する
description: 指定されたチームのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 325c5d9813794a57b59de6caaaea359d3f51f830
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421331"
---
# <a name="update-team"></a><span data-ttu-id="48280-103">チームを更新する</span><span class="sxs-lookup"><span data-stu-id="48280-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48280-104">指定した[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="48280-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48280-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48280-105">Permissions</span></span>
<span data-ttu-id="48280-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48280-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48280-108">Permission type</span></span>      | <span data-ttu-id="48280-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48280-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48280-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48280-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48280-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48280-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48280-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48280-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48280-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48280-113">Not supported.</span></span>    |
|<span data-ttu-id="48280-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48280-114">Application</span></span> | <span data-ttu-id="48280-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48280-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="48280-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="48280-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="48280-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="48280-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="48280-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48280-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="48280-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48280-119">Request headers</span></span>
| <span data-ttu-id="48280-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48280-120">Header</span></span>       | <span data-ttu-id="48280-121">値</span><span class="sxs-lookup"><span data-stu-id="48280-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48280-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48280-122">Authorization</span></span>  | <span data-ttu-id="48280-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48280-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48280-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48280-125">Content-Type</span></span>  | <span data-ttu-id="48280-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48280-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48280-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="48280-127">Request body</span></span>
<span data-ttu-id="48280-128">要求本文で、 [team](../resources/team.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="48280-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48280-129">応答</span><span class="sxs-lookup"><span data-stu-id="48280-129">Response</span></span>

<span data-ttu-id="48280-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="48280-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48280-131">例</span><span class="sxs-lookup"><span data-stu-id="48280-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="48280-132">要求</span><span class="sxs-lookup"><span data-stu-id="48280-132">Request</span></span>
<span data-ttu-id="48280-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48280-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48280-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="48280-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48280-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48280-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="48280-136">C#</span><span class="sxs-lookup"><span data-stu-id="48280-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48280-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="48280-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="48280-138">応答</span><span class="sxs-lookup"><span data-stu-id="48280-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
