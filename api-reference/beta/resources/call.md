---
title: call リソースの種類
description: アプリケーションに関して着信が存在する場合か、アプリケーションによって `app/calls` で `POST` を介して発信が作成されると、**call** リソースが作成されます。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9d297a60538901b6117a7e20f32fa0cc437b9b84
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338802"
---
# <a name="call-resource-type"></a>call リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションに関して着信が存在する場合か、アプリケーションによって `app/calls` で `POST` を介して発信が作成されると、**call** リソースが作成されます。

通話はピアツーピアまたはマルチパーティ通話として設定できます。 マルチパーティ通話を作成または参加する場合、`chatInfo` と `meetingInfo` を指定します。 これらを指定しないと、新しい臨時会議が自動的に作成されます。 着信の場合、高可用性ストアにこれらの値が記録されるので、アプリケーションがクラッシュしたときに、アプリケーションが通話に再度参加できるようになります。

アプリケーションでは同じ ID を複数回にわたり招待することはできませんが、同じ会議に何度も参加することは可能です。 アプリケーションが参加するたびに、対象会議に対する個別の通話 `id` が提供されます。 クライアントが異なる参加者として表示されるように、会議に参加するために別々の ID を使用することをお勧めします。

## <a name="methods"></a>メソッド

| メソッド                                                            | 戻り値の型                                       | 説明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [call を取得する](../api/call-get.md)                                    | [call](call.md)                                   | **call** オブジェクトのプロパティを読み取ります。      |
| [削除する](../api/call-delete.md)                                   |                                                   | アクティブな **call** を削除または切断します。        |
| **Call 処理**                                                 |                                                   |                                              |
| [応答する](../api/call-answer.md)                                   |                                                   | 着信に応答します。                     |
| [拒否する](../api/call-reject.md)                                   |                                                   | 着信を拒否します。                     |
| [リダイレクトする](../api/call-redirect.md)                               |                                                   | 着信をリダイレクトします。                   |
| [転送する](../api/call-transfer.md)                               |                                                   | 通話を転送します                              |
| **マルチパーティ**                                                   |                                                   |                                              |
| [参加者を一覧表示する](../api/call-list-participants.md)             | [participant](participant.md) コレクション          | participant オブジェクト コレクションを取得します。         |
| [参加者を招待する](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | アクティブな通話に参加者を招待します。      |
| [すべての参加者をミュートする](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | 通話ですべての参加者をミュートします。           |
| [オーディオ ミキサーを構成する](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | マルチパーティ会話の音声を構成します。  |
| [audioRoutingGroup を作成する](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | audioRoutingGroups コレクションに投稿して、新しい audioRoutingGroup を作成します。 |
| [audioRoutingGroups を一覧表示する (List audioRoutingGroups)](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md) コレクション|audioRoutingGroup オブジェクト コレクションを取得します。  |
| **対話型音声応答**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | 通話でプロンプトを再生します。                     |
| [録音する](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | 通話を録音します。                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | メディア処理を取り消します。                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | DTMF トーンを登録します。                     |
| **自分の参加に関する操作**                                   |                                                   |                                              |
| [ミュートする](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | 通話で自分をミュートします。                       |
| [ミュート解除する](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | 通話で自分のミュートを解除します。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | 自分の名簿のメタデータを更新します。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | 通話における画面共有を開始および停止します                                             |

## <a name="properties"></a>プロパティ

| プロパティ            | 型                                                                                                   | 説明                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | String コレクション                                                                                      | アクティブなモダリティの一覧。 可能な値は、`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data` です。 読み取り専用です。 サーバーによって生成されます。                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | 通話に応答した参加者。 読み取り専用です。 サーバーによって生成されます。                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) コレクション                                                                   | 再通話したときのルーティング情報。 読み取り専用です。 サーバーによって生成されます。                                                                                                                |
| callbackUri         | String                                                                                                 | コールバック時のコールバック ID またはサブスクリプション ID。                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | チャット情報。                                                                                                                                                                               |
| direction           | String                                                                                                 | 通話方向。 使用可能な値: `incoming`、`outgoing`。 読み取り専用です。 サーバーによって生成されます。                                                                                            |
| id                  | String                                                                                                 | 読み取り専用です。 サーバーによって生成されます。                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) または [serviceHostedMediaConfig](servicehostedmediaconfig.md) | メディア構成。                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | 会議の機能が含まれます。                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) または [tokenMeetingInfo](tokenmeetinginfo.md)             | 会議の情報。                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | 読み取り専用です。 サーバーによって生成されます。                                                                                                                                                                        |
| requestedModalities | String コレクション                                                                                      | 要求されたモダリティの一覧。 | 可能な値は、`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data` です。                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | 結果の情報。 たとえば、終了理由を保持できます。 読み取り専用です。 サーバーによって生成されます。                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | 発信ピアツーピア通話の呼び出しタイムアウト                                                                                                                                                     |
| routingPolicies     | String コレクション                                                                                      | 使用可能な値は、`none`、`noMissedCall`、`disableForwardingExceptPhone`、`disableForwarding` です。                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | 通話の発信者。                                                                                                                                                                         |
| state               | String                                                                                                 | 通話状態。 可能な値は、`incoming`、`establishing`、`ringing`、`established`、`hold`、`transferring`、`transferAccepted`、`redirecting`、`terminating`、`terminated` です。 読み取り専用です。 サーバーによって生成されます。                         |
| subject             | String                                                                                                 | 会話の件名。                                                                                                                                                                    |
| Targets             | [participantInfo](participantinfo.md) コレクション                                                       | 通話対象。                                                                                                                                                                            |
| tenantId            | String                                                                                                 | Azure Active Directory の tenantId。                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | 読み取り専用です。 サーバーによって生成されます。                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | 読み取り専用です。 サーバーによって生成されます。                                                                                                                                                                        |

> 注: `Server generated` というマークの付いたプロパティは、`app/calls` の `POST` 処理時に無視されます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ        | 型                                                 | 説明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md) コレクション | 読み取り専用です。 Null 許容型。                                                |
| operations          | [commsOperation](commsoperation.md)コレクション       | 読み取り専用。Null 許容型です。                                                |
| participants        | [participant](participant.md) コレクション             | 読み取り専用。Null 許容型です。                                                |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "chatInfo",
    "direction",
    "id",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "microsoft.graph.toneInfo"}
}
```

> **注:** Microsoft Teams でスケジュール設定された会議の参加 URL が見つかります。 その URL からデータを抽出し、`chatInfo` と `meetingInfo` に情報を設定する方法について次に示します。

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  truncated: true
}-->
```json
{
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "id": "4b444206-207c-42f8-92a6-e332b41c88a2"
      }
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
