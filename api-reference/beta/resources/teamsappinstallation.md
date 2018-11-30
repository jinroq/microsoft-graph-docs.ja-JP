---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
ms.openlocfilehash: 64573e163c0ec5ce9f3282e747dffd4ccc6718de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069479"
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

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | 文字列   | 一意の id (チームの appid とは異なる)。 |

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

