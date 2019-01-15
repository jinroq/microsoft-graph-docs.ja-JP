---
title: チームを更新します。
description: 指定されたチームのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6dd8e38261cb2e64c3717ea3bee26ca96bd8958
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016619"
---
# <a name="update-team"></a><span data-ttu-id="481ee-103">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="481ee-103">Update team</span></span>



<span data-ttu-id="481ee-104">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="481ee-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="481ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="481ee-105">Permissions</span></span>
<span data-ttu-id="481ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="481ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="481ee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="481ee-108">Permission type</span></span>      | <span data-ttu-id="481ee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="481ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="481ee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="481ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="481ee-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481ee-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="481ee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="481ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="481ee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="481ee-113">Not supported.</span></span>    |
|<span data-ttu-id="481ee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="481ee-114">Application</span></span> | <span data-ttu-id="481ee-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481ee-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="481ee-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="481ee-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="481ee-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="481ee-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="481ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="481ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="481ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="481ee-119">Request headers</span></span>
| <span data-ttu-id="481ee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="481ee-120">Header</span></span>       | <span data-ttu-id="481ee-121">値</span><span class="sxs-lookup"><span data-stu-id="481ee-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="481ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="481ee-122">Authorization</span></span>  | <span data-ttu-id="481ee-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="481ee-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="481ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="481ee-125">Content-Type</span></span>  | <span data-ttu-id="481ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="481ee-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="481ee-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="481ee-127">Request body</span></span>
<span data-ttu-id="481ee-128">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="481ee-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="481ee-129">応答</span><span class="sxs-lookup"><span data-stu-id="481ee-129">Response</span></span>

<span data-ttu-id="481ee-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="481ee-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="481ee-131">例</span><span class="sxs-lookup"><span data-stu-id="481ee-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="481ee-132">要求</span><span class="sxs-lookup"><span data-stu-id="481ee-132">Request</span></span>
<span data-ttu-id="481ee-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="481ee-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
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
#### <a name="response"></a><span data-ttu-id="481ee-134">応答</span><span class="sxs-lookup"><span data-stu-id="481ee-134">Response</span></span>
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
