---
title: referencedObject リソースの種類
description: 同じディレクトリの定義で定義されている別のオブジェクトへの参照について説明します。
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821036"
---
# <a name="referencedobject-resource-type"></a>referencedObject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

同じ[ディレクトリの定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照について説明します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 種類                      | 説明    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |参照先オブジェクトの名前です。 [ディレクトリの定義](synchronization-directorydefinition.md)内のオブジェクトのいずれかに一致する必要があります。|
|referencedProperty          |String                     |**サポートされていません**。 対象の値が、参照として使用されるが、参照されるオブジェクトのプロパティの名前です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
