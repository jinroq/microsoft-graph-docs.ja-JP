---
title: alerttrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 9142c4d86b627f1d1e1e790c9b3b279b07005ad2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339161"
---
# <a name="alerttrigger-resource-type"></a>alerttrigger リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
