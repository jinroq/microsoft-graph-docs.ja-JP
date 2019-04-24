---
title: networkInterface リソースの種類
description: このホストに関連付けられているネットワークインターフェイスカード (NIC) を表します。
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457068"
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
