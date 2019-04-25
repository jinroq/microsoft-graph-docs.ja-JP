---
title: audioconferencing リソースの種類
description: onlineMeeting の電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535562"
---
# <a name="audioconferencing-resource-type"></a>audioconferencing リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[onlineMeeting](onlinemeeting.md)の電話アクセス情報を表します。

## <a name="properties"></a>プロパティ

| プロパティ            | 型    | 説明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| ダイヤルイン url           | String  | 外部からアクセス可能な web ページへの URL。ダイヤルイン情報が含まれています。 |
| leaderPasscode      | String  | 電話会議プロバイダーに接続するために必要なリーダーパスワード。      |
| participantPasscode | String  | 音声会議プロバイダーに接続するために必要な、参加者のパスワード。 |
| tollFreeNumber      | String  | 音声会議プロバイダーに接続するための無料電話番号。              |
| tollNumber          | String  | 音声会議プロバイダーに接続する有料電話番号。                   |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
