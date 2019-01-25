---
title: synchronizationJob リソースの種類
description: バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510569"
---
# <a name="synchronizationjob-resource-type"></a>synchronizationJob リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md)コレクション  |特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。|
|[SynchronizationJob を取得します。](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |SynchronizationJob オブジェクトのプロパティと関係を参照してください。|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |特定のアプリケーション用の新しいジョブを作成します。|
|[Start](../api/synchronization-synchronizationjob-start.md)          |なし   |同期を開始します。 ジョブが一時停止状態にある場合は、ジョブが一時停止された時点から続行します。 ジョブは、検疫では、検疫の状態がクリアされます。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |なし   |上で起動し、ディレクトリ内のすべてのオブジェクトを再処理するジョブを強制します。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |なし   |同期を一時的に停止します。 ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |なし   |同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。|
|[SynchrnoizationSchema を取得します。](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |ジョブの効果的な同期スキーマを取得します。|
|[SynchroizationSchema を更新します。](../api/synchronization-synchronizationschema-update.md)    |なし   |ジョブの同期のスキーマを更新します。 |
|[資格情報を検証します。](../api/synchronization-synchronizationjob-validatecredentials.md)|なし|ターゲット ディレクトリに対して指定された資格情報をテストします。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|id             |String                     |固有の同期ジョブの識別子です。 読み取り専用です。|
|Schedule       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|スケジュールがジョブを実行するために使用します。 読み取り専用です。|
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
