---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 312b9347519935c4ff34f51cee24e0082c3da58e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969766"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。

## <a name="properties"></a>プロパティ

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | 文字列   | 一意の id (チームの appid とは異なる)。 |
| teamsAppId          | 文字列   | チームのアプリケーション マニフェストの id です。 |
| displayName         | string   | アプリケーション開発者によって提供されるアプリケーションの名前。 |
| version             | 文字列   | アプリケーションのバージョン番号です。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a>関連項目

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
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

