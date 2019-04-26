---
title: alerttrigger リソースの種類
description: 検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569467"
---
# <a name="alerttrigger-resource-type"></a>alerttrigger リソースの種類

検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|name|String|検出トリガーとして機能するプロパティの名前。|
|type|String|キーと値のペアで解釈するプロパティの型。 たとえば、String、Boolean、などです。|
|value|文字列型 (String)|検出トリガーとして提供されるプロパティの値。|

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
