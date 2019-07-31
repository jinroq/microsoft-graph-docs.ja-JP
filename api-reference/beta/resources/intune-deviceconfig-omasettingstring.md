---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c54bdab0870dfd4f3b28ae0af9036682f0464a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969948"
---
# <a name="omasettingstring-resource-type"></a>omaSettingString リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OMA 設定の文字列の定義です。


[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|description|String|説明。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|omaUri|文字列型 (String)|OMA。 [omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承|
|value|文字列|値。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```





