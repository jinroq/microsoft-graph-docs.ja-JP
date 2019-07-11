---
title: referencedObject リソースの種類
description: 同じディレクトリ定義で定義されている別のオブジェクトへの参照を記述します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b06bac82ca78c3d249d3b173c0db7f72a953e2d2
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620452"
---
# <a name="referencedobject-resource-type"></a>referencedObject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同じ[ディレクトリ定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照を記述します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |参照されるオブジェクトの名前を指定します。 [ディレクトリ定義](synchronization-directorydefinition.md)内のいずれかのオブジェクトと一致している必要があります。|
|referencedProperty          |String                     |**現時点ではサポートされていません**。 参照されるオブジェクト内のプロパティの名前。その値は、参照として使用されます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
