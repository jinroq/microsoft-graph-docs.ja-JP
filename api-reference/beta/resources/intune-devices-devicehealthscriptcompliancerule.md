---
title: deviceHealthScriptComplianceRule リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371539"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a>deviceHealthScriptComplianceRule リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|detectionType|[deviceHealthScriptDetectionType](../resources/intune-devices-devicehealthscriptdetectiontype.md)|まだ文書化されていません。 可能な値は、`notConfigured`、`string` です。|
|operator|[deviceHealthScriptComplianceRuleOperator](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|まだ文書化されていません。 可能な値は、`notConfigured`、`equal`、`notEqual` です。|
|detectionValue|String|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



