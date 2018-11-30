---
title: alertTrigger リソースの種類
description: (プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。
ms.openlocfilehash: b4af3be67669fd27f27e888cbc28b60b0c1c67a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023539"
---
# <a name="alerttrigger-resource-type"></a>alertTrigger リソースの種類

(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
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

## <a name="example"></a>使用例

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