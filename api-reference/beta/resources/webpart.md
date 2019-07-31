---
author: rahmit
description: WebPart リソースは、サイトページ上の web パーツの種類とレンダリング情報を表します。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007355"
---
# <a name="webpart-resource"></a>webPart リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**WebPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。

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
| **type**                | String           | WebPart の種類を指定する一意の識別子。 読み取り専用です。
| **data**                | [sitePageData][] | WebPart に必要なプロパティ (webPart によって異なります)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>解説

Web パーツでは、**データ**の下に必要なプロパティを定義できます。

ページの詳細については、「 [Sitepage](sitepage.md)」を参照してください。
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
