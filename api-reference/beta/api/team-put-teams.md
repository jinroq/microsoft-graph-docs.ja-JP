---
title: グループからチームを作成する
description: グループから新しいチームを作成します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a28036cfb253405fab55eca80fa2b0a17232a96c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544632"
---
# <a name="create-team-from-group"></a><span data-ttu-id="ad949-103">グループからチームを作成する</span><span class="sxs-lookup"><span data-stu-id="ad949-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad949-104">[グループ](../resources/group.md)から新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="ad949-104">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="ad949-105">チームを作成するために、グループには少なくとも 1 人の所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad949-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="ad949-106">グループが作成されて 15 分以上経っていない場合は、レプリケーションの遅延のためにチーム作成の呼び出しが失敗し、404 エラー コードが表示される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ad949-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="ad949-107">呼び出しと呼び出しの間に 10 秒の遅延を設けて、チーム作成の呼び出しを 3 回再試行するパターンをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ad949-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad949-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad949-108">Permissions</span></span>

<span data-ttu-id="ad949-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad949-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad949-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad949-111">Permission type</span></span>      | <span data-ttu-id="ad949-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad949-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad949-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad949-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ad949-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad949-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad949-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad949-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad949-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad949-116">Not supported.</span></span>    |
|<span data-ttu-id="ad949-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad949-117">Application</span></span> | <span data-ttu-id="ad949-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad949-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="ad949-119">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad949-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ad949-120">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ad949-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ad949-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad949-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="ad949-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad949-122">Request headers</span></span>

| <span data-ttu-id="ad949-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad949-123">Header</span></span>       | <span data-ttu-id="ad949-124">値</span><span class="sxs-lookup"><span data-stu-id="ad949-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad949-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad949-125">Authorization</span></span>  | <span data-ttu-id="ad949-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad949-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad949-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad949-128">Content-Type</span></span>  | <span data-ttu-id="ad949-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ad949-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad949-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad949-130">Request body</span></span>

<span data-ttu-id="ad949-131">要求本文で、[team](../resources/team.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad949-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad949-132">応答</span><span class="sxs-lookup"><span data-stu-id="ad949-132">Response</span></span>

<span data-ttu-id="ad949-133">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [team](../resources/team.md) オブジェクトを返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad949-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad949-134">例</span><span class="sxs-lookup"><span data-stu-id="ad949-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ad949-135">要求</span><span class="sxs-lookup"><span data-stu-id="ad949-135">Request</span></span>

<span data-ttu-id="ad949-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad949-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/beta/groups/{id}/team
Content-type: application/json

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

#### <a name="response"></a><span data-ttu-id="ad949-137">応答</span><span class="sxs-lookup"><span data-stu-id="ad949-137">Response</span></span>

<span data-ttu-id="ad949-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad949-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ad949-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ad949-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-teams.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="ad949-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="ad949-141">See also</span></span>

- [<span data-ttu-id="ad949-142">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="ad949-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
