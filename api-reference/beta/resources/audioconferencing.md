---
title: audioConferencing リソースの種類
description: OnlineMeeting の電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 94dc02920e7270fbfdacb10ee9a8edee8315fc67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974284"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[OnlineMeeting](onlinemeeting.md)の電話アクセス情報を表します。

## <a name="properties"></a>プロパティ

| プロパティ            | 型    | 説明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| ダイヤルイン Url           | String  | 外部からアクセス可能な web ページへの URL。ダイヤルイン情報が含まれています。 |
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
