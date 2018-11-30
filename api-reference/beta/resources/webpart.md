---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069476"
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

| プロパティ                | 型             | 説明
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | Web パーツの種類を指定する一意の識別子です。 読み取り専用。
| **データ**                | [sitePageData][] | Web パーツ (web パーツによって異なります) に必要なプロパティ

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
