---
title: 組織の Microsoft Teams 内のすべてのチームのリストを作成する
description: 'すべてのチームのリストを作成する方法 '
ms.openlocfilehash: 2a9dbaa1fc9a02897870865295fd8d0dac9266a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092471"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>組織の Microsoft Teams 内のすべてのチームのリストを作成する

組織 (テナント) 内のすべての[チーム](/graph/api/resources/team?view=graph-rest-beta)のリストを作成するには、チームを所有するグループをすべて割り出し、各チームの情報を取得します。

## <a name="get-a-list-of-groups"></a>グループのリストを取得する

組織内の、チームを所有するすべての[グループ](/graph/api/resources/group?view=graph-rest-beta)のリストを取得するには、[すべてのグループのリスト](/graph/api/group-list?view=graph-rest-beta)を取得し、その中から "Team" を含む **resourceProvisioningOptions** プロパティを持つグループをプログラムで検索します。
グループはサイズの大きいオブジェクトであるため、$select のみを使用して対象のグループのプロパティを取得します。

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> **注**: 使用されていない古いチームには、resourceProvisioningOptions が設定されていないチームがあります。 詳細については、「[既知の問題](known-issues.md#missing-teams-in-list-all-teams)」を参照してください。

応答の例を次に示します。 

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

## <a name="get-a-list-of-groups-using-beta-apis"></a>ベータ版の API を使用してグループのリストを取得する

ベータ版の API を使用すると、$filter を使用して、チームを所有するグループのみ返すことができるようになります。

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> **Note**: /groups に対して $filter を使用できるのは、ベータ版エンドポイントのみとなります。 resourceProvisioningOptions は、v1.0 とベータ版で利用可能です。

> **注**: 使用されていない古いチームの一部は、リストに含まれません。 詳細については、「[既知の問題](known-issues.md#missing-teams-in-list-all-teams)」を参照してください。

応答の例を次に示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

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

## <a name="get-team-information-for-a-group"></a>グループのチームの情報を入手する

特定のグループ内のチームの情報を取得するには、[get team](/graph/api/team-get?view=graph-rest-beta) API を呼び出し、グループ ID を指定します。

```http
GET /teams/{group-id}
```

次の例は応答を示しています。

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
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

## <a name="see-also"></a>関連項目

- [参加チームのリストを作成する](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [グループを一覧表示する](/graph/api/group-list?view=graph-rest-beta)
