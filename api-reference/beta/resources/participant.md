---
title: 参加者のリソースの種類
description: 参加者のタイプです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508147"
---
# <a name="participant-resource-type"></a>参加者のリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参加者のタイプです。

## <a name="methods"></a>メソッド

| メソッド                                                          | 戻り値の型                              | 説明                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [構成要素を取得します。](../api/participant-get.md)                    | [参加者](participant.md)            | **構成要素**オブジェクトのプロパティを参照します。    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | 参加者のオーディオ ミキサーを構成します。            |
| [招待](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | 通話に参加者を招待します。                 |
| [参加者のミュート](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | 呼び出し内の参加者をミュートします。                     |
| [参加者全員をミュートします。](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | 会議のすべての参加者をミュートします。         |

## <a name="properties"></a>プロパティ

| プロパティ             | 型                                     | 説明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | 参加者の id です。                                          |
| Info                 | [participantInfo](participantinfo.md)    | 参加者の参加者です。                          |
| isInLobby            | boolean                                  | 参加者がロビーに入っている場合は true。                          |
| isMuted              | boolean                                  | 参加者がミュートされている場合は true (クライアントまたはサーバーがミュートになって)    |
| mediaStreams         | [mediaStream](mediastream.md)コレクション | メディア ストリームのリスト。                                   |
| metadata             | String                                   | 名簿にある参加者が提供するデータの blob     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 参加者が録画機能を持つかどうかについて説明します。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
