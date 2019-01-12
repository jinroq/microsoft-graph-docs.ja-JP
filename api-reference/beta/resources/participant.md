---
title: 参加者のリソースの種類
description: 参加者のタイプです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d6a4474525086fb1e8aefe00ad37acaf6511e9f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938332"
---
# <a name="participant-resource-type"></a>参加者のリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ             | 種類                                     | 説明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| ID                   | String                                   | 参加者の id です。                                          |
| 情報                 | [participantInfo](participantinfo.md)    | 参加者の参加者です。                          |
| isInLobby            | ブール                                  | 参加者がロビーに入っている場合は true。                          |
| isMuted              | ブール                                  | 参加者がミュートされている場合は true (クライアントまたはサーバーがミュートになって)    |
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
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
