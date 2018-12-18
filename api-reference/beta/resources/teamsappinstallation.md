---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
author: nkramer
ms.openlocfilehash: cab42c3bc2bde2e20dff3478d432d70e1563d248
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341798"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。 アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[リスト アプリケーション](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | チームでインストールされているアプリケーションを一覧表示します。|
|[アプリを追加します。](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | (インストール) を追加するチームにアプリです。|
|[アプリを抹消します。](../api/teamsappinstallation-delete.md) | なし | 削除 (アンインストール)、チームからのアプリケーションです。|
|[アプリケーションをアップグレードします。](../api/teamsappinstallation-delete.md) | なし | アプリケーションの最新バージョンにアップグレードします。|

## <a name="properties"></a>Properties

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | string   | 一意の id (チームの appid とは異なる)。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ   | 型    | 説明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| インストールされているアプリケーションです。 |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| このバージョンのアプリケーションの詳細。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
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

