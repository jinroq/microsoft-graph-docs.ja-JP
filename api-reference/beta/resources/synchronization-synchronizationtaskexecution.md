---
title: 同期タスク実行リソースの種類
description: 同期ジョブの実行結果の概要を示します。
localization_priority: Normal
ms.openlocfilehash: a9008dd7d51a1d07be75c5b9bbad34d636fff74c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339826"
---
# <a name="synchronizationtaskexecution-resource-type"></a>同期タスク実行リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期ジョブの実行結果の概要を示します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|activityidentifier           |String |ジョブの実行の識別子。|
|対象の count                |Int64  |このアプリケーションに対して割り当てられた処理済みエントリの数。|
|countEntitledForProvisioning |Int64  |プロビジョニング用に割り当てられた処理済みエントリの数。|
|countEscrowed                |Int64  |escrowed されたエントリの数 (エラー)。|
|countEscrowedRaw             |Int64  |システム生成 escrows を含む、escrowed されたエントリの数。|
|countexported 済み                |Int64  |エクスポートされたエントリの数。|
|countExports                 |Int64  |エクスポートが予期されたエントリの数。|
|countImported                |Int64  |インポートされたエントリの数。|
|countImportedDeltas          |Int64  |インポートされたデルタ変更の数。|
|countImportedReferenceDeltas |Int64  |参照変更に関連するインポートされたデルタ変更の数。|
|error                        |[同期エラー](synchronization-synchronizationerror.md)|エラーが発生した場合は、詳細情報を含む**同期エラー**オブジェクトが格納されています。|
|state                        |String |この実行の結果を要約したコード。 可能な値は、`Succeeded`、`Failed`、`EntryLevelErrors` です。|
|開始時刻                    |DateTimeOffset|このジョブの実行が開始された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|timeended                    |DateTimeOffset|このジョブの実行が終了した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
