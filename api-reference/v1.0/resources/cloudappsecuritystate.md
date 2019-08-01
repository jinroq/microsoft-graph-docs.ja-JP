---
title: cloudAppSecurityState リソースの種類
description: クラウドアプリケーション (destinationServiceName、destinationServiceIp) に関するステートフルな情報を含みます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e000d5d788a293c9aed7b702da2653f42116c0c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029716"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState リソースの種類

クラウドアプリケーション (destinationServiceName、destinationServiceIp) に関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|クラウドアプリケーション/サービスへの接続の宛先 IP アドレス。|
|destinationServiceName|String|クラウドアプリケーション/サービス名 ("Salesforce"、"DropBox" など)。|
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
