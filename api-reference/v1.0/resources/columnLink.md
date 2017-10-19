---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a>ColumnLink リソース型

[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。

[contentType]: contentType.md

## <a name="json-representation"></a>JSON 表記

以下は、**columnLink** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | 列の一意識別子。
| **name**      | string | このコンテンツ タイプの列の名前。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
