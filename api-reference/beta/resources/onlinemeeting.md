---
title: onlineMeeting リソースの種類
description: 参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 611731673d932d6c5135c0115d735e4d642b1bfe
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792794"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
| [OnlineMeeting を取得する](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | OnlineMeeting オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ

| プロパティ                  | 型                                                   | 説明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | オンライン会議への受付を制御するアクセスレベル。 可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。 |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | OnlineMeeting の電話アクセス情報を表します。 |
| canceledDateTime          | DateTime                                               | 会議がキャンセルされた時刻。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | この会議に関連付けられているチャット。 |
| 日付/時刻 (datetime)          | DateTime                                               | 会議が作成された時刻。 読み取り専用です。
| endDateTime               | DateTime                                               | 会議の終了時刻。 |
| entryExitAnnouncement     | Boolean                                                | オンライン会議の出席アナウンスの状態。 出席依頼のアナウンスが有効になっている場合、オンライン会議では、音声で会議に参加する参加者の名前がアナウンスされます。 |
| expirationDateTime        | DateTime                                               | オンライン会議を削除できる、世界協定時 (UTC) の日付と時刻。 日付と時刻は、サーバー上の現在の日付と時刻の1年前、10年前にする必要があります。 |
| id                        | 文字列                                                 | オンライン会議に関連付けられている ID。 ID として GET HTTP 要求で使用されます。 読み取り専用です。 サーバーによって生成されます。 |
| isCancelled               | Boolean                                                | 会議がキャンセルされたかどうか。 |
| joinUrl                   | String                                                 | オンライン会議が web から参加しているときに使用される URL。 |
| 会議の種類               | String                                                 | 使用可能な値`meetNow`は`scheduled`、 `recurring`、 `broadcast` 、、(メモ: [create onlineMeeting](../api/application-post-onlinemeetings.md) only がサポート`meetNow`) のいずれかです。 |
| participants              | [会議参加者](meetingparticipants.md)          | オンライン会議に関連付けられている参加者。  これには、開催者と出席者が含まれます。 |
| startDateTime             | DateTime                                               | 会議の開始時刻。 |
| subject                   | String                                                 | オンライン会議の件名。 |
| capabilities              | 文字列コレクション                                      | 会議機能のリスト。 可能な値は`questionAndAnswer`次のとおりです。 |
| videoTeleconferenceId     | String                                                 | ビデオ会議 id。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String"
}
```