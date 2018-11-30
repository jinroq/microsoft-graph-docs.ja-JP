---
title: networkInterface リソースの種類
description: このホストに関連付けられているネットワーク インターフェイス カード (NIC) を表します。
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067179"
---
# <a name="networkinterface-resource-type"></a>networkInterface リソースの種類

このホストに関連付けられているネットワーク インターフェイス カード (NIC) を表します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|説明|String|NIC の説明 (イーサネット アダプターなどで、ワイヤレス LAN アダプターのローカル エリア接続 * <> # など。)。|
|ipV4Address|String|この NIC に関連付けられている最後の IPv4 アドレス|
|ipV6Address|String|最終公開 (別名) IPv6 グローバル アドレスこの NIC に関連付けられています。|
|localIpV6Address|String|この NIC に関連付けられているローカルの (リンク ローカル アドレスまたはサイト ローカル) IPv6 アドレスを最後します。|
|macAddress|String|このホスト上の NIC の MAC アドレスです。|

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