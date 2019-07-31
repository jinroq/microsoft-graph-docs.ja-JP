---
title: 同期ジョブリソースの種類
description: バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。 同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。 同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a311c8ae7618778c2dbd8cdbc9a5b30af254eae4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007796"
---
# <a name="synchronizationjob-resource-type"></a>同期ジョブリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。 同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。 同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[同期ジョブ](synchronization-synchronizationjob.md)のコレクション  |特定のアプリケーションインスタンス (サービスプリンシパル) の既存のジョブを一覧表示します。|
|[同期ジョブを取得する](../api/synchronization-synchronizationjob-get.md) | [同期ジョブ](synchronization-synchronizationjob.md) |同期ジョブオブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[同期ジョブ](synchronization-synchronizationjob.md)   |指定したアプリケーションの新しいジョブを作成します。|
|[Start](../api/synchronization-synchronizationjob-start.md)          |None   |同期を開始します。 ジョブが一時停止状態である場合、ジョブが一時停止した時点から続行されます。 ジョブが検疫されている場合は、検疫の状態はクリアされます。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |None   |ジョブを強制的に開始し、ディレクトリ内のすべてのオブジェクトを再処理します。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |None   |一時的に同期を停止します。 ジョブの状態を含むすべての進行状況が持続され、[開始](../api/synchronization-synchronizationjob-start.md)呼び出しが行われたときにジョブは中断したところから続行されます。|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |None   |同期を停止し、ジョブに関連付けられているすべての状態を完全に削除します。|
|[同期スキーマを取得する](../api/synchronization-synchronizationschema-get.md)    |[同期スキーマ](synchronization-synchronizationschema.md)   |ジョブの有効な同期スキーマを取得します。|
|[同期スキーマの更新](../api/synchronization-synchronizationschema-update.md)    |None   |ジョブの同期スキーマを更新します。 |
|[資格情報を検証する](../api/synchronization-synchronizationjob-validatecredentials.md)|None|ターゲットディレクトリに対して提供された資格情報をテストします。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|id             |String                     |一意の同期ジョブ識別子。 読み取り専用です。|
|schedule       |[同期スケジュール](synchronization-synchronizationschedule.md)|ジョブを実行するために使用するスケジュール。 読み取り専用です。|
|status         |[同期の状態](synchronization-synchronizationstatus.md)     |ジョブの状態。ジョブが最後に実行された日時、現在のジョブの状態、エラーが含まれます。|
|templateId     |String    |このジョブの基になっている[同期テンプレート](synchronization-synchronizationtemplate.md)の識別子。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|スキーマ|[同期スキーマ](synchronization-synchronizationschema.md)| ジョブに対して構成されている同期スキーマ。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
