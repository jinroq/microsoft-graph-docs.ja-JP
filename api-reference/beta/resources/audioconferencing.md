---
title: audioConferencing リソースの種類
description: OnlineMeeting には、電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977508"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[OnlineMeeting](onlinemeeting.md)には、電話アクセス情報を表します。

## <a name="properties"></a>プロパティ

| プロパティ            | 種類    | 説明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | ダイヤルイン情報を含む外部からアクセス可能な web ページの URL です。 |
| leaderPasscode      | String  | オーディオ会議プロバイダーへの接続に必要なリーダーのパスワードです。      |
| participantPasscode | String  | オーディオ会議プロバイダーへの接続に必要な参加者のパスワードです。 |
| tollFreeNumber      | String  | オーディオ会議プロバイダーに接続する無料電話番号です。              |
| tollNumber          | String  | オーディオ会議プロバイダーに接続する有料電話番号です。                   |

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
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
