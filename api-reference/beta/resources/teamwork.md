---
title: teamwork リソースの種類
description: 組織で使用可能な Microsoft Teams の機能のコンテナー。
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908594"
---
# <a name="teamwork-resource-type"></a>teamwork リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織で使用可能な Microsoft Teams の機能の範囲のコンテナー。

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
  "@odata.type": "microsoft.graph.teamwork",
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
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>関連項目

- [userTeamwork リソース](userteamwork.md)
