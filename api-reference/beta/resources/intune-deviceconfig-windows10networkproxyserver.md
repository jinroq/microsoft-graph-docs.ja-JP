---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f29c69789f6b2a4d41bbb5179ff71f721c64c88f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162105"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ネットワーク プロキシ サーバーのポリシーです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|address|String|プロキシ サーバーへのアドレス。 <server>\[“:”<port>\] 形式でアドレスを指定します|
|exceptions|String コレクション|プロキシ サーバーを使用できないアドレス。 システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。|
|useForLocalAddresses|Boolean|ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```




