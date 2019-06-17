---
title: Devicemanagementの信頼性ルール Osversion リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c90a026a231998d7cd3ae25ab55ce63c5edb553
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002505"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a>Devicemanagementの信頼性ルール Osversion リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|minOSVersion|String|適用ルールの最小 OS バージョン。|
|maxOSVersion|String|適用ルールの最大 OS バージョン。|
|name|String|オブジェクトの名前を指定します。|
|ruleType|[Devicemanagementの信頼性ルールの種類](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|適用性ルールの種類。 可能な値: `include`、`exclude`。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```





