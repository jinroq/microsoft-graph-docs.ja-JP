---
title: チームを作成します。
description: 新しいチームを作成します。
ms.openlocfilehash: 3f2fa97af217d6109f169e5b2ef75a0c71bde2e7
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210158"
---
# <a name="create-team"></a><span data-ttu-id="7b882-103">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b882-103">Create team</span></span>

> <span data-ttu-id="7b882-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b882-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b882-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b882-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b882-106">新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="7b882-106">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b882-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b882-107">Permissions</span></span>

<span data-ttu-id="7b882-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b882-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b882-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b882-110">Permission type</span></span>                        | <span data-ttu-id="7b882-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b882-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7b882-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b882-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b882-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b882-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="7b882-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b882-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b882-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b882-115">Not supported.</span></span>                              |
| <span data-ttu-id="7b882-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b882-116">Application</span></span>                            | <span data-ttu-id="7b882-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b882-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7b882-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b882-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="7b882-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b882-119">Request headers</span></span>

| <span data-ttu-id="7b882-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b882-120">Header</span></span>        | <span data-ttu-id="7b882-121">値</span><span class="sxs-lookup"><span data-stu-id="7b882-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7b882-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b882-122">Authorization</span></span> | <span data-ttu-id="7b882-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b882-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b882-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b882-125">Content-Type</span></span>  | <span data-ttu-id="7b882-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b882-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="7b882-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b882-127">Request body</span></span>

<span data-ttu-id="7b882-128">要求の本体で、[チーム](../resources/team.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b882-128">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b882-129">応答</span><span class="sxs-lookup"><span data-stu-id="7b882-129">Response</span></span>

<span data-ttu-id="7b882-130">かどうかは成功すると、この API を取得、 `202 Accepted` [teamsAsyncOperation](../resources/teamsasyncoperation.md)へのリンクを含む応答します。</span><span class="sxs-lookup"><span data-stu-id="7b882-130">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="7b882-131">例</span><span class="sxs-lookup"><span data-stu-id="7b882-131">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="7b882-132">委任されたアクセス許可の使用例</span><span class="sxs-lookup"><span data-stu-id="7b882-132">Example - delegated permissions</span></span>

<span data-ttu-id="7b882-133">ここでは、最低限の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b882-133">Here is an example of a minimal request.</span></span> <span data-ttu-id="7b882-134">その他のプロパティを省略することによって、クライアントが暗黙的にかかってによって表される定義済みのテンプレートから既定の設定`template`。</span><span class="sxs-lookup"><span data-stu-id="7b882-134">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="7b882-135">要求</span><span class="sxs-lookup"><span data-stu-id="7b882-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="7b882-136">応答</span><span class="sxs-lookup"><span data-stu-id="7b882-136">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="7b882-137">例 - インストールされているアプリにチームを作成、複数のチャネルを使用して、固定されたタブでアクセス許可を委任します。</span><span class="sxs-lookup"><span data-stu-id="7b882-137">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="7b882-138">フル ペイロードを使用して要求を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b882-138">Here is request with a full payload.</span></span> <span data-ttu-id="7b882-139">クライアントが基本テンプレート内の値をオーバーライドして追加の入力規則で許可されている範囲内の項目の配列の値を持つ、 `specialization`。</span><span class="sxs-lookup"><span data-stu-id="7b882-139">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="7b882-140">要求</span><span class="sxs-lookup"><span data-stu-id="7b882-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7b882-141">応答</span><span class="sxs-lookup"><span data-stu-id="7b882-141">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="7b882-142">アプリケーションのアクセス許可の使用例</span><span class="sxs-lookup"><span data-stu-id="7b882-142">Example - application permissions</span></span>

<span data-ttu-id="7b882-143">ここでは、アプリケーションのアクセス許可を使用して最小限の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b882-143">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="7b882-144">その他のプロパティを省略することによって、クライアントが暗黙的にかかってによって表される定義済みのテンプレートから既定の設定`template`。</span><span class="sxs-lookup"><span data-stu-id="7b882-144">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="7b882-145">アプリケーションのアクセス許可を持つ[ユーザー](../resources/user.md)は要求を発行する必要があるに指定する場合、`owners`コレクションです。</span><span class="sxs-lookup"><span data-stu-id="7b882-145">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="7b882-146">要求</span><span class="sxs-lookup"><span data-stu-id="7b882-146">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7b882-147">応答</span><span class="sxs-lookup"><span data-stu-id="7b882-147">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="7b882-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b882-148">See also</span></span>

- [<span data-ttu-id="7b882-149">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="7b882-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
