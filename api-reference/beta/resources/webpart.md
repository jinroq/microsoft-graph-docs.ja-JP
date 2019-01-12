---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9147d434a94380c4d178efdf80ccba90734bf96f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939043"
---
# <a name="webpart-resource"></a>web パーツ リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>プロパティ

| プロパティ                | 種類             | 説明
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | Web パーツの種類を指定する一意の識別子です。 読み取り専用です。
| **data**                | [sitePageData][] | Web パーツ (web パーツによって異なります) に必要なプロパティ

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>解説

Web パーツは、[**データ**の独自の必要なプロパティを定義できます。

ページの詳細については、 [sitePage](sitepage.md)を参照してください。
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
