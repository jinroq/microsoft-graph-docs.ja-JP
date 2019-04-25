---
title: teamsapp リソースの種類
description: Microsoft Teams アプリカタログのアプリ。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553954"
---
# <a name="teamsapp-resource-type"></a>teamsapp リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Microsoft Teams](teams-api-overview.md)アプリカタログのアプリ。

ユーザーは、これらのアプリを Microsoft teams ストアで表示できます。これらのアプリは、[[アプリをチームに追加する](../api/teamsappinstallation-add.md)] メソッドを使用して[Teams](team.md)にインストールできます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[公開されたアプリの一覧を表示する](../api/teamsapp-list.md) | [teamsApp](teamsapp.md) コレクション | Microsoft Teams アプリカタログから、公開されたアプリを一覧表示します。|
|[アプリを発行する](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | 組織のアプリカタログにアプリを発行します。|
|[公開されたアプリを更新する](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 組織のアプリカタログで公開されているアプリを更新します。|
|[公開されたアプリを削除する](../api/teamsapp-delete.md) | なし | 公開されたアプリを組織のアプリカタログから削除します。|

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | カタログアプリの生成されたアプリ id ( [Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者提供の id とは異なります)。 |
| externalId          | string   | [Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)のアプリ開発者によって提供されるカタログの ID。 |
| displayName                | string   | [Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)のアプリ開発者によって提供されるカタログアプリの名前です。 |
| distributionMethod  | teamsAppDistributionMethod     | アプリの配布方法。 |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod の値

|メンバー|値|説明|
|:---|:---|:---|
|ストア|.0| アプリは、Microsoft Teams アプリストアを介してすべてのテナントで利用できます。|
|組織|1 |アプリはこのテナントでのみ使用できます。|
|サイドロード|2 |アプリは、そのアプリがインストールされているユーザー/チームのみが利用できます。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|appdefinitions|[teamsAppDefinition](teamsappdefinition.md)コレクション| アプリの各バージョンの詳細。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>関連項目

- [teamsAppInstallation](teamsappinstallation.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

