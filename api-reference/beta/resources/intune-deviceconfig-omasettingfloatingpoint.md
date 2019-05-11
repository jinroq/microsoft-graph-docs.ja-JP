---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4a4b93a7a02dbd221a3c0d75f83eba1c7d4566b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951125"
---
# <a name="omasettingfloatingpoint-resource-type"></a>omaSettingFloatingPoint リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OMA 設定の浮動小数点の定義です。


[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|description|String|説明。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|omaUri|文字列型 (String)|OMA。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|値|単精度浮動小数点型 (Single)|値。|

## <a name="relationships"></a>関係
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




