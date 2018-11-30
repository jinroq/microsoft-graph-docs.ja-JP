---
title: recordOperation リソースの種類
description: RecordOperation 型
ms.openlocfilehash: 5863e5ef84b00c65cd0806af8a3364fe3d1ab73f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067828"
---
# <a name="recordoperation-resource-type"></a>recordOperation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

RecordOperation 型

## <a name="properties"></a>プロパティ

| プロパティ                       | 型                        | 説明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | クライアントのコンテキスト。                                                                                                                               |
| completionReason               | String                      | 可能な値は、`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError` です。 |
| createdDateTime                | DateTimeOffset              | レコーディングが作成された時刻。                                                                                                          |
| id                             | String                      | サーバー操作の id です。読み取り専用です。 サーバーを生成します。                                                                                             |
| lastActionDateTime             | DateTimeOffset              | 操作の最後の操作の時間です。                                                                                                     |
| recordResourceLocation         | String                      | 記録が保存されている場所です。                                                                                                      |
| recordResourceAccessToken      | String                      | 記録を取得するために必要なアクセス トークンです。                                                                                              |
| resultInfo                     | [resultInfo](resultinfo.md) | 結果の情報です。  読み取り専用。 サーバーを生成します。                                                                                             |
| status                         | String                      | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。 読み取り専用です。 サーバーを生成します。                                                 |

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
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceLocation": "String",
  "recordResourceAccessToken": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>使用例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
