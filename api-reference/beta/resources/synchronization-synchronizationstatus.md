---
title: 同期状態リソースの種類
description: 同期ジョブの現在の状態を表します。
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453871"
---
# <a name="synchronizationstatus-resource-type"></a>同期状態リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[同期ジョブ](synchronization-synchronizationjob.md)の現在の状態を表します。

## <a name="properties"></a>プロパティ

| プロパティ                              | 型      | 説明    |
|:--------------------------------------|:----------|:---------------|
|code|String|同期ジョブの高レベルの状態コード。 可能な値は、`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine` です。|
|countSuccessiveCompleteFailures|Int64|このジョブが失敗した連続した時間数。|
|escrowsPruned|ブール型|`true`最初の同期中にジョブの escrows (オブジェクトレベルのエラー) が排除された場合。 Escrows を排除できる初期の同期時には、通常、検疫内にジョブを配置するエラーのしきい値に達します。 検疫に入る代わりに、同期プロセスによってジョブのエラーがクリアされ、初期同期が完了するまで続行されます。 初期同期が完了すると、ジョブは一時停止し、ユーザーがエラーをクリーンアップするのを待ちます。|
|lastexecution|[同期タスクの実行](synchronization-synchronizationtaskexecution.md)|ジョブの前回の実行の詳細。|
|lastSuccessfulExecution|[同期タスクの実行](synchronization-synchronizationtaskexecution.md)|このジョブの前回の実行の詳細。エラーはありませんでした。|
|lastSuccessfulExecutionWithExports|[同期タスクの実行](synchronization-synchronizationtaskexecution.md)|ターゲットディレクトリにオブジェクトをエクスポートした、ジョブの最後の実行の詳細。|
|progress|[同期の進行状況](synchronization-synchronizationprogress.md)のコレクション|完了までのジョブの進行状況の詳細。|
|済み|[同期検疫](synchronization-quarantine.md)|ジョブが検疫されている場合は、検疫の詳細。|
|steadyStateFirstAchievedTime|DateTimeOffset|安定した状態 (プロセスに加えられた変更はありません) が最初に達成された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|steadyStateLastAchievedTime|DateTimeOffset|安定した状態 (プロセスに加えられた変更がない状態) が最後に達成された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|synchronizedEntryCountByType|[stringkeylongvaluepair](synchronization-stringkeylongvaluepair.md)コレクション|オブジェクトの種類別にリストされた、同期されたオブジェクトの数。|
|トラブルシューティング url|String|エラーが発生した場合は、問題のトラブルシューティング手順が記載されている URL を使用します。|

### <a name="synchronization-status-code-details"></a>同期状態コードの詳細

| 値                              | 説明    |
|:-----------------------------------|:---------------|
|NotConfigured                       |ジョブは構成されておらず、実行されません。 認証は提供されませんでした。 |
|notrun                              |ジョブが構成されている可能性がありますが、最初の実行が完了していない可能性があります。|
|Active                              |ジョブは定期的に実行されています。|
|一時停止                              |ジョブが一時停止されました (通常は管理者によって)。現在実行されていませんが、ジョブの状態は保持されます。|
|検疫                          |ジョブは検疫中です。 これは、大量のエラーが発生した場合や、失効済みまたは期限が切れた資格情報などの重大なエラーが発生した場合に発生する可能性があります。 検疫中は、同期プロセスによってジョブの実行が試行されます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
