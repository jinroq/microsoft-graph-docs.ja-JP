---
title: Microsoft Teams チームを含めたグループの作成
description: 'チームを含めてグループを作成するには、2 つの手順が必要です。 '
author: nkramer
ms.openlocfilehash: ea11d0ee7ee4e6e1d0bf6dc10ab8c9d064aa3610
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313889"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="0b455-103">Microsoft Teams チームを含めたグループの作成</span><span class="sxs-lookup"><span data-stu-id="0b455-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="0b455-104">[チーム](/graph/api/resources/team?view=graph-rest-beta)を含めて[グループ](/graph/api/resources/group?view=graph-rest-beta)を作成するには、2 つの手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b455-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="0b455-105">適切なプロパティを使用して[グループを作成します](/graph/api/group-post-groups?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="0b455-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="0b455-106">グループに[チームを追加](/graph/api/team-put-teams?view=graph-rest-beta)します。</span><span class="sxs-lookup"><span data-stu-id="0b455-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="0b455-107">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="0b455-107">Create a group</span></span>

<span data-ttu-id="0b455-108">チームを含めるには、次の例に示すプロパティの値を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b455-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="0b455-109">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="0b455-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="0b455-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="0b455-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="0b455-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="0b455-111">**securityEnabled** = false</span></span>

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

<span data-ttu-id="0b455-112">次の例に、応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0b455-112">The following example shows response.</span></span> 

><span data-ttu-id="0b455-113">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0b455-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="0b455-114">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0b455-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="0b455-115">グループにチームを追加する</span><span class="sxs-lookup"><span data-stu-id="0b455-115">Add a team to the group</span></span>

<span data-ttu-id="0b455-116">次に示すように、グループにチームを追加します。</span><span class="sxs-lookup"><span data-stu-id="0b455-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="0b455-117">次の例に、応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0b455-117">The following example shows the response.</span></span> 

><span data-ttu-id="0b455-118">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0b455-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="0b455-119">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0b455-119">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="0b455-120">作成したチームには、グループと同じ ID が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="0b455-120">The created team has the same ID as the group.</span></span>