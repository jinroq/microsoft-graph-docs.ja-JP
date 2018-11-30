---
title: synchronizationStatus リソースの種類
description: SynchronizationJob の現在の状態を表します。
ms.openlocfilehash: cf1b1e79e5ad784f1f43a2e5bf082c68b41e96ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074417"
---
# <a name="synchronizationstatus-resource-type"></a>synchronizationStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[SynchronizationJob](synchronization-synchronizationjob.md)の現在の状態を表します。

## <a name="properties"></a>プロパティ

| プロパティ                              | 型      | 説明    |
|:--------------------------------------|:----------|:---------------|
|code|String|同期ジョブの高度なステータス コードです。 可能な値は、`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine` です。|
|countSuccessiveCompleteFailures|Int64|連続回数このジョブが失敗しました。|
|escrowsPruned|ブール値|`true`場合はジョブの escrows (オブジェクト レベルのエラー) は、初期同期中に排除されました。 初期同期中にエラーを通常どおりになりそうなジョブ検疫のしきい値に達した場合、escrows を排除することができます。 検疫場所にではなく、同期プロセスはジョブのエラーをクリアし、初期同期が完了するまで続きます。 初期同期が完了すると、ジョブが一時停止し、エラーをクリーンアップするまで待機します。|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|ジョブの前回の実行の詳細です。|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|このジョブは、エラーがなかったは、前回の実行の詳細です。|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|ターゲット ディレクトリにオブジェクトをエクスポートすると、ジョブの前回の実行の詳細です。|
|進行状況|[synchronizationProgress](synchronization-synchronizationprogress.md)コレクション|完了するまで、ジョブの進行状況の詳細です。|
|検査|[synchronizationQuarantine](synchronization-quarantine.md)|検査中のジョブの場合は、詳細を検査します。|
|steadyStateFirstAchievedTime|DateTimeOffset|最初に安定した状態 (プロセスに変更) が達成された時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|steadyStateLastAchievedTime|DateTimeOffset|最後に安定した状態 (プロセスに変更) が達成された時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)コレクション|オブジェクトの種類ごとに一覧表示、同期オブジェクトの数。|
|troubleshootingUrl|String|エラーの場合、問題のトラブルシューティングの手順で URL です。|

### <a name="synchronization-status-code-details"></a>同期ステータス コードの詳細

| 値                              | 説明    |
|:-----------------------------------|:---------------|
|NotConfigured                       |ジョブが構成されていないと、実行しません。 認証が指定されていません。 |
|NotRun                              |ジョブは、設定されていれば、および可能性があります開始は、その最初の実行を終了していません。|
|アクティブ                              |ジョブの有効期限が定期的に行われています。|
|一時停止                              |ジョブ (管理者) は通常、一時停止し、現在実行されていないが、ジョブの状態が保持されます。|
|検査                          |ジョブでは、検査中です。 大量のエラー、または資格情報の失効期限切れなどの重大なエラーがある場合、このエラーが発生する可能性があります。 検査中に、同期処理を減少の頻度でジョブの実行を試みます。|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
