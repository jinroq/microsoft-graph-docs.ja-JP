---
title: チームを更新します。
description: 指定されたチームのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb882a31916d31744d57cdc0ef3d2a161361b628
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925988"
---
# <a name="update-team"></a><span data-ttu-id="61f77-103">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="61f77-103">Update team</span></span>

> <span data-ttu-id="61f77-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61f77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61f77-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61f77-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61f77-106">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="61f77-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61f77-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="61f77-107">Permissions</span></span>
<span data-ttu-id="61f77-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61f77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61f77-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61f77-110">Permission type</span></span>      | <span data-ttu-id="61f77-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="61f77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61f77-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61f77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61f77-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61f77-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="61f77-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61f77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61f77-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61f77-115">Not supported.</span></span>    |
|<span data-ttu-id="61f77-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61f77-116">Application</span></span> | <span data-ttu-id="61f77-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61f77-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="61f77-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="61f77-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="61f77-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="61f77-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="61f77-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61f77-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="61f77-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61f77-121">Request headers</span></span>
| <span data-ttu-id="61f77-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61f77-122">Header</span></span>       | <span data-ttu-id="61f77-123">値</span><span class="sxs-lookup"><span data-stu-id="61f77-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61f77-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="61f77-124">Authorization</span></span>  | <span data-ttu-id="61f77-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="61f77-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="61f77-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61f77-127">Content-Type</span></span>  | <span data-ttu-id="61f77-128">application/json</span><span class="sxs-lookup"><span data-stu-id="61f77-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61f77-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="61f77-129">Request body</span></span>
<span data-ttu-id="61f77-130">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="61f77-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="61f77-131">応答</span><span class="sxs-lookup"><span data-stu-id="61f77-131">Response</span></span>

<span data-ttu-id="61f77-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="61f77-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61f77-133">例</span><span class="sxs-lookup"><span data-stu-id="61f77-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="61f77-134">要求</span><span class="sxs-lookup"><span data-stu-id="61f77-134">Request</span></span>
<span data-ttu-id="61f77-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61f77-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="61f77-136">応答</span><span class="sxs-lookup"><span data-stu-id="61f77-136">Response</span></span>
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
