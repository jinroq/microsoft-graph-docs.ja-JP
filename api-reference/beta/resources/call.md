---
title: リソースの種類を呼び出す
description: アプリケーション宛ての着信呼び出しがあるか、アプリケーションを使用して新しい送信呼び出しを作成するときに、**呼び出す**リソースが作成された、`POST`の`app/calls`。
ms.openlocfilehash: 8819f03b844f1d67a56f8bbd9e6eca0608de92ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071572"
---
# <a name="call-resource-type"></a>リソースの種類を呼び出す

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーション宛ての着信呼び出しがあるか、アプリケーションを使用して新しい送信呼び出しを作成するときに、**呼び出す**リソースが作成された、`POST`の`app/calls`。

ピア ツー ピアとマルチパーティの呼び出しは、呼び出しを設定できます。 マルチパーティの電話への参加を作成または、指定の`chatInfo`と`meetingInfo`。 これらが指定されなかった場合、新しいアドホック会議が自動的に作成します。 着信呼び出しに、可用性の高いストアでこれらの値を記録できるように、アプリケーションがクラッシュした場合に、通話に参加するようにアプリケーション。

同じ id が複数回を招待することはできません、ですが、アプリケーションが、同じ会議の複数回に参加することができます。 たびに個別の呼び出し、アプリケーションの結合`id`会議には、その呼び出しのために用意されています。 クライアントにさまざまな参加者を表示するためにミーティングに参加する別の id を使用することをお勧めします。

## <a name="methods"></a>メソッド

| メソッド                                                            | 戻り値の型                                       | 説明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [呼び出しを取得します。](../api/call-get.md)                                    | [呼び出し](call.md)                                   | 読み取り、オブジェクトのプロパティ**を呼び出します**。      |
| [削除](../api/call-delete.md)                                   |                                                   | 削除または**呼び出し**のアクティブな回線を切る。        |
| **呼び出し処理**                                                 |                                                   |                                              |
| [回答](../api/call-answer.md)                                   |                                                   | 着信呼び出しに応答します。                     |
| [Reject](../api/call-reject.md)                                   |                                                   | 着信呼び出しを拒否します。                     |
| [リダイレクト](../api/call-redirect.md)                               |                                                   | 着信呼び出しをリダイレクトします。                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | 通話を転送します。                              |
| **マルチ パーティー**                                                   |                                                   |                                              |
| [参加者の一覧](../api/call-list-participants.md)             | [参加者](participant.md)のコレクション          | 構成要素オブジェクトのコレクションを取得します。         |
| [参加者を招待します。](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | アクティブな通話に参加者を招待します。      |
| [参加者全員をミュートします。](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | 呼び出しのすべての参加者をミュートします。           |
| [オーディオ ミキサーを構成します。](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | 通話の音声を構成します。  |
| [AudioRoutingGroup を作成します。](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | AudioRoutingGroups コレクションへの投稿には、新しい audioRoutingGroup を作成します。 |
| [リスト audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)コレクション|AudioRoutingGroup オブジェクトのコレクションを取得します。  |
| **対話型音声応答**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [commsOperation](commsoperation.md)               | 呼び出しではプロンプトを再生します。                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | 呼び出しを記録します。                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | メディア処理をキャンセルします。                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | DTMF トーンを購読します。                     |
| **自己構成要素の操作**                                   |                                                   |                                              |
| [ミュート](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | 呼び出しで自身をミュートします。                       |
| [ミュート解除します。](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | 呼び出しで自身のミュートを解除します。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | 名簿に、自身のメタデータを更新します。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | 起動し、画面の呼び出しでの共有を停止                                             |

## <a name="properties"></a>プロパティ

| プロパティ            | 型                                                                                                   | 説明                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | 文字列コレクション                                                                                      | アクティブな様相の一覧です。 可能な値は、`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data` です。 値の取得のみ可能です。 サーバーを生成します。                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | 参加者の呼び出しに応答をします。 値の取得のみ可能です。 サーバーを生成します。                                                                                                                                |
| callRoutes          | [callRoute](callroute.md)コレクション                                                                   | ルーティングについての呼び出しを再ターゲットする方法。 値の取得のみ可能です。 サーバーを生成します。                                                                                                                |
| callbackUri         | String                                                                                                 | コールバックまたはサブスクリプションの ID をコールバックが配信されます。                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | チャット情報。                                                                                                                                                                               |
| 方向           | String                                                                                                 | 呼び出しの方向です。 使用可能な値は、`incoming`または`outgoing`。 値の取得のみ可能です。 サーバーを生成します。                                                                                            |
| id                  | String                                                                                                 | 読み取り専用。 サーバーを生成します。                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md)または[serviceHostedMediaConfig](servicehostedmediaconfig.md) | メディアの構成です。                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | 会議の機能が含まれています。                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md)または[tokenMeetingInfo](tokenmeetinginfo.md)             | 会議の情報。                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | 読み取り専用。 サーバーを生成します。                                                                                                                                                                        |
| requestedModalities | String コレクション                                                                                      | 要求された形式の一覧です。 | 可能な値は、`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data` です。                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | 結果の情報です。 たとえば退職理由を保持できます。 値の取得のみ可能です。 サーバーを生成します。                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | 送信ピア ツー ピアの通話の着信のタイムアウト                                                                                                                                                     |
| routingPolicies     | String コレクション                                                                                      | 可能な値は、`none`、`noMissedCall`、`disableForwardingExceptPhone`、`disableForwarding` です。                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | 通話の発信者です。                                                                                                                                                                         |
| state               | String                                                                                                 | 呼び出しの状態です。 可能な値は、`incoming`、`establishing`、`ringing`、`established`、`hold`、`transferring`、`transferAccepted`、`redirecting`、`terminating`、`terminated` です。 値の取得のみ可能です。 サーバーを生成します。                         |
| subject             | String                                                                                                 | 会話の件名です。                                                                                                                                                                    |
| ターゲット             | [participantInfo](participantinfo.md)コレクション                                                       | 呼び出しのターゲットです。                                                                                                                                                                            |
| tenantId            | String                                                                                                 | Azure Active Directory 内の tenantId です。                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | 読み取り専用。 サーバーを生成します。                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | 値の取得のみ可能です。 サーバーを生成します。                                                                                                                                                                        |

> メモ: プロパティとしてマーク`Server generated`を処理するときに無視されます`POST`の`app/calls`。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ        | 型                                                 | 説明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md)コレクション | 読み取り専用。Null 許容型。                                                |
| operations          | [commsOperation](commsoperation.md)コレクション       | 読み取り専用。Null 許容型。                                                |
| participants        | [参加者](participant.md)のコレクション             | 読み取り専用です。Null 許容型。                                                |

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
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **注:** マイクロソフトのチームとのスケジュールされたミーティングの参加の URL が表示されます。 塗りつぶし、URL からデータを抽出するには`chatInfo`と`meetingInfo`。

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
<!-- {
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
