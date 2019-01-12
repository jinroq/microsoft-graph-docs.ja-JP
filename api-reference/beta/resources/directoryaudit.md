---
title: directoryAudit リソースの種類
description: このリソースを表し、ディレクトリの監査項目のコレクション
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991784"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit リソースの種類
このリソースを表し、ディレクトリの監査項目のコレクション


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |コレクションとそのプロパティでディレクトリの監査項目を一覧表示します。|
|[DirectoryAudit を取得します。](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |特定のディレクトリの監査項目とそのプロパティを取得します。|


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|アクティビティが実行された日時を示します。 タイムスタンプ型が、常に UTC 時刻です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|activityDisplayName|String|アクティビティ名または操作の名前 (例。 「ユーザーを作成する」、「グループ メンバーの追加」)。 ログに記録する活動のリストは、 [Azure の広告活動のリスト](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)を参照してください。|
|additionalDetails|[keyValue](keyvalue.md)コレクション|活動に関する詳細情報を示します。|
|category|String|活動の対象となっているリソース カテゴリを示します。 (例: ユーザーの管理、グループの管理などです。)。|
|correlationId|GUID|により、さまざまなサービス全体にわたる活動を関連付ける一意の ID を示します。 サービス全体にわたるトレース ログを使用できます。|
|id|String| アクティビティの一意の ID を示します。 これは、GUID です。|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|ユーザーまたはアプリケーションに関する情報が、アクティビティを開始することを示します。|
|loggedByService|String|サービスが動作を開始する情報を示します (例: セルフ サービスのパスワード管理、コア ディレクトリ、B2C、ユーザーの招待、Microsoft 個人情報管理、Id 管理の権限を持つ。|
|result|string| 活動の結果を示します。使用可能な値: `success`、 `failure`、 `timeout`、 `unknownFutureValue`。||
|resultReason|String|結果が [エラー] または [タイムアウト] の場合は、エラーの原因を示します。|
|targetResources|[targetResource](targetresource.md)コレクション|活動のためのリソースが変更された情報を示します。 ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリケーション、役割、グループ、ポリシーまたはその他を指定できます。

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
