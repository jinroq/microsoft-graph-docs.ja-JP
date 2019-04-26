---
title: onlineMeeting リソースの種類
description: 参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568864"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
| [onlineMeeting を取得する](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | onlineMeeting オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ

| プロパティ                  | 型                                                   | 説明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | オンライン会議への受付を制御するアクセスレベル。 可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。 |
| audioconferencing         | [audioconferencing](audioconferencing.md)              | onlineMeeting の電話アクセス情報を表します。 |
| canceleddatetime          | DateTime
                                               | 会議がキャンセルされた時刻。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | この会議に関連付けられているチャット。 |
| 日付/時刻 (datetime)          | DateTime
                                               | 会議が作成された時刻。 該当.
| endDateTime               | DateTime
                                               | 会議の終了時刻。 |
| entryexitannouncement     | Boolean                                                | オンライン会議の出席アナウンスの状態。 出席依頼のアナウンスが有効になっている場合、オンライン会議では、participantswho の名前が音声で会議に参加するようにアナウンスされます。 |
| expirationDateTime        | DateTime
                                               | オンライン会議を削除できる、世界協定時 (UTC) の日付と時刻。 日付と時刻は、サーバー上の現在の日付と時刻の1年前、10年前にする必要があります。 |
| id                        | String                                                 | オンライン会議に関連付けられている ID。 ID として GET HTTP 要求で使用されます。 読み取り専用です。 サーバーによって生成されます。 |
| isCancelled               | Boolean                                                | 会議がキャンセルされたかどうか。 |
| joinurl                   | String                                                 | オンライン会議が web から参加しているときに使用される URL。 |
| 会議の種類               | String                                                 | 可能な値は`meetNow`、 `scheduled`、 `recurring`、、です。`broadcast` |
| 参加者              | [会議参加者](meetingparticipants.md)          | オンライン会議に関連付けられている参加者。  これには、開催者と出席者が含まれます。 |
| startDateTime             | DateTime
                                               | 会議の開始時刻。 |
| subject                   | String                                                 | オンライン会議の件名。 |

## <a name="relationships"></a>関係
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
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
