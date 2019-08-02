---
title: グループからチームを作成する
description: グループから新しいチームを作成します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b4b40190678813233c0755463e3344c21579913c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990828"
---
# <a name="create-team-from-group"></a><span data-ttu-id="f6dc4-103">グループからチームを作成する</span><span class="sxs-lookup"><span data-stu-id="f6dc4-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> <span data-ttu-id="f6dc4-104">この API は、[[チームを作成する](../api/team-post.md)] を優先して廃止中であり、2019 年末までに削除されます。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-104">This API is in the process of being depracated in favor of [Create team](../api/team-post.md), and will be removed by the end of 2019.</span></span> <span data-ttu-id="f6dc4-105">グループからチームを作成する方法の詳細については、「[チームを作成する](../api/team-post.md)」の例の 4 と 5 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-105">For details about how to create a team from a group, see examples 4 and 5 in [Create team](../api/team-post.md).</span></span>

<span data-ttu-id="f6dc4-106">[グループ](../resources/group.md)から新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-106">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="f6dc4-107">チームを作成するために、グループには少なくとも 1 人の所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="f6dc4-108">グループが作成されて 15 分以上経っていない場合は、レプリケーションの遅延のためにチーム作成の呼び出しが失敗し、404 エラー コードが表示される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="f6dc4-109">呼び出しと呼び出しの間に 10 秒の遅延を設けて、チーム作成の呼び出しを 3 回再試行するパターンをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6dc4-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6dc4-110">Permissions</span></span>

<span data-ttu-id="f6dc4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6dc4-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6dc4-113">Permission type</span></span>      | <span data-ttu-id="f6dc4-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6dc4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6dc4-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6dc4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f6dc4-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6dc4-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6dc4-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6dc4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6dc4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-118">Not supported.</span></span>    |
|<span data-ttu-id="f6dc4-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6dc4-119">Application</span></span> | <span data-ttu-id="f6dc4-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6dc4-120">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="f6dc4-121">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f6dc4-122">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-122">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6dc4-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6dc4-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="f6dc4-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6dc4-124">Request headers</span></span>

| <span data-ttu-id="f6dc4-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6dc4-125">Header</span></span>       | <span data-ttu-id="f6dc4-126">値</span><span class="sxs-lookup"><span data-stu-id="f6dc4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6dc4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6dc4-127">Authorization</span></span>  | <span data-ttu-id="f6dc4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6dc4-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6dc4-130">Content-Type</span></span>  | <span data-ttu-id="f6dc4-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f6dc4-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6dc4-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6dc4-132">Request body</span></span>

<span data-ttu-id="f6dc4-133">要求本文で、[team](../resources/team.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-133">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f6dc4-134">応答</span><span class="sxs-lookup"><span data-stu-id="f6dc4-134">Response</span></span>

<span data-ttu-id="f6dc4-135">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [team](../resources/team.md) オブジェクトを返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-135">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6dc4-136">例</span><span class="sxs-lookup"><span data-stu-id="f6dc4-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f6dc4-137">要求</span><span class="sxs-lookup"><span data-stu-id="f6dc4-137">Request</span></span>

<span data-ttu-id="f6dc4-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6dc4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6dc4-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6dc4-140">C#</span><span class="sxs-lookup"><span data-stu-id="f6dc4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6dc4-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6dc4-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6dc4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6dc4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f6dc4-143">Java</span><span class="sxs-lookup"><span data-stu-id="f6dc4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6dc4-144">応答</span><span class="sxs-lookup"><span data-stu-id="f6dc4-144">Response</span></span>

<span data-ttu-id="f6dc4-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-145">The following is an example of the response.</span></span> 

><span data-ttu-id="f6dc4-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f6dc4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
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
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="f6dc4-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6dc4-148">See also</span></span>

- [<span data-ttu-id="f6dc4-149">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="f6dc4-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
