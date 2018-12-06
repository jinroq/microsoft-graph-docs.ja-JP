---
title: 組織の Microsoft Teams 内のすべてのチームのリストを作成する
description: 'すべてのチームのリストを作成する方法 '
ms.openlocfilehash: 2a9dbaa1fc9a02897870865295fd8d0dac9266a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092471"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a><span data-ttu-id="19477-103">組織の Microsoft Teams 内のすべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="19477-103">List all teams in Microsoft Teams for an organization</span></span>

<span data-ttu-id="19477-104">組織 (テナント) 内のすべての[チーム](/graph/api/resources/team?view=graph-rest-beta)のリストを作成するには、チームを所有するグループをすべて割り出し、各チームの情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="19477-104">To list all [teams](/graph/api/resources/team?view=graph-rest-beta) in an organization (tenant), you find all groups that have teams, and then get information for each team.</span></span>

## <a name="get-a-list-of-groups"></a><span data-ttu-id="19477-105">グループのリストを取得する</span><span class="sxs-lookup"><span data-stu-id="19477-105">Gets a list of groups.</span></span>

<span data-ttu-id="19477-106">組織内の、チームを所有するすべての[グループ](/graph/api/resources/group?view=graph-rest-beta)のリストを取得するには、[すべてのグループのリスト](/graph/api/group-list?view=graph-rest-beta)を取得し、その中から "Team" を含む **resourceProvisioningOptions** プロパティを持つグループをプログラムで検索します。</span><span class="sxs-lookup"><span data-stu-id="19477-106">To get a list of all [groups](/graph/api/resources/group?view=graph-rest-beta) in the organization that have teams, get a [list of all groups](/graph/api/group-list?view=graph-rest-beta) and then in code find the ones that have a **resourceProvisioningOptions** property that contains "Team".</span></span>
<span data-ttu-id="19477-107">グループはサイズの大きいオブジェクトであるため、$select のみを使用して対象のグループのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="19477-107">Since groups are large objects, use $select to only get the properties of the group you care about.</span></span>

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> <span data-ttu-id="19477-108">**注**: 使用されていない古いチームには、resourceProvisioningOptions が設定されていないチームがあります。</span><span class="sxs-lookup"><span data-stu-id="19477-108">**Note**: Certain unused old teams will not have resourceProvisioningOptions set.</span></span> <span data-ttu-id="19477-109">詳細については、「[既知の問題](known-issues.md#missing-teams-in-list-all-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19477-109">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="19477-110">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19477-110">The following is an example of the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "00e897b1-70ba-4cb9-9126-fd5f95c4bb78",
            "resourceProvisioningOptions": []
        },
        {
            "id": "00f6e045-f884-4359-a617-d459ee626862",
            "resourceProvisioningOptions": [
                "Team"
            ]
        }
    ]
}
```

## <a name="get-a-list-of-groups-using-beta-apis"></a><span data-ttu-id="19477-111">ベータ版の API を使用してグループのリストを取得する</span><span class="sxs-lookup"><span data-stu-id="19477-111">Get a list of groups using beta APIs</span></span>

<span data-ttu-id="19477-112">ベータ版の API を使用すると、$filter を使用して、チームを所有するグループのみ返すことができるようになります。</span><span class="sxs-lookup"><span data-stu-id="19477-112">Using the beta APIs, you can use $filter to return only the groups that have teams.</span></span>

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> <span data-ttu-id="19477-113">**Note**: /groups に対して $filter を使用できるのは、ベータ版エンドポイントのみとなります。</span><span class="sxs-lookup"><span data-stu-id="19477-113">**Note**: $filter on /groups is only available through the beta endpoint.</span></span> <span data-ttu-id="19477-114">resourceProvisioningOptions は、v1.0 とベータ版で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="19477-114">resourceProvisioningOptions is available in v1.0 and beta.</span></span>

> <span data-ttu-id="19477-115">**注**: 使用されていない古いチームの一部は、リストに含まれません。</span><span class="sxs-lookup"><span data-stu-id="19477-115">**Note**: Certain unused old teams will not be listed.</span></span> <span data-ttu-id="19477-116">詳細については、「[既知の問題](known-issues.md#missing-teams-in-list-all-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19477-116">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="19477-117">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19477-117">The following is an example of the response.</span></span> 

><span data-ttu-id="19477-118">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="19477-118">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="19477-119">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19477-119">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
    "value": [
        {
            "id": "02bd9fd6-8f93-4758-87c3-1fb73740a315",
            "description": "Welcome to the HR Taskforce team.",
            "displayName": "HR Taskforce",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "HRTaskforce",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private",
        },
        {
            "id": "8090c93e-ba7c-433e-9f39-08c7ba07c0b3",
            "description": "Welcome to the team that we've assembled to launch our product.",
            "displayName": "X1050 Launch Team",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "X1050LaunchTeam",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private",
        }
    ]
}
```

## <a name="get-team-information-for-a-group"></a><span data-ttu-id="19477-120">グループのチームの情報を入手する</span><span class="sxs-lookup"><span data-stu-id="19477-120">Get team information for a group</span></span>

<span data-ttu-id="19477-121">特定のグループ内のチームの情報を取得するには、[get team](/graph/api/team-get?view=graph-rest-beta) API を呼び出し、グループ ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="19477-121">To get team information for the team in a particular group, call the [get team](/graph/api/team-get?view=graph-rest-beta) API and include the group ID.</span></span>

```http
GET /teams/{group-id}
```

<span data-ttu-id="19477-122">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="19477-122">The following example shows the response.</span></span>

><span data-ttu-id="19477-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19477-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="19477-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="19477-125">See also</span></span>

- [<span data-ttu-id="19477-126">参加チームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="19477-126">List joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [<span data-ttu-id="19477-127">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="19477-127">List groups</span></span>](/graph/api/group-list?view=graph-rest-beta)
