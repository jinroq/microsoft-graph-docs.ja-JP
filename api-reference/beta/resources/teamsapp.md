---
title: teamsApp リソースの種類
description: マイクロソフト チーム アプリケーション カタログのアプリケーションです。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b02af5148e40cddd6079de3479767110a9877e4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841574"
---
# <a name="teamsapp-resource-type"></a>teamsApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[マイクロソフト チーム](teams-api-overview.md)アプリケーション カタログのアプリケーションです。

マイクロソフト チーム ストア内のこれらのアプリケーションを表示して、[チーム](team.md)が[チームに追加のアプリケーション](../api/teamsappinstallation-add.md)のメソッドを使用してこれらのアプリケーションをインストールすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[公開されたアプリケーションの一覧を表示します。](../api/teamsapp-list.md) | [teamsApp](teamsapp.md)コレクション | マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。|
|[アプリケーションを発行します。](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | 組織のアプリケーションのカタログには、アプリケーションを発行します。|
|[発行したアプリケーションを更新します。](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 組織のアプリケーションのカタログに公開されたアプリケーションを更新します。|
|[発行したアプリケーションを削除します。](../api/teamsapp-delete.md) | なし | 発行したアプリケーションを組織のアプリケーションのカタログから削除します。|

## <a name="properties"></a>プロパティ

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | 文字列   | カタログ アプリケーションの生成のアプリケーション ID を ([マイクロソフト チーム zip アプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者から提供された ID とは異なる。 |
| externalId          | 文字列   | アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログの ID です。 |
| displayName                | string   | アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログのアプリケーションの名前。 |
| distributionMethod  | teamsAppDistributionMethod     | アプリケーション配布の方法です。 |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod 値

|メンバー|値|説明|
|:---|:---|:---|
|ストア|0| アプリケーションは、マイクロソフトのチームのアプリケーション ストアからのすべてのテナントに使用できます。|
|組織|1|アプリケーションは、このテナントでのみ使用可能です。|
|sideloaded|2|アプリケーションは、ユーザーまたはチームのみ使用可能です、インストールされているをします。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   | 説明 |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md)コレクション| アプリケーションの各バージョンの詳細です。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

