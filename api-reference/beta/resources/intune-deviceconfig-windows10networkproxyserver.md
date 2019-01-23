---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418583"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




