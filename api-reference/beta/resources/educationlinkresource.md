---
title: educationLinkResource リソースの種類
description: EducationResource のサブクラスです。 このリソースは、リンクとは必要なデータに関連付けられていないことです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8cdcb47c02481f2f43ee71f46c24e2b8d8f5ba2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918050"
---
# <a name="educationlinkresource-resource-type"></a>educationLinkResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[EducationResource](educationresource.md)のサブクラスです。 このリソースは、リンクとは必要なデータに関連付けられていないことです。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|link|String|リソースへの URL です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
