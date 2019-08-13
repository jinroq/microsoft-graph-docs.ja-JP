---
title: deviceManagementApplicabilityRuleOsEdition リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0abd5cdde3806b96804f632419e6499be445c16b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332842"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a>deviceManagementApplicabilityRuleOsEdition リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|osEditionTypes|[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)コレクション|適用規則の OS エディションの種類。|
|name|String|オブジェクトの名前を指定します。|
|ruleType|[Devicemanagementの信頼性ルールの種類](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|適用性ルールの種類。 可能な値: `include`、`exclude`。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```



