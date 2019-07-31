---
title: recordOperation リソースの種類
description: RecordOperation の種類
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00b05cd86eeb9cf8be26cdc09fb8a9b254b510db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008804"
---
# <a name="recordoperation-resource-type"></a>recordOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

RecordOperation の種類

## <a name="properties"></a>プロパティ

| プロパティ                       | 型                        | 説明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | クライアントコンテキスト。                                                                                                                               |
| 「補完の理由」               | String                      | 可能な値は、`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none` です。 |
| createdDateTime                | DateTimeOffset              | レコーディングが作成された時刻。                                                                                                          |
| id                             | 文字列                      | サーバー操作 id。読み取り専用です。 サーバーによって生成されます。                                                                                             |
| lastActionDateTime             | DateTimeOffset              | 操作の最後の操作の時刻。                                                                                                     |
| recordResourceAccessToken      | String                      | レコーディングを取得するために必要なアクセストークン。                                                                                              |
| recordResourceLocation         | String                      | レコーディングが配置されている場所。                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | 結果の情報。  読み取り専用です。 サーバーによって生成されます。                                                                                             |
| status                         | String                      | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。 読み取り専用です。 サーバーによって生成されます。                                                 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
