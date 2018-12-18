---
title: alertTrigger リソースの種類
description: (プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。
author: Preetikr
ms.openlocfilehash: f0888e6caf78d806909f818a8b72fb21320e7796
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341269"
---
# <a name="alerttrigger-resource-type"></a>alertTrigger リソースの種類

(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。

## <a name="properties"></a>Properties

| プロパティ   | 種類|説明|
|:---------------|:--------|:----------|
|名前|String|検出のトリガーとして機能するプロパティの名前です。|
|type|String|解釈のキーと値のペアのプロパティの型。 たとえば、文字列、ブール値などです。|
|value|文字列|検出のトリガーとして機能するプロパティの値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>例

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->