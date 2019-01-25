---
title: チームを更新します。
description: 指定されたチームのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f70c3212fb3297158f060d37f2f5906b62139a7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507615"
---
# <a name="update-team"></a><span data-ttu-id="ab918-103">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab918-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab918-104">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab918-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab918-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab918-105">Permissions</span></span>
<span data-ttu-id="ab918-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab918-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab918-108">Permission type</span></span>      | <span data-ttu-id="ab918-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab918-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab918-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab918-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab918-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab918-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab918-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab918-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab918-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab918-113">Not supported.</span></span>    |
|<span data-ttu-id="ab918-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab918-114">Application</span></span> | <span data-ttu-id="ab918-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab918-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="ab918-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="ab918-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ab918-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ab918-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab918-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab918-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ab918-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab918-119">Request headers</span></span>
| <span data-ttu-id="ab918-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab918-120">Header</span></span>       | <span data-ttu-id="ab918-121">値</span><span class="sxs-lookup"><span data-stu-id="ab918-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab918-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab918-122">Authorization</span></span>  | <span data-ttu-id="ab918-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab918-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab918-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab918-125">Content-Type</span></span>  | <span data-ttu-id="ab918-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab918-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab918-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab918-127">Request body</span></span>
<span data-ttu-id="ab918-128">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="ab918-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab918-129">応答</span><span class="sxs-lookup"><span data-stu-id="ab918-129">Response</span></span>

<span data-ttu-id="ab918-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ab918-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ab918-131">例</span><span class="sxs-lookup"><span data-stu-id="ab918-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab918-132">要求</span><span class="sxs-lookup"><span data-stu-id="ab918-132">Request</span></span>
<span data-ttu-id="ab918-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab918-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="ab918-134">応答</span><span class="sxs-lookup"><span data-stu-id="ab918-134">Response</span></span>
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
    "Error: /api-reference/beta/api/team-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
