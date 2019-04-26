---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345793"
---
# <a name="webpart-resource"></a>webPart リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**webPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ                | 型             | 説明
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | webPart の種類を指定する一意の識別子。 読み取り専用です。
| **data**                | [sitepagedata][] | webpart に必要なプロパティ (webpart によって異なります)

[sitepagedata]: sitepagedata.md

## <a name="remarks"></a>注釈

Web パーツでは、**データ**の下に必要なプロパティを定義できます。

ページの詳細については、「 [sitepage](sitepage.md)」を参照してください。
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
