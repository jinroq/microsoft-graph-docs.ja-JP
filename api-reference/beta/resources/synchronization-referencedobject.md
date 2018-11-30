---
title: referencedObject リソースの種類
description: 同じディレクトリの定義で定義されている別のオブジェクトへの参照について説明します。
ms.openlocfilehash: 63645048fd8ba6ad949da43baa261b2842ea4016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073705"
---
# <a name="referencedobject-resource-type"></a>referencedObject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

同じ[ディレクトリの定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照について説明します。

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
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
            