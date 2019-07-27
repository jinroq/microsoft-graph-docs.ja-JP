---
title: userTeamwork リソースの種類
description: 'ユーザー 1 人あたりの使用可能な Microsoft Teams の機能のコンテナ―。 '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d68ceff79856b23f2d86b2c57a6278b7c6ad7e9d
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908587"
---
# <a name="userteamwork-resource-type"></a>userTeamwork リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内のユーザー 1 人あたりの使用可能な Microsoft Teams の機能の範囲のコンテナー。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|id|string| 一意識別子。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:---------------|:--------|:----------|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) コレクション|このユーザーのパーソナル スコープ内にインストールされているアプリ。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
