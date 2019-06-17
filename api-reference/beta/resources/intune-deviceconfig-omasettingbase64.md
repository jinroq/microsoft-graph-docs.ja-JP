---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ecb77bc317216e77cb53c31b8be9bded9cafc19
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995554"
---
# <a name="omasettingbase64-resource-type"></a>omaSettingBase64 リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OMA 設定の Base64 定義。


[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|description|String|説明。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|omaUri|String|OMA。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|fileName|String|Value プロパティに関連付けられているファイル名 (*.cer | * .crt | *. p7b | * .bin)。|
|value|文字列|値。 (Base64 エンコード文字列)|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```





