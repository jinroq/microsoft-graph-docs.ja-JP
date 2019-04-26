---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f95201a725969fa125cdf949874686b9155fc3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568795"
---
# <a name="omasettingstringxml-resource-type"></a>omaSettingStringXml リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OMA 設定文字列の XML 定義です。


[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|説明|String|説明。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|omaUri|文字列|OMA。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|fileName|文字列型 (String)|Value プロパティに関連付けられているファイル名 (*.xml)。|
|value|バイナリ型 (Binary)|値。 (UTF8 でエンコードされたバイト配列)|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



