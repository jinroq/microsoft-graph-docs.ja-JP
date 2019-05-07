---
title: directoryAudit リソース型
description: ディレクトリ監査アイテムとそのコレクションを表します。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f49229ed1ce461a0e9dcc104087ec89726597267
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629293"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit リソース型

ディレクトリ監査アイテムとそのコレクションを表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[directoryAudits を一覧表示する](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。|
|[directoryAudit を取得する](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |特定のディレクトリの監査アイテムとそのプロパティを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|アクティビティが実行された日付と時刻を示します。 Timestamp 型は、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|activityDisplayName|String|アクティビティ名または操作名 (例: [ユーザーの作成] と [グループにメンバーを追加]) を示します。 完全なリストについては、「 [AZURE AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)」を参照してください。|
|additionalDetails|[keyvalue](keyvalue.md) コレクション|アクティビティに関する詳細情報を示します。|
|category|String|どのリソース カテゴリがアクティビティの対象となっているかを示します。 (例: ユーザー管理、グループ管理など)|
|correlationId|GUID|さまざまなサービスの間にまたがるアクティビティを関連付けるのに役立つ一意の ID を示します。 サービスのログを追跡するために使用できます。|
|id|文字列| アクティビティの一意の ID を示します。 これは、GUID です。|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|アクティビティを開始したユーザーまたはアプリについての情報を示します。|
|loggedByService|String|アクティビティを開始するサービスについての情報を示します (例: セルフ サービス パスワード管理、コア ディレクトリ、B2C、招待されたユーザー、Microsoft Identity Manager、Privileged Identity Management)。|
|result|string| アクティビティの結果を示します。使用可能な値は `success`、`failure`、`timeout`、`unknownFutureValue` です。||
|resultReason|String|"失敗" または "タイムアウト" の結果について説明します。|
|targetResources|[targetResource](targetresource.md) コレクション|アクティビティのためにどのリソースが変更されたかについての情報を示します。 ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリ、役割、グループ、ポリシー、その他があります。

## <a name="relationships"></a>関係

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
