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
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>マイクロソフトのチームのチームのグループを作成

[チーム](/graph/api/resources/team?view=graph-rest-beta)を含む[グループ](/graph/api/resources/group?view=graph-rest-beta)を作成するには、2 つの手順が含まれます。 

- 右のプロパティを持つ[グループの作成](/graph/api/group-post-groups?view=graph-rest-beta)をします。
- グループに[チームを追加](/graph/api/team-put-teams?view=graph-rest-beta)します。

## <a name="create-a-group"></a>グループを作成します。

チームが含まれて、する必要があります、次のプロパティ値を設定する例を次に示すように。

- **groupTypes** = {「統合」。 
- **mailEnabled** = true
- **セキュリティの有効化**= false

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

応答の例を次に示します。 

>**注:** 応答オブジェクトが示すようには、読みやすさの短縮される可能性があります。 実際の呼び出しではすべてのプロパティが返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>チームをグループに追加します。

ように、グループ、チームを追加します。

```http
PUT /groups/{id}/team
{ }
```

次の例は応答を示しています。 

>**注:** 応答オブジェクトが示すようには、読みやすさの短縮される可能性があります。 実際の呼び出しではすべてのプロパティが返されます。

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

作成されたチームには、グループと同じ ID があります。
