---
title: チームの作成
description: 新しいチームを作成します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3e901225f5a8f94abb61a6b4052b0db2d47865c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519613"
---
# <a name="create-team"></a><span data-ttu-id="cdb86-103">チームを作成する</span><span class="sxs-lookup"><span data-stu-id="cdb86-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdb86-104">新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdb86-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdb86-105">Permissions</span></span>

<span data-ttu-id="cdb86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdb86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdb86-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdb86-108">Permission type</span></span>                        | <span data-ttu-id="cdb86-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdb86-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cdb86-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdb86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdb86-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdb86-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="cdb86-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdb86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdb86-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdb86-113">Not supported.</span></span>                              |
| <span data-ttu-id="cdb86-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdb86-114">Application</span></span>                            | <span data-ttu-id="cdb86-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdb86-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cdb86-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdb86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="cdb86-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdb86-117">Request headers</span></span>

| <span data-ttu-id="cdb86-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdb86-118">Header</span></span>        | <span data-ttu-id="cdb86-119">値</span><span class="sxs-lookup"><span data-stu-id="cdb86-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cdb86-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdb86-120">Authorization</span></span> | <span data-ttu-id="cdb86-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cdb86-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdb86-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdb86-123">Content-Type</span></span>  | <span data-ttu-id="cdb86-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdb86-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="cdb86-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdb86-125">Request body</span></span>

<span data-ttu-id="cdb86-126">要求本文で、[team](../resources/team.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-126">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cdb86-127">応答</span><span class="sxs-lookup"><span data-stu-id="cdb86-127">Response</span></span>

<span data-ttu-id="cdb86-128">成功すると、この API は [teamsAsyncOperation](../resources/teamsasyncoperation.md) へのリンクを含む `202 Accepted` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="cdb86-129">例</span><span class="sxs-lookup"><span data-stu-id="cdb86-129">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="cdb86-130">例: 委任されたアクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdb86-130">Example - delegated permissions</span></span>

<span data-ttu-id="cdb86-131">最低限の要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-131">Here is an example of a minimal request.</span></span> <span data-ttu-id="cdb86-132">他のプロパティを省略することにより、クライアントは `template` で表される事前に定義されたテンプレートから暗黙的に既定値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="cdb86-133">要求</span><span class="sxs-lookup"><span data-stu-id="cdb86-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="cdb86-134">応答</span><span class="sxs-lookup"><span data-stu-id="cdb86-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="cdb86-135">例: 委任されたアクセス許可を使用して、インストールされたアプリと固定されたタブによる複数のチャネルを持つチームを作成します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-135">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="cdb86-136">完全なペイロードの要求を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-136">Here is request with a full payload.</span></span> <span data-ttu-id="cdb86-137">クライアントは基本テンプレートの値を上書きして、`specialization` の検証規則で許容される範囲に配列値のアイテムを追加できます。</span><span class="sxs-lookup"><span data-stu-id="cdb86-137">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="cdb86-138">要求</span><span class="sxs-lookup"><span data-stu-id="cdb86-138">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="cdb86-139">応答</span><span class="sxs-lookup"><span data-stu-id="cdb86-139">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="cdb86-140">例: アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdb86-140">Example - application permissions</span></span>

<span data-ttu-id="cdb86-141">アプリケーションのアクセス許可を使用した最小限の要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-141">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="cdb86-142">他のプロパティを省略することにより、クライアントは `template` で表される事前に定義されたテンプレートから暗黙的に既定値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cdb86-142">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="cdb86-143">アプリケーションのアクセス許可で要求を発行する際には、[ユーザー](../resources/user.md)が `owners` コレクションで指定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cdb86-143">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="cdb86-144">要求</span><span class="sxs-lookup"><span data-stu-id="cdb86-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="cdb86-145">応答</span><span class="sxs-lookup"><span data-stu-id="cdb86-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="cdb86-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="cdb86-146">See also</span></span>

- [<span data-ttu-id="cdb86-147">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="cdb86-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/team-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
