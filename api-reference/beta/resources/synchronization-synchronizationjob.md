---
title: synchronizationJob リソースの種類
description: バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073911"
---
# <a name="synchronizationjob-resource-type"></a>synchronizationJob リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md)コレクション  |特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。|
|[SynchronizationJob を取得します。](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |SynchronizationJob オブジェクトのプロパティと関係を参照してください。|
|[作成](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |特定のアプリケーション用の新しいジョブを作成します。|
|[Start](../api/synchronization-synchronizationjob-start.md)          |なし   |同期を開始します。 ジョブが一時停止状態にある場合は、ジョブが一時停止された時点から続行します。 ジョブは、検疫では、検疫の状態がクリアされます。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |なし   |上で起動し、ディレクトリ内のすべてのオブジェクトを再処理するジョブを強制します。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |なし   |同期を一時的に停止します。 ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。|
|[削除](../api/synchronization-synchronizationjob-delete.md)        |なし   |同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。|
|[SynchrnoizationSchema を取得します。](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |ジョブの効果的な同期スキーマを取得します。|
|[SynchroizationSchema を更新します。](../api/synchronization-synchronizationschema-update.md)    |なし   |ジョブの同期のスキーマを更新します。 |
|[資格情報を検証します。](../api/synchronization-synchronizationjob-validatecredentials.md)|なし|ターゲット ディレクトリに対して指定された資格情報をテストします。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|id             |String                     |固有の同期ジョブの識別子です。 読み取り専用。|
|スケジュール       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|スケジュールがジョブを実行するために使用します。 読み取り専用。|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |ジョブが前回実行されたときに、ジョブ、ジョブの現在の状態およびエラーの状態です。|
|templateId     |文字列    |このジョブで使用する[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|スキーマ|[synchronizationSchema](synchronization-synchronizationschema.md)| ジョブ用に構成された同期スキーマです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->