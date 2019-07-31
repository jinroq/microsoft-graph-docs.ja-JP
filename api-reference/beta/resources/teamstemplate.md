---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dde08e6c4ecde3b3a600958a5af5cd93b5fc600f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964390"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チームテンプレートは、Microsoft Teams で[チーム](../resources/team.md)を作成するための青写真です。 テンプレートでは、テンプレートを使用して作成された新しいチームでプロビジョニングする必要がある構造、設定、およびコンテンツを指定します。 Microsoft は基本テンプレートのセットを提供しており、お客様は独自のカスタムテンプレートを保存することができます。

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | String   | テンプレートの一意識別子。 Null にすることはできません。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>関連項目

- [team](team.md)

