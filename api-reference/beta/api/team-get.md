---
title: チームを取得する
description: 指定したチームのプロパティとリレーションシップを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a9da6ea1bc1570f40fe4159d9c62951fca539cb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544584"
---
# <a name="get-team"></a><span data-ttu-id="15de2-103">チームを取得する</span><span class="sxs-lookup"><span data-stu-id="15de2-103">Get team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15de2-104">指定した[チーム](../resources/team.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="15de2-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15de2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15de2-105">Permissions</span></span>
<span data-ttu-id="15de2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15de2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15de2-108">Permission type</span></span>      | <span data-ttu-id="15de2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15de2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15de2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15de2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15de2-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15de2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="15de2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15de2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15de2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15de2-113">Not supported.</span></span>    |
|<span data-ttu-id="15de2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15de2-114">Application</span></span> | <span data-ttu-id="15de2-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15de2-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="15de2-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15de2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="15de2-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="15de2-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="15de2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15de2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15de2-119">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="15de2-119">Optional query parameters</span></span>
<span data-ttu-id="15de2-120">このメソッドは、応答をカスタマイズするための $select and $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15de2-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15de2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15de2-121">Request headers</span></span>
| <span data-ttu-id="15de2-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15de2-122">Header</span></span>       | <span data-ttu-id="15de2-123">値</span><span class="sxs-lookup"><span data-stu-id="15de2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15de2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15de2-124">Authorization</span></span>  | <span data-ttu-id="15de2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15de2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15de2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="15de2-127">Request body</span></span>
<span data-ttu-id="15de2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15de2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15de2-129">応答</span><span class="sxs-lookup"><span data-stu-id="15de2-129">Response</span></span>

<span data-ttu-id="15de2-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [team](../resources/team.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15de2-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15de2-131">例</span><span class="sxs-lookup"><span data-stu-id="15de2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="15de2-132">要求</span><span class="sxs-lookup"><span data-stu-id="15de2-132">Request</span></span>
<span data-ttu-id="15de2-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15de2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="15de2-134">応答</span><span class="sxs-lookup"><span data-stu-id="15de2-134">Response</span></span>
<span data-ttu-id="15de2-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15de2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="15de2-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="15de2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
