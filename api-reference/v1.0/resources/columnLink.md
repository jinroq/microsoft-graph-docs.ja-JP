---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: cdae360afb6e626ee481a7e98ed5f90e657203b2
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265121"
---
# <a name="columnlink-resource-type"></a>ColumnLink リソースの種類

[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。

[contentType]: contentType.md

## <a name="json-representation"></a>JSON 表記

以下は、**columnLink** リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 型   | 説明
|:--------------|:-------|:----------------------------------------------------
| **ID**        | 文字列 | 列の一意識別子。
| **name**      | 文字列 | このコンテンツ タイプの列の名前。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
