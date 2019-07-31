---
title: プラン "お気に入り" プラン参照リソースの種類
description: 'プラン [**参照**リソースの種類表す workbookconnection は、ユーザーによってお気に入りとしてマークされているプランへの参照を示します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07803375ca31162f0f7e392d81edb83ab2bd6da3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009070"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>プラン "お気に入り" プラン参照リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プラン [**参照**リソースの種類表す workbookconnection は、ユーザーによってお気に入りとしてマークされている[プラン](plannerplan.md)への参照を示します。 クライアントは、「 **** プラン」では、削除されたプラン、ユーザーがアクセスできなくなったプラン、または別のタイトルで更新された**プラン**を参照することができることに注意してください。

クライアントは、相違点がある場合にユーザーに通知し、エントリを最新の状態に維持することをお勧めします。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|orderHint|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](planner-order-hint-format.md)」で定義されています。|
|プランのタイトル|String|ユーザーがお気に入りとしてマークした時点でのプランのタイトル。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
