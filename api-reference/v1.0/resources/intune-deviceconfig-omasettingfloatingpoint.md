---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb11f40faf9db58fefb984fcc08a9fedd66e97d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951552"
---
# <a name="omasettingfloatingpoint-resource-type"></a>omaSettingFloatingPoint リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

OMA 設定の浮動小数点の定義です。

[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列|表示名。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|説明|String|説明。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|omaUri|文字列|OMA。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|値|単精度浮動小数点型 (Single)|値。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



