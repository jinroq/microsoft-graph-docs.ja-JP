---
title: networkInterface リソースの種類
description: このホストに関連付けられているネットワークインターフェイスカード (NIC) を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef932729149ea21580ff5a8f1cc3f52e253bfc50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009616"
---
# <a name="networkinterface-resource-type"></a>networkInterface リソースの種類

このホストに関連付けられているネットワークインターフェイスカード (NIC) を表します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|description|String|NIC の説明 (イーサネットアダプター、ワイヤレス LAN アダプターのローカルエリア接続 * < # > など)。|
|ipV4Address|String|この NIC に関連付けられている最後の IPv4 アドレス。|
|ipV6Address|String|この NIC に関連付けられている最後のパブリック (グローバル) IPv6 アドレス。|
|localIpV6Address|String|この NIC に関連付けられている最後のローカル (リンクローカルまたはサイトローカル) IPv6 アドレス。|
|macAddress|String|このホスト上の NIC の MAC アドレス。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
