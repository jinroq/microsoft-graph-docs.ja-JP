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
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>Microsoft Teams チームを含めたグループの作成

[チーム](/graph/api/resources/team?view=graph-rest-beta)を含めて[グループ](/graph/api/resources/group?view=graph-rest-beta)を作成するには、2 つの手順が必要です。 

- 適切なプロパティを使用して[グループを作成します](/graph/api/group-post-groups?view=graph-rest-beta)。
- グループに[チームを追加](/graph/api/team-put-teams?view=graph-rest-beta)します。

## <a name="create-a-group"></a>グループを作成する

チームを含めるには、次の例に示すプロパティの値を設定する必要があります。

- **groupTypes** = { "Unified" } 
- **mailEnabled** = true
- **securityEnabled** = false

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

次の例に、応答を示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>グループにチームを追加する

次に示すように、グループにチームを追加します。

```http
PUT /groups/{id}/team
{ }
```

次の例に、応答を示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

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

作成したチームには、グループと同じ ID が割り当てられます。
