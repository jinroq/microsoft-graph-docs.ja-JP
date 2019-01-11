---
title: onlineMeeting リソースの種類
description: 結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b1a0b09c0e7c792b0a9662c08daecd212c027c89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805160"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
| [OnlineMeeting を取得します。](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | OnlineMeeting オブジェクトのプロパティと関係を参照してください。 |

## <a name="properties"></a>プロパティ

| プロパティ                  | 種類                                                   | 説明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | オンラインの会議出席依頼の受付を制御するアクセス レベルです。 可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。 |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | OnlineMeeting には、電話アクセス情報を表します。 |
| canceledDateTime          | DateTime                                               | 会議がキャンセルされた時刻。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | この会議に関連付けられているチャット。 |
| creationDateTime          | DateTime                                               | ミーティングが作成された時刻。 読み取り専用です。
| endDateTime               | DateTime                                               | 会議の終了時間です。 |
| entryExitAnnouncement     | ブール型                                                | オンライン会議の出席のお知らせ状態です。 出勤のお知らせを有効にすると、オンライン会議、発表 participantswho 結合の名前、会議のオーディオを使用します。 |
| expirationDateTime        | DateTime                                               | 絶対の世界協定時刻 (UTC) の日付と時刻は、オンライン会議を削除できます。 曜日と時間は、1 年前に、および現在の日付と、サーバー上の時刻の後 10 年間する必要があります。 |
| id                        | String                                                 | オンライン会議に関連付けられている ID です。 HTTP の GET 要求では ID として使用 読み取り専用です。 サーバーを生成します。 |
| isCancelled               | ブール値                                                | かどうか、会議はキャンセルされました。 |
| joinUrl                   | String                                                 | Web サイトからオンライン会議を結合するときに使用される URL です。 |
| meetingType               | String                                                 | 使用可能な値: `meetNow`、 `scheduled`、 `recurring`、`broadcast` |
| participants              | [meetingParticipants](meetingparticipants.md)          | 参加者がオンライン会議に関連付けられています。  これには、開催者と出席者が含まれます。 |
| startDateTime             | DateTime                                               | 会議の開始時刻。 |
| subject                   | String                                                 | オンライン会議の件名です。 |

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
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
