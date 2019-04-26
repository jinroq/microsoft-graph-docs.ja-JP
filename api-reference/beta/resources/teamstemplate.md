---
title: teamsTemplate リソースの種類
description: teamsTemplate エンティティについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4e960e85e6e8b3017d8f4e0ab89bb85cb4c12f58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345749"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チームテンプレートは、Microsoft Teams で[チーム](../resources/team.md)を作成するための青写真です。 テンプレートでは、テンプレートを使用して作成された新しいチームでプロビジョニングする必要がある構造、設定、およびコンテンツを指定します。 Microsoft は基本テンプレートのセットを提供しており、お客様は独自のカスタムテンプレートを保存することができます。

## <a name="properties"></a>プロパティ

| プロパティ            | 型     | 説明 |
|:------------------- |:-------- |:----------- |
| id                  | String   | テンプレートの一意識別子。 null にすることはできません。 |

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

