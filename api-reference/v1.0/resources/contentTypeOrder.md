---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder リソースの種類

**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。

## <a name="json-representation"></a>JSON 表記

以下は、**contentTypeOrder** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類    | 説明
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | 既定のコンテンツ タイプかどうか
| **position**  | Int32   | コンテンツ タイプが選択 UI で表示される位置を指定します。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
