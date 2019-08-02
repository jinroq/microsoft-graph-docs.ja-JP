---
title: チームの作成
description: 新しいチームを作成します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e8d6307999ab6db7b614e12ea6117245f473c29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990842"
---
# <a name="create-team"></a>チームを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい[チーム](../resources/team.md)を作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Group.ReadWrite.All                         |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                              |
| アプリケーション                            | Group.ReadWrite.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
| :------------ | :------------------------ |
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>要求本文

要求本文で、[team](../resources/team.md) オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功すると、この API は [teamsAsyncOperation](../resources/teamsasyncoperation.md) へのリンクを含む `202 Accepted` 応答を返します。

## <a name="examples"></a>例

### <a name="example-1-delegated-permissions"></a>例 1: 委任されたアクセス許可

最低限の要求の例を次に示します。 他のプロパティを省略することにより、クライアントは `template` で表される事前に定義されたテンプレートから暗黙的に既定値を使用します。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-2-application-permissions"></a>例 2:アプリケーションのアクセス許可

アプリケーションのアクセス許可を使用した最小限の要求の例を次に示します。 他のプロパティを省略することにより、クライアントは `template` で表される事前に定義されたテンプレートから暗黙的に既定値を使用します。 アプリケーションのアクセス許可で要求を発行する際には、[ユーザー](../resources/user.md)が `owners` コレクションで指定されている必要があります。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('userId')"
  ]
}
```

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a>例 3: 委任されたアクセス許可を使用して、複数のチャネル、インストールされたアプリ、および固定されたタブを持つチームを作成する

完全なペイロードの要求を次に示します。 クライアントは基本テンプレートの値を上書きして、`specialization` の検証規則で許容される範囲に配列値のアイテムを追加できます。 

#### <a name="request"></a>要求

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
    "discoverySettings": {
        "showInTeamsSearchAndSuggestions": true
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

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-4-create-a-team-from-group"></a>例 4: グループからチームを作成する

次の例では、**groupId** がわかっている場合に[グループ](../resources/group.md)から新しい[チーム](../resources/team.md)を作成する方法を示します。

この呼び出しに関する注意点:

* チームを作成するには、作成するグループに少なくとも 1 人の所有者がいる必要があります。 
* 作成されるチームは、グループの表示名、visibility、specialization、および所有者を常に継承します。 そのため、**group@odata.bind** プロパティを使用してこの呼び出しを行う場合、チームの **displayName**、**visibility**、**specialization**、または **owners@odata.bind** プロパティを含めるとエラーが発生します。
* グループが作成されて 15 分以上経っていない場合は、レプリケーションの遅延のためにチーム作成の呼び出しが失敗し、404 エラー コードが表示される可能性があります。 呼び出しと呼び出しの間に 10 秒の遅延を設けて、チーム作成の呼び出しを 3 回再試行することをお勧めします。


#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
}
```

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a>例 5: 複数のチャネル、インストールされたアプリ、および固定されたタブを持つチームをグループから作成する

以下に、拡張プロパティを持つ既存のグループを変換する要求を示します。これにより、複数のチャネル、インストールされたアプリ、固定されたタブを持つチームが作成されます。

サポートされているベース テンプレートとサポートされているプロパティの詳細については、「[Teams テンプレートの使用を開始する](https://docs.microsoft.com/ja-JP/MicrosoftTeams/get-started-with-teams-templates)」を参照してください。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a>例 6: 非標準のベース テンプレート タイプを使用してチームを作成する

ベース テンプレート タイプとは、Microsoft が特定の業界向けに作成した特別なテンプレートです。 多くの場合、これらのベース テンプレートにはストアでは入手できない独自のアプリおよび Microsoft Teams のテンプレートでまだ個別にサポートされていないチームのプロパティが含まれます。

非標準のベース テンプレートからチームを作成するには、要求本文で `template@odata.bind` プロパティを `standard` から使用する特定のベース テンプレートへのポイントに変更します。

サポートされているベース テンプレートの詳細については、「[Teams テンプレートの使用を開始する](https://docs.microsoft.com/ja-JP/MicrosoftTeams/get-started-with-teams-templates)」を参照してください。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a>例 7: 拡張プロパティを含んだ非標準のベース テンプレート タイプを使用してチームを作成する

ベース テンプレート タイプは追加のプロパティを使用して拡張することができ、既存のベース テンプレートを元にチームの追加の設定、チャンネル、アプリ、またはタブを設定してベース テンプレートを作成できます。

サポートされているベース テンプレートとサポートされているプロパティの詳細については、「[Teams テンプレートの使用を開始する](https://docs.microsoft.com/ja-JP/MicrosoftTeams/get-started-with-teams-templates)」を参照してください。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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

#### <a name="response"></a>応答

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a>関連項目

- 
  [使用可能なテンプレート](https://docs.microsoft.com/ja-JP/MicrosoftTeams/get-started-with-teams-templates)
- [Retail Teams テンプレートの使用を開始する](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [Healthcare Teams テンプレートの使用を開始する](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [チームを使用してグループを作成する](/graph/teams-create-group-and-team)
