---
title: plannerUserIds リソースの種類
description: '**PlannerUserIds**リソースは、プランを共有しているユーザー id のリストを表します。 これはオープン型です。 Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループの計画を共有します。 このコレクションにグループの既存のメンバーを追加することもできます。ただし、グループが所有しているプランにアクセスするためには必要ありません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3382da3131040f6ae3dc78102ac6e5d64a23695c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965846"
---
# <a name="planneruserids-resource-type"></a>plannerUserIds リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerUserIds**リソースは、[プラン](plannerplan.md)を共有しているユーザー id のリストを表します。 これはオープン型です。 Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループ[の](group.md)計画を共有します。 このコレクションにグループの既存のメンバーを追加することもできます。ただし、グループが所有しているプランにアクセスするためには必要ありません。


## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは、値が`true`ブール値のプロパティとしてユーザー id を提供する必要があります。 ユーザー id を共有しなくなった場合、プロパティの値を`false` boolean に設定することによってプロパティが自動的に削除されます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

例
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
