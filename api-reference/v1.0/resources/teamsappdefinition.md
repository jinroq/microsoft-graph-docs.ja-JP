---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8fafb266b2bfc2c7ea6e0951ac2906f133817246
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860978"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition リソースの種類



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

