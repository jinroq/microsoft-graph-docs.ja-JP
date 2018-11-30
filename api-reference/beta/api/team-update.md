---
title: チームを更新します。
description: 指定されたチームのプロパティを更新します。
ms.openlocfilehash: 9d07fd687facc96c1bc4a93c37cb492b321518e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067744"
---
# <a name="update-team"></a><span data-ttu-id="69be9-103">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="69be9-103">Update team</span></span>

> <span data-ttu-id="69be9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="69be9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69be9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69be9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69be9-106">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="69be9-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69be9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69be9-107">Permissions</span></span>
<span data-ttu-id="69be9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69be9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69be9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69be9-110">Permission type</span></span>      | <span data-ttu-id="69be9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69be9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69be9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69be9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69be9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69be9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69be9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69be9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69be9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69be9-115">Not supported.</span></span>    |
|<span data-ttu-id="69be9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69be9-116">Application</span></span> | <span data-ttu-id="69be9-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69be9-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="69be9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69be9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="69be9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69be9-119">Request headers</span></span>
| <span data-ttu-id="69be9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69be9-120">Header</span></span>       | <span data-ttu-id="69be9-121">値</span><span class="sxs-lookup"><span data-stu-id="69be9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69be9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69be9-122">Authorization</span></span>  | <span data-ttu-id="69be9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69be9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="69be9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69be9-125">Content-Type</span></span>  | <span data-ttu-id="69be9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69be9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69be9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="69be9-127">Request body</span></span>
<span data-ttu-id="69be9-128">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="69be9-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="69be9-129">応答</span><span class="sxs-lookup"><span data-stu-id="69be9-129">Response</span></span>

<span data-ttu-id="69be9-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="69be9-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="69be9-131">例</span><span class="sxs-lookup"><span data-stu-id="69be9-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69be9-132">要求</span><span class="sxs-lookup"><span data-stu-id="69be9-132">Request</span></span>
<span data-ttu-id="69be9-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="69be9-133">The following is an example of the request.</span></span>
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
  }
}
```
#### <a name="response"></a><span data-ttu-id="69be9-134">応答</span><span class="sxs-lookup"><span data-stu-id="69be9-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
