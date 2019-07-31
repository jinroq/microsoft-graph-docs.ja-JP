---
title: teamsApp リソースの種類
description: Microsoft Teams アプリカタログの一つ。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f629851225570426b5785911bbbdb3337f43149f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964509"
---
# <a name="teamsapp-resource-type"></a>teamsApp リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Microsoft Teams](teams-api-overview.md)アプリカタログの一つ。

ユーザーはMicrosoft Teams Storeでこれらのアプリを見ることができ、これらのアプリを[Teams へのアプリを追加](../api/teamsappinstallation-add.md)方法を使用して[teams](team.md) にインストールすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[公開アプリ をリストする](../api/teamsapp-list.md) | [teamsApp](teamsapp.md) コレクション | Microsoft Teams アプリ カタログから公開されたアプリの一覧を表示します。|
|[アプリを発行します。](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | アプリを組織のアプリ カタログに発行します。|
|[公開済みのアプリを更新します。](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 組織のアプリ カタログに発行したアプリを更新します。|
|[公開済みのアプリを削除します。](../api/teamsapp-delete.md) | なし | 組織のアプリ カタログに発行したアプリを削除します。|

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | カタログアプリによって生成されたアプリID（[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)内の開発者提供のIDとは異なります）。 |
| 外部ID          | 文字列   | アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログのID。 |
| displayName                | string   | アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログアプリの名前。 |
| distributionMethod  | teamsAppDistributionMethod     | アプリの配布の方法です。 |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod 値

|メンバー|値|説明|
|:---|:---|:---|
|店|0| このアプリは、Microsoft Teamsアプリストアを通じてすべてのテナントに利用可能です。|
|組織|1|アプリは、このテナントでのみ使用できます。|
|sideloaded|2|アプリはそれがインストールされているユーザー/チームにのみ利用可能です。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md)コレクション| アプリの各バージョンの詳細。 |

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
  "suppressions": []
}
-->

