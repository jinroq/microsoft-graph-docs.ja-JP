---
title: 参加者リソースの種類
description: 参加者の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568660"
---
# <a name="participant-resource-type"></a>参加者リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参加者の種類。

## <a name="methods"></a>メソッド

| メソッド                                                          | 戻り値の型                              | 説明                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [参加者を取得する](../api/participant-get.md)                    | [積極的](participant.md)            | **参加者**オブジェクトのプロパティを読み取ります。    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | 参加者のオーディオミキサーを構成します。            |
| [招待](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | 参加者を呼び出しに招待します。                 |
| [参加者をミュートする](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | 通話の参加者をミュートにします。                     |
| [すべての参加者をミュートする](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | 会議のすべての参加者をミュートにします。         |

## <a name="properties"></a>プロパティ

| プロパティ             | 型                                     | 説明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | 参加者 id。                                          |
| info                 | [participantInfo](participantinfo.md)    | 参加者の参加者。                          |
| isInLobby            | ブール値                                  | 参加者がロビーにある場合は true                          |
| ismuted              | ブール値                                  | 参加者がミュートされている場合は true (クライアントまたはサーバーがミュート状態)    |
| mediastreams         | [mediastream](mediastream.md)コレクション | メディアストリームのリスト。                                   |
| metadata             | String                                   | 参加者が名簿に提供するデータの blob     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 参加者にレコーディング機能があるかどうかに関する情報。 |

## <a name="relationships"></a>関係
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
  "suppressions": []
}
-->
