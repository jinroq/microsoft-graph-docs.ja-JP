---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 原因
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563144"
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
  "suppressions": []
}
-->
