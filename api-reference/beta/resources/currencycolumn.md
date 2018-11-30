---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074190"
---
# <a name="currencycolumn-resource-type"></a>CurrencyColumn リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**currencyColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 型   | 説明
|:--------------|:-------|:----------------------------------------------------
| **locale**    | 文字列 | 通貨記号を推測するロケールを指定します。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
