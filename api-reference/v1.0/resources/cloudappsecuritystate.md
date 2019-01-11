---
title: cloudAppSecurityState リソースの種類
description: ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876805"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState リソースの種類

ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|クラウド アプリケーションやサービスへの接続の宛先の IP アドレス。|
|destinationServiceName|String|クラウド アプリケーションとサービスの名前 (たとえば「Salesforce」、「ドロップ ボックス」など)。|
|riskScore|String|プロバイダーによって生成されると計算されるリスク スコア クラウド アプリケーションとサービスのです。 0 - 1 パーセントに相当する値の範囲をお勧めします。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
