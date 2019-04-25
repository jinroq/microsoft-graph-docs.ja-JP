---
title: referencedobject リソースの種類
description: 同じディレクトリ定義で定義されている別のオブジェクトへの参照を記述します。
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523246"
---
# <a name="referencedobject-resource-type"></a>referencedobject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同じ[ディレクトリ定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照を記述します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |参照されるオブジェクトの名前を指定します。 [ディレクトリ定義](synchronization-directorydefinition.md)内のいずれかのオブジェクトと一致している必要があります。|
|referencedproperty          |String                     |**現時点ではサポートされていません**。 参照されるオブジェクト内のプロパティの名前。その値は、参照として使用されます。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
