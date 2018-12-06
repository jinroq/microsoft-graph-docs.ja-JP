---
title: マイクロソフトのチームのチームのグループを作成
description: 'チームを含むグループを作成するには、2 つの手順が含まれます。 '
ms.openlocfilehash: 530b3625a1aa1d020bff841196e3b83a2eb99a4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092415"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="3ec02-103">マイクロソフトのチームのチームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="3ec02-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="3ec02-104">[チーム](/graph/api/resources/team?view=graph-rest-beta)を含む[グループ](/graph/api/resources/group?view=graph-rest-beta)を作成するには、2 つの手順が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3ec02-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="3ec02-105">右のプロパティを持つ[グループの作成](/graph/api/group-post-groups?view=graph-rest-beta)をします。</span><span class="sxs-lookup"><span data-stu-id="3ec02-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="3ec02-106">グループに[チームを追加](/graph/api/team-put-teams?view=graph-rest-beta)します。</span><span class="sxs-lookup"><span data-stu-id="3ec02-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="3ec02-107">グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="3ec02-107">Create a group</span></span>

<span data-ttu-id="3ec02-108">チームが含まれて、する必要があります、次のプロパティ値を設定する例を次に示すように。</span><span class="sxs-lookup"><span data-stu-id="3ec02-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="3ec02-109">**groupTypes** = {「統合」。</span><span class="sxs-lookup"><span data-stu-id="3ec02-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="3ec02-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="3ec02-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="3ec02-111">**セキュリティの有効化**= false</span><span class="sxs-lookup"><span data-stu-id="3ec02-111">**securityEnabled** = false</span></span>

```http
POST /groups
{
    "displayName":"Flight 157",
    "mailNickname":"flight157",
    "description":"Everything about flight 157",
    "visibility":"Private",
    "groupTypes":["Unified"],
    "mailEnabled":true,
    "securityEnabled":false,
    "members@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
        "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
    ],
    "owners@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
    ]
}
```

<span data-ttu-id="3ec02-112">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3ec02-112">The following example shows response.</span></span> 

><span data-ttu-id="3ec02-113">**注:** 応答オブジェクトが示すようには、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3ec02-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="3ec02-114">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ec02-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="3ec02-115">チームをグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="3ec02-115">Add a team to the group</span></span>

<span data-ttu-id="3ec02-116">ように、グループ、チームを追加します。</span><span class="sxs-lookup"><span data-stu-id="3ec02-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="3ec02-117">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ec02-117">The following example shows the response.</span></span> 

><span data-ttu-id="3ec02-118">**注:** 応答オブジェクトが示すようには、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3ec02-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="3ec02-119">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ec02-119">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
    "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
    "webUrl" : "https://example.com",
    "isArchived" : null,
    "memberSettings" : { },
    "guestSettings" : { },
    "messagingSettings" : { },
    "funSettings" : {}
}
```

<span data-ttu-id="3ec02-120">作成されたチームには、グループと同じ ID があります。</span><span class="sxs-lookup"><span data-stu-id="3ec02-120">The created team has the same ID as the group.</span></span>
