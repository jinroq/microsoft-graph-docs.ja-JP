---
title: audioconferencing リソースの種類
description: onlineMeeting の電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1371e80830bf148588f6bda91326b0521fcdda42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328375"
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
  "suppressions": []
}
-->
