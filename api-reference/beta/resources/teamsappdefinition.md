---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
ms.openlocfilehash: 71a1783131661aed120f375f7cc58d55fb0ca0d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336835"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。

## <a name="properties"></a>Properties

| プロパティ            | 種類     | 説明 |
|:------------------- |:-------- |:----------- |
| ID                  | string   | 一意の id (チームの appid とは異なる)。 |
| teamsAppId          | string   | チームのアプリケーション マニフェストの id です。 |
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

