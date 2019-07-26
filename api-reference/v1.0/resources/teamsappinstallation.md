---
title: teamsAppInstallation リソースの種類
description: 'チームにインストールされている teamsApp。 '
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b180cae4c700eea31a5d5d9b1504f09ca12c3ae0
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908349"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation リソースの種類

[チーム](team.md)にインストールされている[teamsapp](teamsapp.md) 。 アプリの一部である bot は、アプリが追加されるチームの一部になります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[アプリを一覧表示する](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) | チームにインストールされているアプリを一覧表示します。|
|[アプリの追加](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsappinstallation.md) | アプリをチームに追加 (インストール) します。|
|[アプリの削除](../api/teamsappinstallation-delete.md) | None | チームからアプリを削除 (アンインストール) します。|
|[アプリをアップグレードする](../api/teamsappinstallation-upgrade.md) | None | 最新バージョンのアプリにアップグレードします。|

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 一意の id (teams appid ではない)。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ   | 型    | 説明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| インストールされているアプリ。 |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| このバージョンのアプリの詳細。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>関連項目

- [teamsApp](teamsapp.md)
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
