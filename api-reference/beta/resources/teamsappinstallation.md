---
title: teamsAppInstallation リソースの種類
description: 'チーム、チャット、またはユーザーの個人用スコープにインストールされている teamsApp。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2dd382e21a92662615535f69edc3ca2c99c0d7b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964481"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](team.md)、[チャット](chat.md)、または[ユーザー](user.md)の個人の範囲にインストールされている[teamsapp](teamsapp.md) 。 アプリの一部である bot は、アプリが追加されるチーム、チャット、またはユーザーの個人スコープの一部になります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Team にインストールされているアプリを一覧表示する](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) コレクション | チームにインストールされているアプリを一覧表示します。|
|[アプリをチームに追加する](../api/teamsappinstallation-add.md) |None | アプリをチームに追加 (インストール) します。|
|[チームからアプリを削除する](../api/teamsappinstallation-delete.md) | None | チームからアプリを削除 (アンインストール) します。|
|[Team にインストールされたアプリのアップグレード](../api/teamsappinstallation-upgrade.md) | None | 最新バージョンのアプリにアップグレードします。|
|[ユーザー用にインストールされているアプリを一覧表示する](../api/user-list-teamsappinstallation.md) | [teamsAppInstallation](teamsappinstallation.md) コレクション | ユーザーの個人用スコープにインストールされているアプリを一覧表示します。|
|[ユーザーのアプリを追加する](../api/user-add-teamsappinstallation.md) | | ユーザーの個人スコープにアプリを追加 (インストール) します。|
|[ユーザーのアプリを削除する](../api/user-delete-teamsappinstallation.md) | None | ユーザーの個人スコープでアプリを削除 (アンインストール) します。|
|[ユーザー用のアップグレードアプリがインストールされている](../api/user-upgrade-teamsappinstallation.md) | None | ユーザーの個人スコープにインストールされている最新バージョンのアプリにアップグレードします。|

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 一意の ID (チームの ap ID ではありません)。 |

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
