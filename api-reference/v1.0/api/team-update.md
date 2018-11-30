---
title: チームを更新します。
description: 指定されたチームのプロパティを更新します。
ms.openlocfilehash: 27cbf8f571752a27fb68727fe2695a0250f5dc75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020533"
---
# <a name="update-team"></a><span data-ttu-id="06124-103">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="06124-103">Update team</span></span>



<span data-ttu-id="06124-104">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="06124-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06124-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06124-105">Permissions</span></span>
<span data-ttu-id="06124-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06124-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06124-108">Permission type</span></span>      | <span data-ttu-id="06124-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="06124-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06124-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06124-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06124-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06124-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="06124-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06124-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06124-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06124-113">Not supported.</span></span>    |
|<span data-ttu-id="06124-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06124-114">Application</span></span> | <span data-ttu-id="06124-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06124-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="06124-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06124-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06124-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06124-117">Request headers</span></span>
| <span data-ttu-id="06124-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06124-118">Header</span></span>       | <span data-ttu-id="06124-119">値</span><span class="sxs-lookup"><span data-stu-id="06124-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06124-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="06124-120">Authorization</span></span>  | <span data-ttu-id="06124-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="06124-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06124-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06124-123">Content-Type</span></span>  | <span data-ttu-id="06124-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06124-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06124-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="06124-125">Request body</span></span>
<span data-ttu-id="06124-126">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="06124-126">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="06124-127">応答</span><span class="sxs-lookup"><span data-stu-id="06124-127">Response</span></span>

<span data-ttu-id="06124-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="06124-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06124-129">例</span><span class="sxs-lookup"><span data-stu-id="06124-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="06124-130">要求</span><span class="sxs-lookup"><span data-stu-id="06124-130">Request</span></span>
<span data-ttu-id="06124-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06124-131">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="06124-132">応答</span><span class="sxs-lookup"><span data-stu-id="06124-132">Response</span></span>
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
