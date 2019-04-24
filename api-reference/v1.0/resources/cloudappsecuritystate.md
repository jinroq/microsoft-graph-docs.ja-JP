---
title: cloudappsecuritystate リソースの種類
description: クラウドアプリケーション (destinationservicename、destinationserviceip) に関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584860"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudappsecuritystate リソースの種類

クラウドアプリケーション (destinationservicename、destinationserviceip) に関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|destinationserviceip|String|クラウドアプリケーション/サービスへの接続の宛先 IP アドレス。|
|destinationservicename|String|クラウドアプリケーション/サービス名 ("Salesforce"、"DropBox" など)。|
|riskScore|String|プロバイダーが生成/計算する、クラウドアプリケーション/サービスのリスクスコア。 推奨値の範囲0-1。パーセンテージに相当します。|

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
