---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
localization_priority: Normal
ms.openlocfilehash: dda2de3e92128a9813f923d9acfef0eec94680e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510303"
---
# <a name="root-resource-type"></a>Root リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Root** ファセットは、オブジェクトが階層内の最上位であることを示します。
このファセットに値が存在する (null ではない) ことで、オブジェクトがルートであることを示します。
null (または存在しない) 値は、オブジェクトがルートでないことを示します。

**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>プロパティ

**ルート** リソースにはプロパティがありません。


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
